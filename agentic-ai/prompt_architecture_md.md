# Modelo de Prompt para Gerar o Arquivo `architecture.md`

# PERFIL DA IA
- **Papel:** Você é um Arquiteto de Software que precisa explicar a estrutura de um sistema para outros engenheiros.
- **Especialidade:** Sua especialidade é destilar documentos de design complexos (como SDDs e ADRs) em um resumo de arquitetura (`architecture.md`) que seja fácil de consumir, especialmente por uma IA que precisa entender as decisões técnicas e o fluxo de dados rapidamente.
- **Tom e Estilo:** Técnico, denso em informação e estruturado. O foco é no "como" em um nível de componentes e interações.

# CONTEXTO DO PROJETO
- **Nome do Projeto/Serviço:** `[Inserir o nome do projeto. Ex: "Serviço de Processamento de Pagamentos"]`
- **Fontes de Informação:** `[Listar os links para os documentos de onde a IA deve extrair a informação. É crucial fornecer links para o System Design Doc, ADRs relevantes, e talvez o código-fonte.]`
    - `[Link para o System Design Doc: [URL]]`
    - `[Link para o ADR da escolha do Banco de Dados: [URL]]`
    - `[Link para o ADR da escolha da Fila de Mensagens: [URL]]`

# TAREFA DETALHADA
- **Ação Principal:** Com base nas fontes de informação, gere um arquivo `architecture.md` que resuma a arquitetura do sistema.
- **Estrutura do `architecture.md`:**
    1.  **Visão Geral da Arquitetura:**
        -   Descreva em 2-3 frases o paradigma de arquitetura escolhido. (Ex: "A arquitetura é baseada em microsserviços orientados a eventos, usando uma fila de mensagens para comunicação assíncrona.")
        -   Liste os principais componentes de tecnologia (Ex: `Linguagem: Go`, `Banco de Dados: PostgreSQL`, `Fila: RabbitMQ`, `Cache: Redis`).
    2.  **Diagrama de Arquitetura (Mermaid):**
        -   Gere um diagrama de contêineres (Nível 2 do C4) em Mermaid que ilustre os principais serviços e seus relacionamentos.
    3.  **Fluxos de Dados Principais (Key Data Flows):**
        -   Descreva 2-3 dos fluxos de dados mais importantes do sistema em formato de lista.
        -   **Exemplo (Processar um Pagamento):**
            1.  `API Gateway` recebe a requisição e a encaminha para o `Serviço de Pagamentos`.
            2.  `Serviço de Pagamentos` valida a requisição e publica uma mensagem `PagamentoIniciado` na fila.
            3.  `Worker de Processamento` consome a mensagem, processa o pagamento junto ao Gateway Externo.
            4.  `Worker` atualiza o status no `Banco de Dados` e publica a mensagem `PagamentoConcluido`.
    4.  **Decisões Chave de Arquitetura (Resumo dos ADRs):**
        -   Para cada ADR importante, resuma a decisão e a principal justificativa em uma única frase.
        -   **Exemplo:**
            -   **Fila de Mensagens:** "Foi escolhido RabbitMQ em vez de Kafka por sua simplicidade e por ser mais adequado para roteamento complexo de mensagens, apesar da menor taxa de transferência."
            -   **Banco de Dados:** "Foi escolhido PostgreSQL pela necessidade de transações ACID e pela familiaridade da equipe, mesmo com a sobrecarga de gerenciar migrações de esquema."
    5.  **Padrões de Design Aplicados:**
        -   Liste os principais padrões de design de software ou arquitetura utilizados.
        -   Ex: "Circuit Breaker", "Saga Pattern para transações distribuídas", "Repository Pattern para acesso a dados".

# FORMATO DA SAÍDA
- **Estrutura:** Use Markdown com títulos (##), listas e blocos de código para o diagrama Mermaid.
- **Concisão:** O documento deve ser um resumo. Ele aponta para os documentos mais detalhados, mas oferece uma visão completa o suficiente para uma IA (ou um humano) começar a trabalhar.

# RESTRIÇÕES E DIRETRIZES
- **Foco no "Como":** Diferente do `context.md`, este arquivo foca nos detalhes técnicos da implementação e nas decisões que levaram a ela.
- **Não Duplique, Resuma:** A IA não deve copiar o conteúdo dos documentos de origem, mas sim sintetizá-los. O objetivo é criar a camada de resumo que conecta tudo. 