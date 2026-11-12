---
title: "Rastro Imagens — Esportivo"
base: "Análise de design da Nike na coleção VoltAgent/awesome-design-md (https://github.com/VoltAgent/awesome-design-md/tree/main/design-md/nike) — só o estilo, sem marca, logo ou fontes da Nike"
description: "Site de fotos de eventos (corridas, treinos, motos, carros) onde a foto fala e a interface fica quieta: preto, branco, um cinza e o azul da marca."
---

# DESIGN.md — Rastro Imagens (esportivo)

## Essência
A foto é o protagonista; a interface é neutra. Capa com foto grande e título
condensado gigante em maiúsculas; o resto (menu, filtros, botões, cartões) é
preto, branco e cinza claro, com botões em forma de pílula.
O objetivo é prático: achar o evento e clicar em **Ver fotos**.

## Paleta (variáveis CSS)
- `--tinta`: `#111111` — texto, botão principal, faixa da agenda, filtro ativo
- `--branco`: `#FFFFFF` — fundo da página, texto sobre preto
- `--nuvem`: `#F4F5F6` — barra de utilidade, campo de busca, blocos "como achar"
- `--grafite`: `#3A3B3D` — hover do botão preto, fios na faixa preta
- `--cinza`: `#707274` — tipo e data dos álbuns, rodapé
- `--cinza-claro`: `#B5B6B8` — texto secundário sobre preto
- `--fio`: `#D6D7D9` — contorno dos filtros e linha do rodapé
- `--azul`: `#2F8CFF` — o único acento: "Novo", "Próximo" e foco do teclado

Nada de laranja, degradê decorativo ou sombra. Cor só nas fotos.

## Tipografia (Google Fonts)
- **Display**: Archivo condensado (`font-stretch:62%`), peso 900, MAIÚSCULAS.
  Capa 56–148px / 0.86; "Onde vou estar" 56–112px; números dos passos 64px.
- **Títulos de seção**: Archivo 600, 28px.
- **Interface e texto**: Inter 400/500/600, 12–18px.

## Espaço e grid
- Largura máxima 1440px; margem lateral mínima de 16px.
- Seções com 48px de respiro; faixa preta com 56–72px.
- Álbuns em grade de 3 colunas (2 até 900px), espaço de 12px entre colunas e 40px entre linhas.

## Componentes
- **Barra de utilidade** (cinza, 36px): frase do site + Instagram e WhatsApp.
- **Menu** (60px, fixo no topo): marca "RASTRO IMAGENS" condensada, links, busca em pílula cinza à direita (no celular vai para a linha de baixo).
- **Capa**: foto do evento mais recente que tiver miniatura, com degradê escuro embaixo; título "SEU MOVIMENTO DEIXOU UM RASTRO.", linha "Último evento: … · data" e botões pílula "Ver fotos" (branco) e "Próximos eventos" (contorno).
- **Filtros**: pílulas com contorno; a ativa fica preta.
- **Álbum**: a foto é o cartão (sem borda, sem raio, sem sombra, 4:3). Abaixo: tipo (com "Novo ·" em azul), nome em negrito, data, "Ver fotos" sublinhado. Hover amplia a foto 4%.
- **Sem foto**: bloco preto com o grafismo do rastro em branco.
- **Agenda**: faixa preta; título gigante à esquerda, lista à direita com dia grande, nome, cidade/largada e etiqueta pílula ("Próximo" em azul).
- **Como achar sua foto**: 3 blocos cinza numerados (é uma sequência real).
- **Rodapé**: marca, "by Bruno Ghiggi", botões pretos Instagram e WhatsApp.

## Movimento
- Só o zoom leve da foto no hover e a troca de cor dos botões (150ms).
- Respeitar `prefers-reduced-motion`.

## Evitar
- Texto sobre a foto fora da capa (etiquetas não cobrem o atleta).
- Mais de uma cor de acento; cantos arredondados em cartões de foto.
- Carrossel automático, vídeo na capa, emoji.
- Logo, nome ou fontes da Nike — o modelo é só referência de estilo.
