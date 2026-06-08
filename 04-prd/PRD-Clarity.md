# 📄 PRD — Product Requirements Document: Clarity

> **Versão:** 1.0 · **Status:** Em revisão · **PM:** Luiza Nicacio · **Data:** Junho 2025

---

## 1. Contexto e Problema

Profissionais em desenvolvimento acumulam cursos, certificados e mentorias, mas não conseguem transformar esse aprendizado em uma trajetória de carreira com direção clara.

A pesquisa com usuários (8 entrevistas) confirmou que o problema não é falta de conteúdo, é falta de estratégia, organização e acompanhamento.

---

## 2. Objetivo do Produto

Criar uma ferramenta que conecta aprendizado com objetivos profissionais, ajudando o usuário a:
- Definir onde quer chegar na carreira
- Organizar o que já aprendeu
- Saber o que precisa aprender a seguir
- Medir se está evoluindo de verdade

---

## 3. Público-alvo

**Primário:** Profissionais em transição de carreira (ex: QA → PM, Dev → Product)  
**Secundário:** Analistas que buscam promoção em suas áreas  
**Fora do escopo inicial:** Estudantes sem experiência profissional

---

## 4. Métricas de Sucesso

| Métrica | Meta (6 meses) | Por quê importa |
|---------|---------------|-----------------|
| **North Star:** Objetivos concluídos | 2.000 objetivos concluídos/mês | Mede valor real entregue |
| Usuários ativos (MAU) | 10.000 | Tamanho da base |
| Retenção D30 | > 40% | Produto está criando hábito |
| NPS | > 50 | Satisfação e recomendação |
| Conversão free → pago | > 12% | Validação de valor percebido |

---

## 5. Escopo do MVP

### ✅ Must Have (MVP)

#### Feature 1 — Onboarding com objetivo de carreira

O usuário define onde quer chegar em 6 ou 12 meses. Este é o ponto de partida de tudo.

**Critérios de aceite:**
- [ ] Usuário pode definir um objetivo de carreira com prazo
- [ ] Objetivo pode ser editado a qualquer momento
- [ ] Onboarding completo em menos de 3 minutos

---

#### Feature 2 — Registro de cursos e certificados

O usuário centraliza tudo que já aprendeu — de qualquer plataforma.

**Critérios de aceite:**
- [ ] Usuário consegue adicionar curso com: nome, plataforma, data de conclusão e área
- [ ] Cursos ficam organizados por área e data
- [ ] Adição de curso em menos de 30 segundos

---

#### Feature 3 — Dashboard de evolução

Visão clara de onde o usuário está em relação ao objetivo.

**Critérios de aceite:**
- [ ] Dashboard exibe progresso em relação ao objetivo definido
- [ ] Mostra cursos concluídos, horas de estudo e áreas de desenvolvimento
- [ ] Atualiza em tempo real a cada novo curso registrado

---

#### Feature 4 — Trilha personalizada

Com base no objetivo e no que o usuário já sabe, o app sugere próximos passos.

**Critérios de aceite:**
- [ ] Trilha é gerada automaticamente após onboarding
- [ ] Sugestões são divididas por área (habilidades técnicas, comportamentais, conhecimento de mercado)
- [ ] Usuário pode marcar sugestões como "feitas" ou "não me interessa"

---

#### Feature 5 — Check-in semanal

Uma interação rápida toda semana para manter o usuário engajado e o app atualizado.

**Critérios de aceite:**
- [ ] Notificação toda segunda-feira às 9h (configurável)
- [ ] Check-in concluído em menos de 2 minutos
- [ ] Pergunta o que foi estudado na semana e como o usuário se sentiu em relação ao desenvolvimento

---

### 🟡 Should Have (V1.5)

| Feature | Justificativa |
|---------|--------------|
| Metas com prazo e milestone | Aumenta comprometimento e senso de progresso |
| Histórico de check-ins | Permite ao usuário ver evolução ao longo do tempo |
| Exportar cursos como lista | Facilita atualização do LinkedIn |

---

### 🔴 Won't Have no MVP

| Feature | Motivo |
|---------|--------|
| IA para recomendações | Alto custo, validar valor básico primeiro |
| Portfólio automático compartilhável | Depende de dados históricos; melhor na V2 |
| Networking com outros usuários | Fora do core do produto |
| Integração automática com Udemy/Coursera | Complexidade técnica alta; manual funciona no MVP |

---

## 6. Priorização RICE

| Feature | Reach | Impact | Confidence | Effort | Score |
|---------|-------|--------|-----------|--------|-------|
| Registro de objetivos | 1000 | 5 | 90% | 3 | **1500** |
| Dashboard de evolução | 900 | 4 | 80% | 4 | **720** |
| Trilha personalizada | 800 | 5 | 70% | 6 | **467** |
| Check-in semanal | 700 | 4 | 80% | 3 | **747** |
| IA Recomendações | 700 | 5 | 60% | 9 | **233** |

> Fórmula RICE: (Reach × Impact × Confidence) ÷ Effort

**Conclusão:** IA vai para V2. O valor principal está em registro, dashboard e check-in — que juntos criam o loop de uso do produto.

---

## 7. Requisitos Não-Funcionais

| Requisito | Critério |
|-----------|----------|
| Performance | Telas carregam em < 2 segundos |
| Disponibilidade | Uptime > 99,5% |
| Segurança | Dados isolados por usuário, autenticação obrigatória |
| Usabilidade | Usuário completa onboarding sem tutorial ou suporte |
| Mobile-first | App funciona perfeitamente em telas de 375px |

---

## 8. Premissas e Riscos

| Risco | Probabilidade | Impacto | Mitigação |
|-------|--------------|---------|-----------|
| Usuários abandonam antes de completar onboarding | Alta | Alto | Onboarding progressivo, não bloquear uso antes de completar |
| Baixa frequência de check-in | Média | Alto | Notificação + check-in em menos de 2 minutos |
| Usuários não percebem valor no primeiro acesso | Média | Alto | Mostrar exemplo de dashboard preenchido antes de criar conta |
| Concorrentes lançam feature similar | Baixa | Médio | Foco na experiência e nichos específicos |

---

*[← Voltar](../README.md) | Próximo: [User Story Mapping →](../05-user-story-mapping/user-story-map.md)*
