# 🖼️ Wireframes & Decisões de UX — Clarity

> *Cada tela tem uma intenção. Este documento explica não só o que aparece, mas por que aparece daquele jeito.*

---

## Princípios de design do produto

| Princípio | Na prática |
|-----------|-----------|
| **Clareza acima de tudo** | Se o usuário precisa pensar para entender a tela, a tela está errada |
| **Objetivo sempre visível** | O objetivo de carreira aparece em todas as telas principais — é a âncora do produto |
| **Fricção mínima** | Nenhuma ação frequente deve levar mais de 30 segundos |
| **Progresso visível** | O usuário sempre sabe onde está em relação a onde quer chegar |

---

## Fluxo principal

```
[Criar conta] → [Onboarding: Objetivo] → [Onboarding: Área atual]
     → [Adicionar primeiro curso] → [Ver dashboard] → [Check-in semanal]
```

---

## Tela 1 — Onboarding: Definição de Objetivo

**O que o usuário vê:**

```
┌─────────────────────────────────────────────┐
│                                             │
│   Olá! Vamos começar pelo mais importante.  │
│                                             │
│   Qual é o seu objetivo profissional        │
│   para os próximos 12 meses?                │
│                                             │
│   ┌─────────────────────────────────────┐   │
│   │  Ex: Virar Product Manager          │   │
│   └─────────────────────────────────────┘   │
│                                             │
│   Prazo:  [ 6 meses ]  [ 12 meses ]  [ 2a ] │ 
│                                             │
│   ┌─────────────────────────────────────┐   │
│   │         Continuar →                 │   │
│   └─────────────────────────────────────┘   │
│                                             │
│   Você pode mudar isso a qualquer momento.  │
│                                             │
└─────────────────────────────────────────────┘
```

**Decisão de UX:** A tela não tem menu, logo exibido em destaque, nem botão de "pular". O objetivo é a primeira coisa. Não existe "depois" — o produto começa aqui.

A frase "Você pode mudar isso a qualquer momento" reduz ansiedade. Muitos usuários travam em definir o objetivo porque acham que é uma decisão permanente.

---

## Tela 2 — Dashboard Principal

**O que o usuário vê:**

```
┌──────────────────────────────────────────────────────┐
│  Olá, Ana 👋                          [check-in] [+] │
│                                                      │
│  ┌────────────────────────────────────────────────┐  │
│  │  🎯 Virar Product Manager em 12 meses         │   │
│  │  ████████████░░░░░░░░  42% concluído           │  │
│  │  6 meses restantes                             │  │
│  └────────────────────────────────────────────────┘  │
│                                                      │
│  Seu progresso esta semana                           │
│  ┌──────────┐  ┌──────────┐  ┌──────────┐            │
│  │ 3 cursos │  │ 8h study │  │ 4ª semana│            │
│  │ no total │  │ este mês │  │ seguida  │            │
│  └──────────┘  └──────────┘  └──────────┘            │
│                                                      │
│  Próximo passo sugerido                              │
│  ┌────────────────────────────────────────────────┐  │
│  │  📚 Métricas de produto                        │  │
│  │  Você ainda não tem cursos nessa área          │  │
│  │  e é uma das mais pedidas para PM Jr.          │  │
│  │                                    [Ver trilha]│  │
│  └────────────────────────────────────────────────┘  │
│                                                      │
└──────────────────────────────────────────────────────┘
```

**Decisão de UX:** O objetivo aparece no topo, sempre. É a âncora visual e emocional do produto. Abaixo dele, o progresso em relação ao objetivo — não em relação a cursos genéricos.

O "próximo passo sugerido" é contextual: mostra exatamente o que falta, não uma lista genérica de recomendações.

---

## Tela 3 — Check-in Semanal

**O que o usuário vê:**

```
┌─────────────────────────────────────────────┐
│                                             │
│   ✅ Check-in da semana                    │
│   Leva menos de 2 minutos.                  │
│                                             │
│   O que você estudou essa semana?          │
│   ┌─────────────────────────────────────┐  │
│   │  [ ] Nada essa semana               │  │
│   │  [ ] Assisti aulas / vídeos         │  │
│   │  [ ] Li artigos ou livros           │  │
│   │  [ ] Fiz um projeto prático         │  │
│   │  [ ] Conclui um curso               │  │
│   └─────────────────────────────────────┘  │
│                                            │
│   Como você está se sentindo em relação    │
│   ao seu desenvolvimento?                  │
│                                            │
│   😞  😐  🙂  😊  🚀                    │
│                                            │
│   ┌─────────────────────────────────────┐  │
│   │         Registrar check-in          │  │
│   └─────────────────────────────────────┘  │
│                                            │
└────────────────────────────────────────────┘
```

**Decisão de UX:** O check-in tem duas perguntas — uma funcional (o que estudou) e uma emocional (como está se sentindo). A segunda parece simples, mas é o dado mais valioso: permite identificar usuários em risco de churn antes que eles saiam.

O emoji como interface para sentimento reduz fricção: sem caixa de texto, sem reflexão longa — só um clique.

---

## Tela 4 — Trilha Personalizada

**O que o usuário vê:**

```
┌─────────────────────────────────────────────────┐
│  Sua trilha para: Virar Product Manager         │
│                                                 │
│  HABILIDADES TÉCNICAS              3/5 ▓▓▓░░    │
│  ✅ Fundamentos de produto                      │
│  ✅ Metodologias ágeis                          │
│  ✅ Análise de dados básica                     │
│  ○  Métricas de produto          ← próximo      │
│  ○  SQL para PMs                                │
│                                                 │
│  HABILIDADES COMPORTAMENTAIS       1/4 ▓░░░     │
│  ✅ Comunicação com stakeholders               │
│  ○  Priorização e tomada de decisão             │
│  ○  Gestão de conflitos                         │
│  ○  Liderança sem autoridade                    │
│                                                 │
│  CONHECIMENTO DE MERCADO           0/3 ░░░      │
│  ○  Como funciona um time de produto            │
│  ○  Discovery e pesquisa com usuários           │
│  ○  Go-to-market básico                         │
│                                                 │
└─────────────────────────────────────────────────┘
```

**Decisão de UX:** A trilha é dividida em três dimensões (técnica, comportamental, mercado) porque PM é uma função multidimensional. Mostrar só habilidades técnicas seria incompleto — e o usuário perceberia isso.

O "← próximo" ao lado da primeira tarefa incompleta remove a paralisia de escolha: o usuário sabe exatamente onde continuar.

---

## Decisões de navegação

| Decisão | Por quê |
|---------|---------|
| Objetivo visível em todas as telas | É a razão de o usuário estar no app — nunca pode sumir |
| Sem menu hambúrguer | Esconde funcionalidades. As ações principais ficam na tela principal |
| Bottom navigation com 4 itens | Início, Cursos, Trilha, Check-in — os 4 verbos do produto |
| Nenhuma tela com rolagem infinita | Contra o vício de scroll. O app é ferramenta, não rede social |

---

*[← Voltar](../README.md)*
