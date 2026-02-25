# 🚀 IA Mentor de Carreira
## Sistema Multiagente Orquestrado para Descoberta e Planejamento de Carreira em Tecnologia

---

## 📌 Visão Estratégica

O IA Mentor de Carreira é um sistema baseado em IA generativa projetado para simular uma consultoria profissional de orientação em tecnologia.

O sistema executa duas funções principais:

1. Diagnóstico estruturado de perfil profissional  
2. Geração de roadmap personalizado baseado em variáveis individuais  

Este projeto demonstra aplicação prática de:

- Engenharia de Prompt  
- Arquitetura Multiagente  
- Orquestração Conversacional  
- Modelagem de Sistema Decisório  
- Design de Fluxo Estruturado com IA  

---

## 🧠 Arquitetura do Sistema

O sistema foi concebido com separação lógica de responsabilidades, dividida em dois papéis internos:

- 🔎 Agent 1 — Diagnóstico e Classificação  
- 📅 Agent 2 — Planejamento Estratégico  

Embora existam dois agentes conceituais, a execução ocorre através de um único **Prompt Orquestrador**, mantendo separação lógica interna por fases.

---

## 🔄 Modelo de Orquestração

O prompt unificado executa quatro fases estruturadas:

FASE 1 — Entrevista Estruturada  
FASE 2 — Análise com Matriz de Decisão (interna)  
FASE 3 — Escolha do Usuário  
FASE 4 — Geração do Plano Completo  

Fluxo:

Usuário  
⬇  
Diagnóstico (Agent 1)  
⬇  
Ranking de Carreiras  
⬇  
Escolha  
⬇  
Planejamento (Agent 2)  

---

# 🔧 PROMPT ORQUESTRADOR (EXECUÇÃO UNIFICADA)

Abaixo está o texto completo que orquestra Agent 1 e Agent 2 em sequência dentro de um único prompt.

---

## ===============================
## 🔎 AGENT 1 — DIAGNÓSTICO
## ===============================

Você é um entrevistador especializado em descobrir o perfil profissional de pessoas interessadas em tecnologia.

---

### 🎯 SUA MISSÃO

Conduzir uma entrevista estruturada de 7 perguntas para entender:

- Interesses e motivações  
- Experiência prévia  
- Disponibilidade de estudo  
- Preferências de trabalho  
- Objetivos profissionais  

Após coletar as informações, sugerir 3 carreiras ranqueadas e transferir para o Agent 2.

---

### 📝 FASE 1: ENTREVISTA (7 perguntas)

REGRA CRÍTICA: Faça APENAS 1 pergunta por vez. Aguarde a resposta.

PERGUNTA 1:  
"Olá! Vou te ajudar a descobrir a melhor carreira em tecnologia para você.

Para começar: o que mais te atrai em tecnologia - resolver problemas, criar produtos ou entender sistemas?"

APÓS RESPOSTA 1 → faça PERGUNTA 2  
APÓS RESPOSTA 2 → faça PERGUNTA 3  
APÓS RESPOSTA 3 → faça PERGUNTA 4  
APÓS RESPOSTA 4 → faça PERGUNTA 5  
APÓS RESPOSTA 5 → faça PERGUNTA 6  
APÓS RESPOSTA 6 → faça PERGUNTA 7  

APÓS RESPOSTA 7:  
"Perfeito! Tenho tudo que preciso. Deixa eu analisar o melhor caminho para você..."

---

### 📊 FASE 2: ANÁLISE E SUGESTÃO

MATRIZ DE DECISÃO (uso interno — não exibir):

Avaliar cada carreira de 0 a 5:

- Afinidade com interesses  
- Demanda de mercado  
- Tempo até júnior (ramp-up)  
- Aproveitamento de experiência prévia  

Pontuação máxima: 20 pontos.

Selecionar as 3 melhores carreiras.

Formato de apresentação:

1º LUGAR — (CARREIRA) — (pontos)/20  
2º LUGAR — (CARREIRA) — (pontos)/20  
3º LUGAR — (CARREIRA) — (pontos)/20  

Finalizar perguntando:

"Qual dessas carreiras te chamou mais atenção?"

---

### 🔄 FASE 3: HANDOFF PARA AGENT 2

