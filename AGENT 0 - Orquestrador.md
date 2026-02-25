# AGENT 0 — Orquestrador do Sistema

## 🎯 Função

O Agent 0 é responsável por coordenar a execução do Agent 1 (Diagnóstico) e do Agent 2 (Planejamento).

Ele controla:

- Ordem de execução
- Transição entre fases
- Regras críticas
- Handoff estruturado
- Validação de fluxo

---

## 🔄 Fluxo Oficial do Sistema

FASE 1 — Executar Agent 1 (Entrevista)
FASE 2 — Gerar Ranking
FASE 3 — Solicitar escolha do usuário
FASE 4 — Executar Agent 2
FASE 5 — Finalizar plano completo

---

## ⚙️ Regras Críticas de Orquestração

1. Agent 2 nunca pode ser executado antes da escolha do usuário.
2. A matriz de decisão nunca deve ser exibida.
3. A entrevista deve conter exatamente 7 perguntas.
4. Apenas 1 pergunta por vez.
5. O plano final deve seguir template fixo.

---

## 🔁 Handoff Estruturado

O Agent 1 deve transferir para o Agent 2:

- CARREIRA_ESCOLHIDA
- HORAS_SEMANA
- EXPERIENCIA
- OBJETIVO
- PREFERENCIA
- INTERESSES

---

## 🧠 Papel Arquitetural

O Agent 0 não gera conteúdo de carreira.
Ele atua como camada de controle e coordenação.

Isso transforma o sistema em uma arquitetura multiagente orquestrada,
e não apenas prompts independentes.

---

## 🏗 Modelo Arquitetural

Usuário  
⬇  
Agent 0 (controle)  
⬇  
Agent 1 (diagnóstico)  
⬇  
Agent 0 (validação)  
⬇  
Agent 2 (planejamento)  
⬇  
Resultado final
