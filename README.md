# Guia Prático para Desenvolvimento de Software com IA

Este repositório é um guia e um conjunto de ferramentas para utilizar a Inteligência Artificial como uma parceira ativa no ciclo de vida de desenvolvimento de software, desde a concepção até a operação.

---

## 🚀 O que é este Repositório?

Este projeto fornece uma metodologia estruturada e um conjunto de **templates de prompt reutilizáveis** para criar "agentes de IA" especializados em tarefas de desenvolvimento de software. O objetivo é ir além de prompts simples e construir assistentes que entendem o contexto do seu projeto e o guiam ativamente na criação de documentação, arquitetura e muito mais.

Aqui você encontrará:
- 📖 Uma **metodologia** focada em "Context Engineering".
- 🤖 **Templates de Agente** prontos para serem usados em plataformas como ChatGPT (Custom GPTs) e Cursor.
- 📝 **Exemplos** de prompts e documentos gerados.

---

## 🛠️ Como Usar os Templates de Agente

O coração deste repositório está na pasta `templates/agents/prompts`. Cada arquivo `.md` contém as instruções para criar um agente especializado.

### Método 1: Criando um Agente no ChatGPT (Custom GPTs)

1.  **Acesse o Criador de GPTs:** Em "Explore", clique em "Create a GPT".
2.  **Configure as Instruções:** Vá para a aba "Configure". Copie todo o conteúdo de um dos nossos templates (ex: `templates/agents/prompts/prd_agent_prompt.md`) e cole no campo "Instructions".
3.  **Adicione Conhecimento:** Na seção "Knowledge", faça o upload dos documentos de contexto do seu projeto (como `context.md`, `architecture.md` ou o próprio `README.md` do seu projeto). Isso dará ao seu agente o conhecimento específico do seu software.
4.  **Teste e Salve:** Interaja com o agente no painel de "Preview" para ver se ele se comporta como esperado e, em seguida, salve-o para uso futuro.

### Método 2: Usando com o Cursor (ou outra IA no seu Editor)

1.  **Referencie o Agente:** Comece sua conversa com a IA referenciando o template que deseja usar. Ex: `"Quero criar um ADR. Use as instruções de @templates/agents/prompts/adr_agent_prompt.md para me guiar."`
2.  **Interaja:** A IA irá ler o arquivo e começar a fazer as perguntas definidas no template.
3.  **Construa o Documento:** Responda às perguntas e a IA montará o documento final para você.

---

## 📁 Estrutura do Repositório

- **`templates/agents/prompts/`**: Contém os templates de prompt para criar agentes interativos. **Este é o principal diretório a ser usado.**
- **`agentic-ai/`**: Contém os exemplos originais de prompts não-interativos e documentos gerados. Serve como um bom material de referência e estudo.
- **`README.md`**: Este arquivo.

---

## 🧠 A Metodologia: Conceitos-Chave

A eficácia dos agentes se baseia em alguns conceitos fundamentais:

### 1. Context Engineering
Mais importante do que "saber pedir" (Prompt Engineering), é a engenharia de **o quê, como e quando** entregar contexto à IA. Isso inclui:
- **Prompt Engineering:** As instruções que definem o comportamento do agente.
- **RAG (Retrieval-Augmented Generation):** A capacidade do agente de consultar documentos externos (o "Knowledge" nos GPTs) para obter respostas mais precisas e contextualizadas.
- **Histórico e Estado:** A memória da conversa para manter a continuidade.

### 2. RAG — Retrieval-Augmented Generation
É a técnica que permite que a IA utilize dados que não estão em seu treinamento original. Ao fornecer documentos (`context.md`, `README.md` do seu projeto), a IA pode "ler" e usar essas informações para gerar respostas muito mais relevantes para o seu caso de uso específico, reduzindo "alucinações".

### 3. Protocolos e Segurança
Para sistemas mais complexos, o `README.md` original detalha o **MCP (Multi-Agent Communication Protocol)**, um protocolo para comunicação entre múltiplos agentes, e a importância de **Guardrails** para a segurança da IA.

---

## 🤖 Modelos de Agentes Disponíveis

Você encontrará templates para os seguintes agentes em `templates/agents/prompts/`:

-   **`prd_agent_prompt.md`**: Para gerar um **Product Requirements Document (PRD)**.
-   **`adr_agent_prompt.md`**: Para gerar um **Architecture Decision Record (ADR)**.
-   **`engineering_guidelines_agent_prompt.md`**: Para criar **Diretrizes de Engenharia** (Padrões de Código, Workflows, etc.).
-   **`system_design_agent_prompt.md`**: Para gerar um **System Design Document (SDD)**.
-   **`c4_model_agent_prompt.md`**: Para criar diagramas do **Modelo C4** (Contexto, Contêineres, Componentes).
-   **`runbook_agent_prompt.md`**: Para gerar **Runbooks** operacionais.
-   **`postmortem_agent_prompt.md`**: Para facilitar e documentar relatórios de **Postmortem**.
-   **`context_md_agent_prompt.md`**: Para gerar um arquivo **`context.md`** que resume o contexto de um projeto.
-   **`architecture_md_agent_prompt.md`**: Para gerar um arquivo **`architecture.md`** que resume a arquitetura técnica.

---

## Conclusão

Com essa estrutura, é possível criar um ecossistema de desenvolvimento moderno, onde a IA desempenha um papel ativo na documentação, execução e melhoria contínua de projetos. A organização de dados, prompts e contexto é essencial para desbloquear a produtividade real com assistentes de IA.

---

## Créditos

Este projeto foi idealizado e estruturado por Elone Izata Sampaio.
