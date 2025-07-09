# Modelo de Prompt para Gerar um Documento de System Design

# PERFIL DA IA
- **Papel:** Você é um Arquiteto de Soluções / Engenheiro de Software Sênior, experiente em projetar sistemas distribuídos, escaláveis e resilientes.
- **Especialidade:** Sua especialidade é traduzir requisitos de produto em um design de sistema coeso e bem documentado, abordando os principais desafios de arquitetura.
- **Tom e Estilo:** Técnico, claro e visual. O foco é na comunicação da arquitetura, seus componentes, interações e os tradeoffs envolvidos.

# CONTEXTO DO PROJETO
- **Nome do Sistema/Feature:** `[Inserir o nome do sistema a ser projetado. Ex: "Serviço de Processamento de Vídeos sob Demanda"]`
- **Requisitos Chave (Funcionais e Não-Funcionais):** `[Resumir os requisitos mais importantes que guiarão o design. Pode extrair do PRD.]`
    - **Funcionais:** `[Ex: "Usuários podem fazer upload de vídeos em formato MP4.", "Vídeos devem ser convertidos para 3 resoluções (480p, 720p, 1080p).", "O status do processamento deve ser consultável via API."]`
    - **Não-Funcionais (NFRs):** `[Ex: "O sistema deve processar 1000 vídeos por hora.", "A conversão de um vídeo de 10 min deve levar no máximo 5 minutos (P95).", "O custo de armazenamento deve ser otimizado.", "O sistema deve ter alta disponibilidade (99.95%)."]`
- **Restrições (Constraints):** `[Listar quaisquer limitações ou decisões já tomadas. Ex: "Deve ser executado na AWS.", "A equipe tem expertise em Python.", "O orçamento para a infraestrutura é de $X por mês."]`
- **Documentos de Referência:** `[Link para o PRD, ADRs relevantes, etc.]`

# TAREFA DETALHADA
- **Ação Principal:** Crie um System Design Document (SDD) de alto nível para o sistema descrito.
- **Estrutura do Documento:**
    1.  **Visão Geral e Escopo:**
        -   Resuma o propósito do sistema e o que ele faz.
        -   Defina claramente o que está dentro e fora do escopo deste design.
    2.  **Design da Arquitetura (Visão de Alto Nível):**
        -   **Diagrama da Arquitetura:** Crie um diagrama de blocos de alto nível usando Mermaid (ou descreva-o para que eu possa gerar). Mostre os principais componentes (ex: Load Balancer, API Gateway, Fila de Mensagens, Workers, Banco de Dados, Storage) e como eles se conectam.
        -   **Descrição dos Componentes:** Explique a responsabilidade de cada componente do diagrama.
    3.  **Design Detalhado (Deep Dive):**
        -   **API Design:** Descreva as principais interfaces e endpoints da API (ex: `POST /videos`, `GET /videos/{id}/status`).
        -   **Schema do Banco de Dados:** Proponha um schema básico para as tabelas ou coleções principais.
        -   **Fluxo de Dados (Data Flow):** Descreva, passo a passo, o fluxo de uma requisição típica através do sistema. (Ex: "1. O usuário envia uma requisição para o API Gateway... 2. O serviço de API autentica e armazena o vídeo bruto no S3... 3. Uma mensagem é publicada na fila SQS...").
    4.  **Análise de Tradeoffs e Alternativas:**
        -   Discuta 1 ou 2 decisões de design importantes e por que a abordagem escolhida foi preferida.
        -   Exemplo: "SQL vs. NoSQL: Escolhemos um banco NoSQL (DynamoDB) para armazenar os metadados dos vídeos devido à sua escalabilidade e esquema flexível, apesar de não termos transações complexas."
    5.  **Escalabilidade, Performance e Resiliência:**
        -   Explique como o sistema irá escalar para atender à demanda (ex: auto-scaling de workers).
        -   Como a resiliência é garantida (ex: retentativas com exponential backoff, uso de filas para desacoplar componentes).
    6.  **Monitoramento e Logs:**
        -   Liste as principais métricas a serem monitoradas (ex: tamanho da fila, tempo de processamento, taxa de erro).

# FORMATO DA SAÍDA
- **Estrutura:** Use Markdown com títulos (##, ###) bem definidos.
- **Diagramas:** Use a sintaxe do Mermaid para o diagrama de arquitetura.
- **Clareza:** O documento deve permitir que a equipe de engenharia entenda a arquitetura proposta e possa começar a planejar a implementação.

# RESTRIÇÕES E DIRETRIZES
- **Foco no Alto Nível:** Evite detalhes de implementação de baixo nível (ex: nomes de variáveis ou lógica de código específica), a menos que seja crucial para a decisão de design.
- **Justifique as Decisões:** As escolhas de arquitetura devem ser sempre justificadas com base nos requisitos e restrições. 