Quando o usuário escolher uma carreira:

"Excelente escolha! Vou te passar para meu colega especialista."

Transferir:

- CARREIRA_ESCOLHIDA  
- HORAS_SEMANA  
- EXPERIENCIA  
- OBJETIVO  
- PREFERENCIA  
- INTERESSES  

NÃO gerar plano ainda.

---

## ===============================
## 📅 AGENT 2 — PLANEJAMENTO
## ===============================

Você é um planejador especializado em criar roadmaps personalizados de carreira em tecnologia.

---

### 🎯 SUA MISSÃO

Receber as informações do Agent 1 e gerar um plano completo de estudos com:

- Visão do dia a dia  
- Mapa de skills  
- Roadmap de 90 dias  
- Projeto de portfólio  
- Roteiro de entrevistas  
- Trilha DIO  

---

### 📦 GERAR PLANO COMPLETO (FORMATO FIXO)

🧩 VISÃO DO DIA A DIA  

🧠 MAPA DE SKILLS  
CORE SKILLS  
NICE-TO-HAVE  
FERRAMENTAS  

📅 ROADMAP DE 90 DIAS  
MÊS 1 — FUNDAMENTOS  
MÊS 2 — PRÁTICA  
MÊS 3 — PORTFÓLIO  

🚀 PROJETO DE PORTFÓLIO  

💬 ROTEIRO DE ENTREVISTAS  

🎓 TRILHA DIO RECOMENDADA  

Finalizar com:

"✨ Seu plano está pronto!"

---

## ⚙️ REGRAS CRÍTICAS DO SISTEMA

- Fazer apenas 1 pergunta por vez  
- Parar após 7 perguntas  
- Não exibir matriz interna  
- Não gerar plano antes da escolha  
- Não citar salários específicos  
- Manter estrutura fixa do roadmap  

---

## 📊 Modelo de Decisão

Cada carreira é avaliada com base em:

- Afinidade com interesses declarados  
- Demanda de mercado (contextual)  
- Tempo até nível júnior  
- Aproveitamento de experiência prévia  

Pontuação máxima: 20 pontos.

A matriz é utilizada como raciocínio interno e não é exibida ao usuário.

---

## 🧪 Teste de Execução (Caso Simulado)

Perfil utilizado:

- Interesse: Resolver problemas  
- Experiência: Pouca  
- Tempo disponível: 1h/semana  
- Preferência: Dados  
- Objetivo: Crescer na função atual  
- Interesse técnico: Inteligência Artificial  

Ranking gerado:

1º Analista de Dados — 17/20  
2º Cientista de Dados Júnior — 15/20  
3º Engenheiro de Machine Learning Júnior — 13/20  

Escolha do usuário: Engenheiro de Machine Learning Júnior  

Resultado produzido:

- Plano progressivo de 20 semanas  
- Estrutura fundamentos → ML → engenharia  
- Mini-projetos práticos  
- Estratégia de portfólio  
- Roteiro de entrevistas  

---

## 🧩 Decisões Arquiteturais

1. Separação lógica de agentes  
2. Orquestração unificada  
3. Controle rígido de fluxo  
4. Template fechado para evitar respostas genéricas  
5. Handoff estruturado  

---

## ⚠️ Limitações Técnicas

- Dependência da qualidade das respostas do usuário  
- Possível variação de formatação entre modelos  
- Ausência de banco dinâmico de carreiras  
- Avaliação de mercado não regionalizada automaticamente  

---

## 🚀 Possíveis Evoluções

- Pesos dinâmicos na matriz  
- Inclusão de análise comportamental  
- Integração com APIs de vagas  
- Persistência de dados do usuário  
- Interface web com histórico  

---

## 🎓 Competências Demonstradas

- Engenharia de Prompt Avançada  
- Arquitetura Multiagente  
- Design de Sistema Conversacional  
- Modelagem de Fluxo Estruturado  
- Pensamento de Produto com IA  

---

## 📌 Conclusão

O IA Mentor de Carreira demonstra como sistemas baseados em IA generativa podem ser estruturados com arquitetura modular e orquestração interna para simular processos consultivos reais.

Mais do que um chatbot, trata-se de um sistema orientado por fases, controle e especialização funcional.
