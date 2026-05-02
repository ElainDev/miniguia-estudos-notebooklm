# Miniguia de Estudos: Observabilidade Moderna com Dynatrace & NotebookLM
## 📖 Contexto e Objetivos
Este repositório contém o projeto prático desenvolvido para o desafio da **DIO**, focado na utilização da Inteligência Artificial como ferramenta de aprendizagem ativa.
O tema escolhido foi **Observabilidade e Dynatrace**, o que venho estudando na minha Residência Tecnológica junto com mentores da Extreme Group. O objetivo deste caderno temático é consolidar conhecimentos sobre monitoramento de infraestrutura, hosts e grupos de processos, utilizando o **NotebookLM** para organizar o fluxo de informações e gerar insights técnicos baseados em documentações oficiais.

## 📚 Curadoria de Fontes
Para alimentar a inteligência do NotebookLM, foram selecionadas 4 fontes principais de alta autoridade:
- **Dynatrace Documentation (PDF):** Visão geral sobre "Host Monitoring" e "Process Groups".
- **Observability Whitepaper:** Conceitos fundamentais de Traces, Logs e Metrics.
- **DQL (Dynatrace Query Language) Guide:** Documentação técnica sobre extração de dados.
- **Artigo Técnico:** Os 3 pilares da Observalidade.

 ### Links:
- https://docs.dynatrace.com/docs
- https://www.elastic.co/explore/devops-observability/understanding-aiops-for-observability?utm_campaign=G-TXT-AMER-NA-Observability-EN-Lead_Gen-MQL-NB&utm_content=Observability&utm_source=google&utm_medium=cpc&device=c&utm_term=observability%20tools&utm_id=7018X000001yRu4QAE&gad_source=1&gad_campaignid=22934802693&gbraid=0AAAAADrDgoJ6GzmuZ54D4uHuNu4hGiSJr&gclid=CjwKCAjwwdbPBhBgEiwAxBRA4RS7bh8-96P63cZ8_lO1aQT-cTkRD0Aen3yKiHfCyeh99IoT5SxW-xoCy6AQAvD_BwE
- https://docs.dynatrace.com/docs/platform/grail/dynatrace-query-language
- https://www.elastic.co/pt/blog/3-pillars-of-observability

## 🧠 Engenharia de Prompts e "Cicatrizes" (Troubleshooting)
Nesta etapa, testei a capacidade do NotebookLM de sintetizar informações técnicas baseadas na documentação de Observabilidade.

**Prompt 1 & 2 (Conceitual):** Foquei em estabelecer a base.
- **O que aprendi:** A IA diferenciou bem que Monitoramento te diz o que está acontecendo, enquanto a Observabilidade explica o porquê.

**Prompt 3 & 4 (Aplicação Prática):** Aqui conectei com o dia a dia do Dynatrace.

- **O que aprendi:** No Prompt 3, soube explicar bem e dar exemplos (Infraestrutura, Hosts e Process Group).

**Insight do Prompt 4:** Este prompt foi o mais valioso, pois gerou um roteiro de investigação que posso usar em minhas atividades como monitora.

**Prompt 5 (DQL e Comandos):** "Faça uma tabela de comandos de DQL e para que serve."
- **Dificuldade (Cicatriz):** A IA trouxe uma tabela muito simplificada com apenas os comandos básicos e citou o termo Grail, que eu ainda não conhecia profundamente.

- **Solução/Ajuste:** Percebi que a IA tende a ser "econômica" nas respostas técnicas. Para resolver, apliquei um novo prompt pedindo especificamente por comandos de agregação, conversão de tempo e análise de strings, forçando a IA a explorar funções mais avançadas do DQL além do básico fetch.

- **Aprendizado:** Descobri que o DQL depende da arquitetura do Grail para funcionar e que, para ter um guia completo, preciso segmentar as perguntas por tipos de funções (ex: funções de agregação vs. funções de filtragem).

**🛠️ Miniguia de Estudo (Entrega Final)**

**1. Glossário de Conceitos-Chave**
- **Observabilidade:** Capacidade de medir os estados internos de um sistema a partir dos dados que ele gera externamente (métricas, logs e traces).

- **Host:** No Dynatrace, refere-se a uma máquina física ou virtual monitorada pelo OneAgent.

- **Process Group (PG):** Um conjunto de processos que executam a mesma função em diferentes hosts (ex: um cluster de servidores web).

- **DQL (Dynatrace Query Language):** Linguagem baseada em pipeline usada para consultar dados.

**2. Guia de Prompts para Revisão Futura**
💡 Copie e cole estes prompts no seu caderno do NotebookLM para revisar os conceitos antes de apresentações ou mentorias:

- **Revisão Rápida:** "Com base nas fontes, crie um resumo de 5 pontos sobre a importância de monitorar Process Groups em vez de processos isolados."

- **Desafio Técnico:** "Gere 3 perguntas de múltipla escolha sobre a sintaxe do DQL e forneça as respostas comentadas."

- **Simulação:** "Imagine que um Host está com alto consumo de CPU. Usando as informações das fontes, crie um passo a passo de como eu deveria investigar esse problema dentro do Dynatrace, mencionando quais telas ou camadas (Hosts/Processes) devo olhar primeiro."
