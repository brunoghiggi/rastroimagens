---
title: "Rastro Imagens — Editorial de revista"
base: "Magazine Case-Study Portfolio (https://theaicareerlab.com/design-md/portfolio-case-study-magazine)"
description: "Site de fotos de eventos (corridas, treinos, motos, carros) com cara de revista impressa: papel, tinta, um único azul editorial, fotos grandes e legendas reais."
---

# DESIGN.md — Rastro Imagens

Adaptado do modelo "Magazine Case-Study Portfolio". Cada evento é tratado como uma
matéria de revista: chapéu (kicker), título forte em serifa, linha fina (dek) e uma
foto grande. A pessoa deve sentir que está folheando uma revista de esporte, não
rolando uma grade de miniaturas.

## Essência
- A foto é o design. Nada cobre o atleta: etiquetas e textos ficam fora da imagem.
- Texto factual, sem linguagem de marketing.
- O objetivo continua prático: achar o evento e clicar em **Ver fotos**.

## Paleta (variáveis CSS)
- `--papel`: `#F1ECE2` — fundo da página (papel de jornal quente)
- `--papel-frio`: `#E8E5DE` — fundo de seções alternadas
- `--tinta`: `#161513` — texto principal e blocos sem foto
- `--tinta-media`: `#5C5752` — legendas, linha fina, metadados
- `--fio`: `#221F1B` — fios (hairlines) e réguas
- `--acento`: `#1F3A8A` — o único azul: links, sublinhados, "Novo", aspas
- `--acento-suave`: `#D8DEEE` — destaque raro (realce de bloco)

Um só acento. Sem laranja, sem verde, sem segunda cor.

## Tipografia (Google Fonts)
- **Display** (títulos): Playfair Display, pesos 400/700 (+ itálico).
- **Texto**: Source Serif 4, 18–19px, peso 400.
- **Utilitária** (menu, chapéus, legendas, botões de filtro): Inter, só em tamanhos pequenos.

Escala:
- Título de capa (H1): até 96px / 0.98, 700, letter-spacing -0.03em
- Título de seção (H2): 44 / 50, 400 itálico
- Título de evento (H3): 26–40px, 700
- Linha fina: 22–28px, 400 itálico, `--tinta-media`
- Texto: 19 / 32
- Legenda / chapéu: 12–13px, Inter, MAIÚSCULAS, letter-spacing 0.08em, `--tinta-media`

Hierarquia: todo evento abre com chapéu ("CORRIDA · 03 OUT 2026"), depois título, depois linha fina.

## Espaço e grid
- Grid de 12 colunas a partir de 1024px; texto corrido com no máximo ~640px.
- Celular: coluna única, 20–24px de margem lateral.
- Ritmo vertical de 8px; 96–120px entre seções grandes.
- Fios de 1px em `--fio` separam os itens da lista de álbuns.

## Componentes
- **Menu**: barra de 56px, marca à esquerda em Playfair, links à direita em Inter maiúsculo. Sem menu hambúrguer — os links quebram linha.
- **Capa**: chapéu, título grande, linha fina, campo de busca sublinhado (sem caixa), filtros como texto maiúsculo com sublinhado azul no ativo.
- **Último evento**: foto larga (sangrada na grade), legenda abaixo, título e link "Ver fotos →".
- **Lista de álbuns**: lista vertical, NÃO grade. Cada item: texto à esquerda (chapéu, título, linha fina, link) e foto à direita; no celular empilha com a foto primeiro. Hover: foto amplia 2%, título ganha sublinhado azul.
- **Sem foto**: bloco em `--tinta` com o grafismo do rastro em cor de papel.
- **Agenda**: lista com a data em Playfair grande à esquerda e fio acima de cada item.
- **Como achar sua foto**: passos numerados com numeral em Playfair itálico azul.
- **Botões**: só texto com sublinhado `--acento`; a ação principal "Ver fotos →" em serifa itálica com seta que anda no hover.

## Movimento
- Curva `cubic-bezier(0.4, 0, 0.2, 1)`; 200ms em links/hover; 800ms para revelar imagens ao rolar.
- Sem parallax, sem carrossel automático, sem cursor animado.
- Respeitar `prefers-reduced-motion`.

## Evitar
- Grade de miniaturas como índice principal.
- Vídeo na capa, carrossel automático.
- Modo escuro (a estética é de papel).
- Emoji e selos de terceiros.
- Mais de uma cor de acento.
- Ícones dentro do conteúdo (setas de 1px são permitidas).
