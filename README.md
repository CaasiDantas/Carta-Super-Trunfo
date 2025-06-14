# 🃏 Super Trunfo - Cidades Fictícias

Este projeto é uma implementação do clássico jogo **Super Trunfo** em linguagem C, adaptado para o contexto de **cidades fictícias**. Cada carta representa uma cidade com dados estatísticos e socioeconômicos, permitindo comparações entre atributos estratégicos para definir uma vencedora.

---

## 🔍 Visão Geral

O sistema funciona totalmente em ambiente de terminal, oferecendo um menu interativo para:

- 📋 **Visualizar todas as cartas disponíveis**, com exibição dos atributos calculados;
- ✏️ **Alterar os valores de uma carta específica**, como população, área, PIB e pontos turísticos;
- ⚔️ **Comparar duas cartas**, em modo simples ou avançado, com base em atributos selecionados;
- 📘 **Visualizar as regras básicas** do jogo.

---

## 🧩 Estrutura das Cartas

Cada carta armazena os seguintes atributos:

- `codigo` — Identificador da cidade fictícia (ex: A01, B02)
- `populacao` — Número de habitantes
- `area` — Extensão territorial em km²
- `pib` — Produto Interno Bruto (em bilhões de dólares)
- `pontos_turisticos` — Quantidade de pontos turísticos

A partir desses dados, o sistema calcula automaticamente:

- `densidade_populacional` — População / Área
- `pib_per_capita` — PIB / População
- `super_poder` — Soma ponderada de todos os atributos, usada como fator de comparação geral

---

## ⚙️ Funcionalidades do Código

### 📇 Cadastro e Cálculo

- As cartas são pré-definidas com valores fictícios representando diferentes regiões.
- Ao serem exibidas ou modificadas, seus atributos derivados são recalculados automaticamente.

### 🔁 Edição Dinâmica

- Permite modificar qualquer valor base da carta escolhida, facilitando testes e simulações.

### 🆚 Comparação entre Cartas

#### Comparação Simples
- O usuário seleciona um único atributo para confronto direto entre duas cartas.

#### Comparação Avançada
- Permite a seleção de **dois atributos diferentes** para avaliar uma "soma ponderada", dando mais profundidade estratégica à comparação.

---

## 📌 Objetivo Educacional

Este projeto é ideal para fins didáticos, como:

- Prática com **estruturas em C**
- Uso de **funções**, **vetores de structs** e **entrada/saída formatada**
- Exercício de **lógica condicional**, **loops**, e **interação via console**

---

## 📚 Regras Resumidas

- A carta com maior valor no atributo escolhido vence.
- A exceção é a densidade populacional, onde o menor valor é considerado melhor.
- A opção "Super Poder" pode ser usada para simular uma avaliação global da carta.

---
