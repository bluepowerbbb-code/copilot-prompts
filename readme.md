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

### 🔎 Agent 1 – Diagnóstico e Classificação
Responsável por:
- Conduzir entrevista estruturada (7 perguntas)
- Coletar variáveis estratégicas
- Aplicar matriz interna de decisão
- Ranqueiar 3 carreiras
- Realizar handoff estruturado

Variáveis coletadas:
- Interesses principais
- Experiência prévia
- Horas disponíveis por semana
- Preferência operacional (pessoas, dados ou código)
- Objetivo profissional
- Interesses técnicos
- Experiência reaproveitável

---

### 📅 Agent 2 – Planejamento Estratégico
Responsável por:
- Descrever o dia a dia da carreira escolhida
- Mapear habilidades essenciais e complementares
- Criar roadmap de 90 dias adaptado
- Definir projeto de portfólio
- Simular roteiro de entrevistas
- Recomendar trilha educacional

---

## 🔄 Modelo de Orquestração

Embora o sistema possua dois agentes conceituais, a execução ocorre através de um único Prompt Orquestrador.

Esse prompt mantém separação lógica interna por fases:

FASE 1 – Entrevista Estruturada  
FASE 2 – Análise com Matriz de Decisão (interna)  
FASE 3 – Escolha do Usuário  
FASE 4 – Geração do Plano Completo  

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

# 🔧 Prompt Orquestrador (Execução Unificada)

Abaixo deve ser inserido o prompt completo responsável por orquestrar os dois papéis (Agent 1 e Agent 2) dentro de um único fluxo sequencial.

Este prompt deve conter:

- Definição dos dois papéis internos
- Regras rígidas de controle de fluxo
- Entrevista com 7 perguntas (1 por vez)
- Matriz de decisão interna não exibida
- Ranking estruturado
- Handoff automático
- Geração completa do roadmap conforme template

---

📌 INSERIR AQUI O TEXTO COMPLETO DO PROMPT ORQUESTRADOR

(cole aqui o prompt final unificado contendo Agent 1 + Agent 2 em sequência lógica)

---

Observação Técnica:

Mesmo sendo executado como um único prompt, o sistema mantém:

- Separação funcional
- Controle de estado por fases
- Regras explícitas para impedir:
  - Geração prematura de plano
  - Continuação após 7 perguntas
  - Vazamento da matriz de decisão
  - Quebra de formato do roadmap

---

## 📊 Modelo de Decisão

Cada carreira é avaliada de 0 a 5 nos seguintes critérios:

- Afinidade com interesses declarados
- Demanda de mercado (contextual)
- Tempo até nível júnior (ramp-up)
- Aproveitamento de experiência prévia

Pontuação máxima: 20 pontos.

A matriz é utilizada como raciocínio interno e não é exibida ao usuário.

---

## 🧪 Teste de Execução (Caso Simulado)

### Perfil Utilizado

- Interesse: Resolver problemas  
- Experiência: Pouca  
- Tempo disponível: 1h/semana  
- Preferência: Dados  
- Objetivo: Crescer na função atual  
- Interesse técnico: Inteligência Artificial  

---

### Ranking Gerado

1º Analista de Dados — 17/20  
2º Cientista de Dados Júnior — 15/20  
3º Engenheiro de Machine Learning Júnior — 13/20  

Escolha do usuário: Engenheiro de Machine Learning Júnior

---

### Resultado Produzido

O sistema gerou:

- Plano progressivo de 20 semanas
- Estrutura de fundamentos → ML → Deep Learning → Engenharia
- Mini-projetos práticos
- Estratégia de portfólio
- Roteiro de entrevistas
- Recursos gratuitos recomendados

---

## 🧩 Decisões Arquiteturais

1. Separação lógica de agentes para modularidade  
2. Orquestração unificada para simplicidade de execução  
3. Controle rígido de fluxo conversacional  
4. Template fechado para evitar respostas genéricas  
5. Handoff estruturado com variáveis padronizadas  

---

## ⚠️ Limitações Técnicas

- Dependência da qualidade das respostas do usuário  
- Possível variação de formatação entre modelos  
- Ausência de banco dinâmico de carreiras  
- Avaliação de mercado não regionalizada automaticamente  

---

## 🚀 Possíveis Evoluções

- Implementação de pesos dinâmicos na matriz  
- Inclusão de análise comportamental (soft skills)  
- Integração com APIs de vagas  
- Persistência de dados do usuário  
- Interface web com histórico de execução  

---

## 🎓 Competências Demonstradas

Este projeto evidencia:

- Engenharia de Prompt Avançada  
- Arquitetura Multiagente  
- Design de Sistema Conversacional  
- Modelagem de Fluxo Estruturado  
- Pensamento de Produto com IA  

---

## 📌 Conclusão

O IA Mentor de Carreira demonstra como sistemas baseados em IA generativa podem ser estruturados com arquitetura modular e orquestração interna para simular processos consultivos reais.

Mais do que um chatbot, trata-se de um sistema orientado por fases, controle e especialização funcional.
