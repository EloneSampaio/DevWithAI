
# Estrutura Base para Projetos com Integração de IA

Este documento apresenta três modelos de estrutura de pastas e arquivos recomendados para projetos com foco em IA, engenharia de contexto, RAG e agentes inteligentes.

---

## 🔧 Opção 1 – Estrutura Padrão Simples (Lean & Clean)

> Ideal para MVPs, projetos pequenos, protótipos, uso pessoal ou consultorias rápidas.

```
project-root/
├── README.md
├── .env.example
├── docs/
│   ├── context.md
│   └── architecture.md
├── prompts/
│   └── base_prompt.md
├── prps/
│   └── prp_example.md
├── scripts/
│   └── generate_embeddings.py
├── data/
│   ├── raw/
│   └── processed/
├── app/
│   ├── main.py
│   └── utils.py
```

---

## 🧠 Opção 2 – Estrutura Modular para IA com Agentes e RAG

> Ideal para aplicações que integram agentes, automações, RAG e documentação técnica estruturada.

```
project-root/
├── README.md
├── .env.example
├── docs/
│   ├── context.md
│   ├── architecture.md
│   ├── glossary.md
│   └── research.md
├── prompts/
│   ├── base_prompt.md
│   ├── rag_prompt.md
│   └── validation.md
├── prps/
│   ├── prp_base.md
│   ├── prp_rag.md
│   └── prp_mcp.md
├── workflows/
│   ├── plan_global.md
│   ├── plan_prompt.md
│   └── plan_ia.md
├── agents/
│   ├── registry.json
│   └── strategies/
│       ├── rag_agent.py
│       └── planning_agent.py
├── scripts/
│   ├── ingest_data.py
│   └── validate_outputs.py
├── data/
│   ├── sources/
│   └── embeddings/
├── tests/
│   ├── test_agents.py
│   └── test_rag.py
└── MCP/
    ├── session.json
    ├── tools.json
    └── stream_example.json
```

---

## 🏢 Opção 3 – Estrutura Enterprise Ready (Full CM + RAG + Avaliação)

> Ideal para times, produtos com múltiplos fluxos, agentes coordenados, e pipelines de IA em produção.

```
project-root/
├── README.md
├── LICENSE
├── .env.example
├── configs/
│   ├── project.yaml
│   └── agents.yaml
├── docs/
│   ├── context.md
│   ├── architecture.md
│   ├── decisions/
│   │   ├── adr-001-context-engineering.md
│   │   └── adr-002-rag-setup.md
│   ├── glossary.md
│   └── team_roles.md
├── prompts/
│   ├── system/
│   │   ├── base.md
│   │   └── meta_agent.md
│   ├── tasks/
│   │   ├── rag.md
│   │   └── validation_loop.md
│   └── evaluation/
│       ├── eval_instructions.md
│       └── rubrics.md
├── prps/
│   ├── base.md
│   ├── prp_auth_feature.md
│   ├── prp_vector_storage.md
│   └── prp_agent_decision.md
├── workflows/
│   ├── global.md
│   ├── per_feature.md
│   └── auto_generated.md
├── agents/
│   ├── registry.json
│   ├── handlers/
│   │   ├── rag_handler.py
│   │   └── planner_handler.py
│   └── memory/
│       ├── vector_store.py
│       └── history_manager.py
├── scripts/
│   ├── init_pipeline.py
│   ├── generate_embeddings.py
│   └── evaluate_output.py
├── data/
│   ├── ingestion/
│   ├── processed/
│   └── logs/
├── tests/
│   ├── unit/
│   ├── integration/
│   └── eval/
└── MCP/
    ├── schemas/
    │   └── tool_schema.json
    ├── sessions/
    │   └── example_session.json
    └── messages/
        └── stream_example.json
```

---

Escolha a estrutura que mais se adapta ao seu contexto de projeto e equipe.
