---
title: "Rastro Imagens — Site A · Vitrine"
base: "Identidade visual da Rastro Imagens (canvas 'Rastro Imagens — Identidade Visual', cópia em identidade-visual/), prancha Site-A-Vitrine.dc.html"
description: "Site de fotos de corridas, treinos, motos e carros na Serra Gaúcha. Foto em primeiro lugar, com as cores, a fonte e o logo da marca."
---

# DESIGN.md — Rastro Imagens (Vitrine)

A fonte da verdade é a identidade visual em `identidade-visual/`
(Conceito, Logos, Sistema, Textos). Este arquivo resume o que o site usa.

## Essência
"Tudo que se move deixa um rastro." A foto é a vitrine; quem chega quer achar
a própria foto, então a busca fica na capa. Slogan: **Deixe seu rastro.**

## Cores (variáveis CSS)
- `--asfalto` `#16191C` — base da marca: cabeçalho, faixa da agenda, rodapé, último evento
- `--azul` `#2F8CFF` — Azul Elétrico: botões, logo, datas da agenda, chamada para organizadores
- `--neblina` `#F7F5F0` — fundo do site e texto sobre o Asfalto
- `--concreto` `#A3A9AE` — texto de apoio sobre fundo escuro (datas, cidades)
- `--asfalto-2` `#22272B` — cartões da agenda
- Apoio: `--azul-escuro` `#0B4FB3` (links sobre claro), `--texto-2` `#4F565C`, `--linha` `#E2DED5`
- Nunca usar o Azul Elétrico em texto pequeno sobre fundo claro.

## Tipografia
- **Archivo** (Google Fonts), uma família só.
- Títulos: Archivo Expanded Black (`font-weight:900; font-stretch:125%`), sempre em CAIXA ALTA, frases curtas.
- Textos: Archivo Regular/Medium.
- Rótulos: 13px, 800, `letter-spacing:3px`, em caixa alta.

## Logo
- Opção B "R em movimento" (três R com opacidade 22% / 50% / 100% em Azul Elétrico) + "RASTRO" Black Expanded + "IMAGENS" espaçado em azul.
- Assinatura "by Bruno Ghiggi" pequena, em cinza, abaixo do nome (rodapé).
- Grafismo do rastro (três linhas que afinam) quando falta foto.

## Estrutura da página (Site A · Vitrine)
1. **Cabeçalho** Asfalto fixo: logo, Álbuns, Agenda, Para organizadores, Instagram.
2. **Capa**: foto grande do evento mais recente com miniatura, degradê escuro embaixo, "SEU MOVIMENTO DEIXOU UM RASTRO.", busca + "Achar minha foto" (azul) e filtros em pílula com contorno.
3. **Último evento**: cartão Asfalto com foto à esquerda; data · tipo em azul, nome em Black Expanded, botão "Ver fotos".
4. **Álbuns**: grade de cartões brancos (raio 12px, borda `--linha`), foto 3:2; etiquetas (data, NOVO, tipo) **abaixo da foto, nunca sobre o atleta**.
5. **Onde vou estar**: faixa Asfalto, cartões com borda superior azul de 4px e data grande em azul (4 primeiras datas + "Ver mais datas").
6. **Melhores momentos**: mosaico com as fotos dos 5 eventos mais recentes (uma grande 2×2 + quatro pequenas) e "Seguir @rastroimagens".
7. **Organiza um evento?**: bloco azul com botão escuro "Falar no WhatsApp".
8. **Rodapé** Asfalto + botão flutuante do WhatsApp.

## Regras
- Não citar as plataformas de venda (Foco Radical, Fotto) no site.
- Sem frase de "camiseta azul" na agenda.
- Botões com raio 8px; filtros em pílula.
- Respeitar `prefers-reduced-motion`; animação só no hover dos cartões e do mosaico.
