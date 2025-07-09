# Guia Prático de Prompts de IA

## Introdução

Este guia fornece exemplos práticos de prompts eficientes para diferentes cenários de uso. Cada exemplo segue uma estrutura consistente que inclui:
- Cenário: Descrição do contexto e necessidade
- Prompt: Estrutura detalhada do prompt
- Análise: Explicação das técnicas utilizadas e por que funcionam

## Estrutura dos Prompts

Cada prompt segue o seguinte template:
1. **PERFIL DA IA**: Define o papel e especialidade do assistente
2. **CONTEXTO DO PROJETO**: Fornece informações essenciais sobre o projeto
3. **TAREFA DETALHADA**: Especifica o que precisa ser feito
4. **FORMATO DA SAÍDA**: Define como a resposta deve ser estruturada
5. **RESTRIÇÕES E DIRETRIZES**: Estabelece limites e requisitos específicos

## Índice de Exemplos
1. [Desenvolvimento (Nova Feature)](#exemplo-1-desenvolvimento-de-nova-feature)
2. [Arquitetura (Escolha de Tecnologia)](#exemplo-2-escolha-de-tecnologia)
3. [Negócios (Pesquisa de Mercado)](#exemplo-3-pesquisa-de-mercado)
4. [Educacional (Pesquisa Histórica)](#exemplo-4-pesquisa-de-fato-histórico)
5. [Marketing (Análise de Conteúdo)](#exemplo-5-análise-comparativa-usando-links)
6. [Investimentos (Pesquisa Aprofundada)](#exemplo-6-pesquisa-de-mercado-com-busca-profunda)
7. [Gestão (Análise de Documentos)](#exemplo-7-análise-baseada-em-um-documento-fornecido)

Cada exemplo inclui:
- 📝 Cenário detalhado
- 🎯 Prompt estruturado
- 📊 Análise das técnicas utilizadas

## Exemplo 1: Desenvolvimento de Nova Feature

### Cenário
Uma equipe de produto precisa planejar a implementação de um sistema de "gamificação" (conquistas e pontos) em um aplicativo de aprendizado de idiomas para aumentar o engajamento dos usuários.

### Prompt de Exemplo
# PERFIL DA IA
- **Papel:** Você é um híbrido de Gerente de Produto Sênior e Engenheiro de Software Tech Lead, com vasta experiência em desenvolvimento de aplicativos mobile e em estratégias de engajamento de usuários.
- **Especialidade:** Sua especialidade é a implementação de sistemas de gamificação (streaks, pontos, badges, leaderboards) em plataformas educacionais.
- **Tom e Estilo:** Estratégico, técnico e pragmático. Foque em soluções viáveis e um plano de ação claro.

# CONTEXTO DO PROJETO
- **Produto:** Aplicativo de aprendizado de idiomas chamado "LinguaBoost".
- **Objetivo Final:** Aumentar a retenção diária de usuários em 20% no próximo trimestre através da introdução de mecânicas de gamificação.
- **Público-Alvo:** Jovens adultos (18-30 anos) que aprendem por conta própria e são motivados por competição e recompensas visuais.
- **Stack Tecnológica (Resumida):** Frontend em React Native, Backend em Node.js com PostgreSQL.

# TAREFA DETALHADA
- **Ação Principal:** Desenvolva um plano técnico e de produto para a feature "Sistema de Conquistas" no LinguaBoost.
- **Passos a Seguir:**
    1.  **Brainstorm de Mecânicas:** Sugira 3 mecânicas de gamificação centrais (ex: "Ofensiva Diária", "Conquistas por Nível", "Pontos de Experiência - XP"). Descreva brevemente como cada uma funcionaria.
    2.  **Esboço Técnico:** Descreva a arquitetura necessária. Especifique os modelos de banco de dados (tabelas e colunas) para `users`, `achievements`, `user_achievements`. Liste os principais endpoints de API necessários (ex: `POST /api/lessons/complete`, `GET /api/users/:id/profile`).
    3.  **Plano de Fases (Rollout):** Proponha um plano de implementação em duas fases. Fase 1 (MVP) com as funcionalidades essenciais e Fase 2 com as melhorias (ex: leaderboards, compartilhamento social das conquistas).

# FORMATO DA SAÍDA
- **Estrutura:** Use Markdown. Organize a resposta em três seções claras: "1. Mecânicas de Gamificação", "2. Esboço da Arquitetura Técnica" e "3. Plano de Implementação em Fases".
- **Elementos Obrigatórios:** Dentro do esboço técnico, use blocos de código para exemplificar a estrutura das tabelas do banco de dados.

# RESTRIÇÕES E DIRETRIZES
- **O que Evitar:** Não sugira tecnologias fora da nossa stack atual. Foque em uma implementação que seja eficiente e escalável.

### Análise das Técnicas Aplicadas
**Persona Híbrida:** Define que a IA deve pensar tanto no valor para o usuário (Produto) quanto na viabilidade técnica (Engenharia), resultando em um plano mais completo.

**Contexto Detalhado:** Informar a stack tecnológica e o objetivo de negócio (aumentar retenção em 20%) direciona a IA para soluções realistas e alinhadas à estratégia.

**Tarefa Passo a Passo:** Quebrar a solicitação em "Mecânicas", "Técnica" e "Fases" organiza o raciocínio da IA e garante que todas as áreas do planejamento sejam cobertas.

**Formato Específico:** Pedir a resposta em seções e com blocos de código torna o resultado imediatamente útil para a equipe de desenvolvimento, servindo como um documento inicial de planejamento.

## Exemplo 2: Escolha de Tecnologia

### Cenário
Uma startup está iniciando um novo produto SaaS e precisa decidir qual framework de frontend (React, Vue ou Svelte) utilizar. A decisão impactará a velocidade de desenvolvimento e a contratação de futuros talentos.

### Prompt de Exemplo
# PERFIL DA IA
- **Papel:** Você é um CTO (Chief Technology Officer) experiente, especializado em arquitetura de software para startups de alto crescimento.
- **Especialidade:** Sua análise deve ser imparcial e baseada em dados, considerando não apenas a performance técnica, mas também o impacto no negócio (custo, tempo de mercado, ecossistema).
- **Tom e Estilo:** Analítico, objetivo e conclusivo. Use uma linguagem clara e baseie suas afirmações em critérios bem definidos.

# CONTEXTO DO PROJETO
- **Produto:** Uma plataforma SaaS de dashboards de análise de dados (B2B), que exigirá alta interatividade, visualização de gráficos e atualizações em tempo real.
- **Equipe Atual:** Uma equipe pequena com 3 desenvolvedores. Um tem boa experiência com React, os outros são mais generalistas com JavaScript.
- **Prioridades do Negócio:** 1) Velocidade de desenvolvimento para lançar um MVP em 4 meses. 2) Facilidade de contratação de novos desenvolvedores no futuro. 3) Performance e escalabilidade a longo prazo.

# TAREFA DETALHADA
- **Ação Principal:** Realize uma análise comparativa entre React, Vue.js e Svelte para o nosso projeto.
- **Critérios de Análise:** Avalie os três frameworks com base nos seguintes critérios:
    1.  **Curva de Aprendizagem:** Considerando a equipe atual.
    2.  **Performance (Runtime):** Especialmente para manipulação de grandes volumes de dados no DOM.
    3.  **Ecossistema:** Disponibilidade de bibliotecas, ferramentas de desenvolvimento e suporte da comunidade.
    4.  **Pool de Talentos:** Facilidade para contratar desenvolvedores no mercado brasileiro.
    5.  **Escalabilidade e Manutenção:** Como cada framework se comporta em projetos de grande porte.

# FORMATO DA SAÍDA
- **Estrutura:**
    1.  Crie uma tabela comparativa em Markdown que resume a análise para cada framework e critério, com uma nota de 1 a 5 para cada item.
    2.  Após a tabela, escreva um parágrafo de análise para cada framework, detalhando os prós e contras no nosso contexto.
    3.  Finalize com uma seção chamada "Recomendação Final", indicando a escolha mais estratégica e justificando-a com base nas prioridades do negócio.

# RESTRIÇÕES E DIRETRIZES
- **O que Evitar:** Não baseie a recomendação apenas em preferência pessoal ou hype. A decisão deve ser estritamente fundamentada nos critérios e no contexto fornecido.

### Análise das Técnicas Aplicadas
**Persona de CTO:** Garante uma visão estratégica que equilibra fatores técnicos com necessidades de negócio (contratação, velocidade).

**Critérios Explícitos:** Forçar a análise em dimensões específicas (performance, ecossistema, etc.) evita uma resposta genérica e foca no que realmente importa para a decisão.

**Formato de Tabela + Recomendação:** A tabela oferece uma visão rápida e comparável, enquanto a recomendação final força a IA a sintetizar os dados e tomar uma posição justificada, que é o objetivo da tarefa.

**Contexto da Equipe:** Mencionar a experiência prévia da equipe é um dado crucial que a IA usará para ponderar a "Curva de Aprendizagem".

## Exemplo 3: Pesquisa de Mercado

### Cenário
O dono de uma cafeteria local quer validar a ideia de lançar uma nova linha de bebidas veganas e precisa entender o mercado, a concorrência e o público-alvo.

### Prompt de Exemplo
# PERFIL DA IA
- **Papel:** Você é um Analista de Pesquisa de Mercado especializado no setor de Alimentos e Bebidas (A&B) no Brasil.
- **Especialidade:** Análise de tendências de consumo, comportamento do consumidor e cenário competitivo para pequenos e médios negócios.
- **Tom e Estilo:** Informativo, analítico e orientado a dados. Apresente os insights de forma clara e acionável.

# CONTEXTO DO PROJETO
- **Negócio:** "Café Aconchego", uma cafeteria de pequeno porte localizada em Uberlândia, Minas Gerais.
- **Objetivo da Pesquisa:** Avaliar a viabilidade e o potencial de mercado para uma nova linha de bebidas funcionais e veganas (lattes com leites vegetais, smoothies, etc.).
- **Público-Alvo Potencial:** Consumidores preocupados com a saúde, veganos, vegetarianos e intolerantes à lactose.
- **Localização:** Foco no mercado específico de Uberlândia.

# TAREFA DETALHADA
- **Ação Principal:** Conduza uma análise de mercado concisa sobre o nicho de bebidas veganas em Uberlândia.
- **Passos a Seguir:**
    1.  **Tendências de Consumo:** Identifique as principais tendências de consumo relacionadas a veganismo e alimentação saudável no Brasil que impactam o setor de cafeterias.
    2.  **Análise Competitiva:** Identifique 2-3 potenciais concorrentes diretos ou indiretos em Uberlândia (outras cafeterias ou lojas de produtos naturais) que já oferecem produtos similares. Descreva seus pontos fortes e fracos.
    3.  **Sugestão de Mix de Produtos:** Com base na análise, sugira um cardápio inicial com 4 ideias de bebidas veganas, incluindo uma breve descrição atrativa para cada uma.
    4.  **Estratégia de Preços:** Proponha uma faixa de preço para essas bebidas, considerando os custos de insumos (leites vegetais, superfoods) e o posicionamento de mercado.

# FORMATO DA SAÍDA
- **Estrutura:** Organize a resposta como um relatório sumário em Markdown, com seções numeradas correspondendo aos passos da tarefa.
- **Elementos Obrigatórios:** Na análise competitiva, crie uma pequena tabela para comparar os concorrentes.

# RESTRIÇÕES E DIRETRIZES
- **O que Evitar:** Não forneça dados genéricos globais. A análise deve ser o mais localizada possível para o Brasil e, idealmente, para a cidade de Uberlândia.

### Análise das Técnicas Aplicadas
**Localização Específica:** Mencionar "Uberlândia, Minas Gerais" força a IA a buscar ou inferir informações locais, tornando a pesquisa infinitamente mais relevante do que uma análise genérica.

**Persona de Analista de Mercado:** Garante que a resposta use uma linguagem de negócios e se baseie em conceitos de marketing (tendências, concorrência, mix de produtos).

**Tarefa Orientada à Ação:** O prompt não pede apenas "informações", mas sim um "relatório acionável" que inclui sugestões de produtos e preços, que é o que o dono do café realmente precisa.

**Restrição de Localização:** Reforçar para evitar dados globais foca a IA na informação mais valiosa para o usuário.

## Exemplo 4: Pesquisa de Fato Histórico

### Cenário
Um estudante do ensino médio precisa escrever um trabalho sobre as causas da Inconfidência Mineira e quer uma fonte de informação confiável e bem estruturada.

### Prompt de Exemplo
# PERFIL DA IA
- **Papel:** Você é um Professor e Historiador de uma universidade brasileira, especialista em Brasil Colônia.
- **Especialidade:** Sua paixão é explicar eventos históricos complexos de forma clara, didática e envolvente para jovens estudantes.
- **Tom e Estilo:** Didático, claro e estruturado. Evite academicismos excessivos, mas mantenha a precisão histórica.

# CONTEXTO DO PROJETO
- **Usuário:** Um estudante do Ensino Médio.
- **Objetivo:** Entender as causas e os principais atores da Inconfidência Mineira para escrever um trabalho escolar de aproximadamente 1000 palavras.
- **Nível de Profundidade:** A explicação deve ser detalhada, mas acessível para alguém que não é especialista no assunto.

# TAREFA DETALHADA
- **Ação Principal:** Elabore uma explicação completa sobre as causas da Inconfidência Mineira (1789).
- **Passos a Seguir:**
    1.  **Contexto Geral:** Inicie com um parágrafo contextualizando a situação da capitania de Minas Gerais no final do século XVIII (declínio da produção de ouro, alta carga tributária da Coroa Portuguesa).
    2.  **Causas do Movimento:** Organize as causas em três categorias distintas, usando bullet points para cada uma:
        * **Causas Econômicas:** (ex: a "derrama", os impostos sobre o ouro).
        * **Causas Políticas e Sociais:** (ex: a insatisfação da elite local com o domínio português).
        * **Influências Externas (Filosóficas):** (ex: os ideais do Iluminismo e a Independência dos EUA).
    3.  **Principais Figuras:** Liste 3-4 figuras centrais do movimento (ex: Tiradentes, Cláudio Manuel da Costa) e descreva em uma frase o papel ou a motivação de cada um.

# FORMATO DA SAÍDA
- **Estrutura:** Use Markdown com títulos e subtítulos para cada seção (Contexto, Causas, Figuras). Use listas com marcadores (bullet points) para facilitar a leitura e a organização das ideias.
- **Elementos Obrigatórios:** Ao final, inclua uma seção chamada "Fontes para Aprofundamento" e sugira 2 livros ou artigos acadêmicos conhecidos sobre o tema, que possam ser usados na bibliografia do trabalho.

# RESTRIÇÕES E DIRETRIZES
- **O que Evitar:** Não use uma linguagem excessivamente complexa ou jargões de historiador. O objetivo é a clareza para um estudante. Mantenha a narrativa focada nos fatos e causas, evitando opiniões ou interpretações muito controversas sem o devido contraponto.

### Análise das Técnicas Aplicadas
**Persona Dupla (Professor/Historiador):** Garante precisão histórica (Historiador) e uma linguagem acessível (Professor).

**Contexto do Usuário:** Especificar que é para um "estudante do Ensino Médio" é a instrução mais importante, pois calibra todo o nível de complexidade da resposta.

**Formato Estruturado:** Pedir a divisão em "causas econômicas, políticas, filosóficas" força uma análise multifacetada e organizada, ideal para um trabalho escolar.

**Elemento Obrigatório (Fontes):** Solicitar fontes para aprofundamento adiciona um imenso valor acadêmico, ajudando o estudante a construir uma bibliografia sólida.

## Exemplo 5: Análise Comparativa Usando Links

### Cenário
Uma analista de marketing de conteúdo acabou de publicar um artigo no blog da empresa e quer compará-lo com o artigo de um concorrente que está bem ranqueado no Google para o mesmo tópico, a fim de encontrar oportunidades de melhoria.

### Prompt de Exemplo
# PERFIL DA IA
- **Papel:** Você é um Estrategista de Conteúdo e especialista em SEO (Search Engine Optimization) com foco em tecnologia B2B.
- **Especialidade:** Sua especialidade é analisar a estrutura, tom, profundidade e uso de palavras-chave em artigos de blog para identificar pontos fortes e fracos.
- **Tom e Estilo:** Analítico, direto e focado em recomendações práticas e acionáveis.

# CONTEXTO DO PROJETO
- **Objetivo:** Melhorar nosso artigo para superar o do concorrente nos rankings de busca do Google.
- **Foco da Análise:** Entender as diferenças de abordagem, estrutura e otimização para SEO entre os dois textos.

# FONTES DE DADOS (LINKS PARA ANÁLISE)
- **Nosso Artigo:** `https://www.nossaempresa.com/blog/guia-completo-ia-generativa`
- **Artigo do Concorrente:** `https://www.concorrentex.com/insights/o-que-e-ia-generativa-2025`

# TAREFA DETALHADA
- **Ação Principal:** Acesse e analise os dois artigos fornecidos nos links e realize uma análise comparativa detalhada.
- **Passos a Seguir:**
    1.  **Resumo e Tese Central:** Resuma em um parágrafo a tese central de cada artigo.
    2.  **Análise Comparativa em Tabela:** Crie uma tabela em Markdown comparando os dois artigos nos seguintes quesitos:
        * Estrutura do Conteúdo (Uso de H2, H3, listas)
        * Tom de Voz (Formal, casual, técnico)
        * Profundidade Técnica (Superficial, intermediário, profundo)
        * Palavras-chave Primárias e Secundárias (Identifique as principais)
        * Chamada para Ação (CTA - O que eles pedem para o leitor fazer?)
    3.  **Plano de Ação:** Com base na sua análise, liste 5 recomendações específicas e acionáveis para melhorarmos o nosso artigo.

# FORMATO DA SAÍDA
- **Estrutura:** Organize a resposta em três seções: "1. Resumos", "2. Tabela Comparativa" e "3. Recomendações de Melhoria".

# RESTRIÇÕES E DIRETRIZES
- **O que Evitar:** Não faça uma análise superficial. Quero insights detalhados sobre as diferenças estratégicas entre os dois conteúdos.

### Análise das Técnicas Aplicadas
**Instrução de Fonte Explícita:** A seção FONTES DE DADOS elimina qualquer ambiguidade sobre qual conteúdo analisar. É muito mais preciso do que pedir à IA para "encontrar" os artigos.

**Persona de Especialista em SEO:** Garante que a análise vá além de uma simples comparação de texto, focando em elementos cruciais para o ranqueamento.

**Tarefa Comparativa e Acionável:** O prompt não pede apenas para "comparar", ele estrutura a comparação em uma tabela e, o mais importante, exige um "Plano de Ação". Isso transforma a análise em valor de negócio imediato.

## Exemplo 6: Pesquisa de Mercado com Busca Profunda

### Cenário
Um consultor de investimentos precisa montar uma apresentação para seus clientes sobre o cenário atual e as perspectivas para o mercado de energia renovável no Brasil, usando os dados mais recentes disponíveis.

### Prompt de Exemplo
# PERFIL DA IA
- **Papel:** Você é um Analista de Mercado Sênior do setor de energia, com foco em energias renováveis na América Latina.
- **Especialidade:** Sua especialidade é sintetizar dados de mercado, notícias regulatórias e relatórios de investimentos em insights claros e estratégicos.
- **Tom e Estilo:** Profissional, baseado em dados e confiante.

# CONTEXTO DO PROJETO
- **Objetivo:** Criar o conteúdo para uma apresentação que explique o cenário de investimentos em energia renovável no Brasil para clientes com conhecimento intermediário do mercado financeiro.
- **Restrição Temporal:** As informações devem ser as mais atuais possíveis, focando em dados e notícias dos últimos 12 meses (de meados de 2024 até hoje).

# TAREFA DETALHADA
- **Ação Principal:** Realize uma busca aprofundada na internet para coletar e sintetizar informações atualizadas sobre o mercado de energia renovável no Brasil.
- **Tópicos de Pesquisa (Use como guia para suas buscas):**
    * `"crescimento energia solar Brasil 2024 2025"`
    * `"investimento em energia eólica Brasil leilões recentes"`
    * `"marco legal hidrogênio verde Brasil últimas notícias"`
    * `"perspectivas ANEEL para energias renováveis 2025"`
- **Síntese da Informação:** Com base na sua pesquisa, estruture a informação para uma apresentação de slides.
    1.  **Slide 1: Panorama Geral:** Crie bullet points com os principais dados de crescimento do setor (solar e eólica) no último ano.
    2.  **Slide 2: Principais Vetores de Crescimento:** Liste 3 a 4 fatores que estão impulsionando o mercado (ex: queda de custos, incentivos fiscais, demanda corporativa).
    3.  **Slide 3: Desafios e Riscos:** Identifique 3 desafios importantes (ex: infraestrutura de transmissão, instabilidade regulatória).
    4.  **Slide 4: Perspectivas Futuras:** Resuma as perspectivas para os próximos 2-3 anos, mencionando o potencial do hidrogênio verde.

# FORMATO DA SAÍDA
- **Estrutura:** Apresente a resposta como um roteiro de slides, usando títulos claros para cada "slide" (ex: `## Slide 2: Principais Vetores de Crescimento`). Use bullet points para o conteúdo de cada slide.

# RESTRIÇÕES E DIRETRIZES
- **Obrigatoriedade:** Para cada dado ou afirmação importante (ex: "o mercado solar cresceu X%"), cite a fonte (ex: "Fonte: Relatório da ABSOLAR, 2025").

### Análise das Técnicas Aplicadas
**Guia de Busca:** Fornecer "Tópicos de Pesquisa" direciona a busca da IA, aumentando a chance de encontrar informações relevantes e específicas, em vez de fazer uma busca genérica.

**Restrição Temporal:** A instrução "últimos 12 meses" é crucial para garantir a atualidade dos dados, que é o ponto principal da tarefa.

**Formato de Apresentação:** Pedir a saída em formato de "slides" torna o conteúdo imediatamente utilizável para o consultor, que pode copiar e colar em seu PowerPoint ou Google Slides.

**Citação de Fontes:** Exigir a citação de fontes é uma prática essencial para prompts de pesquisa, pois aumenta a confiabilidade e permite que o usuário verifique as informações.

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