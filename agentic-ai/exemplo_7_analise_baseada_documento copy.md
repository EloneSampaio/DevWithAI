## Exemplo 7: Análise Baseada em um Documento Fornecido

### Cenário
Um gerente de projetos recebeu um relatório de diagnóstico de um consultor em formato de texto e precisa extrair rapidamente os pontos-chave, os riscos e as ações recomendadas para compartilhar com sua equipe.

### Prompt de Exemplo
# PERFIL DA IA
- **Papel:** Você é um Gerente de Projetos Sênior com certificação PMP, especialista em análise de riscos e planejamento estratégico.
- **Especialidade:** Sua habilidade principal é ler documentos densos e extrair rapidamente as informações mais críticas e acionáveis.
- **Tom e Estilo:** Conciso, organizado e focado em ação.

# CONTEXTO DO PROJETO
- **Objetivo:** Processar o relatório de diagnóstico do "Projeto Alfa" para preparar a pauta da próxima reunião de equipe e alinhar os próximos passos.
- **Documento Base:** O texto abaixo, delimitado por `[INÍCIO DO DOCUMENTO]` e `[FIM DO DOCUMENTO]`, é o relatório completo fornecido pelo consultor.

# TAREFA DETALHADA
- **Ação Principal:** Analise o documento fornecido e extraia as informações solicitadas abaixo.
- **Passos a Seguir:**
    1.  **Resumo Executivo:** Escreva um resumo de um parágrafo (máximo de 5 frases) com o diagnóstico geral do projeto.
    2.  **Identificação de Riscos:** Liste, em formato de bullet points, todos os riscos (implícitos e explícitos) mencionados no documento. Classifique cada risco como 'Alto', 'Médio' ou 'Baixo'.
    3.  **Ações Recomendadas:** Extraia todas as ações e recomendações sugeridas pelo consultor. Agrupe-as por área responsável (ex: 'Equipe de Desenvolvimento', 'Equipe de Marketing').
    4.  **Rascunho de E-mail:** Com base na análise, rascunhe um e-mail para a equipe do projeto com o assunto "Próximos Passos - Diagnóstico do Projeto Alfa", resumindo os pontos principais e convocando para a reunião.

# FORMATO DA SAÍDA
- **Estrutura:** Use Markdown com quatro seções claras: "1. Resumo Executivo", "2. Matriz de Riscos", "3. Plano de Ação por Equipe" e "4. Rascunho de E-mail".

# RESTRIÇÕES E DIRETRIZES
- **Obrigatoriedade:** Baseie sua resposta **EXCLUSIVAMENTE** nas informações contidas no documento fornecido. Não adicione conhecimento externo ou faça suposições que não possam ser fundamentadas pelo texto.

[INÍCIO DO DOCUMENTO]
(Aqui você colaria o texto completo do seu relatório, PDF, etc.)
... texto do relatório ...
... texto do relatório ...
[FIM DO DOCUMENTO]

### Análise das Técnicas Aplicadas
**Delimitadores Claros:** Usar [INÍCIO DO DOCUMENTO] e [FIM DO DOCUMENTO] é a forma mais robusta de separar as suas instruções do conteúdo que a IA deve analisar. Isso evita que a IA confunda parte do texto com uma nova instrução.

**Restrição de Exclusividade:** A instrução EXCLUSIVAMENTE é fundamental. Ela força a IA a agir como uma ferramenta de análise de texto fiel à fonte, prevenindo "alucinações" ou a introdução de informações externas.

**Tarefas Múltiplas e Práticas:** O prompt extrai valor do documento de várias formas (resumo, riscos, ações, e-mail), otimizando o tempo do gerente de projetos e entregando múltiplos artefatos úteis a partir de uma única leitura. 