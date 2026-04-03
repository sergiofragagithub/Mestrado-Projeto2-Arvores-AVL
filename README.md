# Projeto 2: Comparativo de Performance entre Árvore Binária (ABB) e Árvore AVL

Este projeto foi desenvolvido para a disciplina de **Algoritmos e Programação** do Programa de Pós-Graduação em Computação Aplicada (PPGCA) da **Universidade Presbiteriana Mackenzie**.

## 🎯 Objetivo do Projeto
Analisar a eficiência de algoritmos de busca e inserção em estruturas de dados não lineares, utilizando um volume real de dados (Dataset Olist - E-commerce com ~100 mil registros).

## 🛠️ Ambiente e Tecnologias
* **Hardware:** Intel Core i7-5500U @ 2.40 GHz | 8 GB RAM.
  **Linguagem:** Python 3 (Ambiente Google Colab).
  **Estruturas:** Árvore Binária de Busca (ABB) e Árvore AVL (Auto-balanceada).

## 📊 Resultados de Performance
Os testes práticos confirmaram a eficiência da árvore balanceada para grandes datasets:

| Métrica | Árvore ABB (Simples) | Árvore AVL (Balanceada) | Ganho de Performance |
| :--- | :--- | :--- | :--- |
| **Inserção Total** | 317 ms | 306 ms | Superior (AVL) |
| **Busca (ID Final)** | 7.956 ns| 918 ns | **~8,6x mais rápida** |

![Gráfico de Performance](resultado_performance.png)

## 💡 Análise do "Pulo do Gato"
**Eficiência na Inserção:** A AVL foi mais rápida (306 ms) porque a árvore mantida em menor altura agiliza a localização do ponto de inserção, compensando o custo das rotações.
**Previsibilidade:** Enquanto a ABB demonstra sinais de degeneração (tendendo a O(n)), a AVL garante a complexidade logarítmica O(log n) e mantém o sistema escalável.
**Índice Secundário:** Implementação de uma segunda árvore AVL indexada pelo campo `price`, permitindo buscas instantâneas por critérios multidimensionais.

🎓 Autoria e Orientação

Autor: Sérgio Guedes Fraga

Mestrando em Computação Aplicada - Universidade Presbiteriana Mackenzie

Orientadora: Profa. Dra. Valéria Farinazzo Martins 

Instituição: Universidade Presbiteriana Mackenzie 

Disciplina: Algoritmos e Programação


