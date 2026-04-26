# Calculadora de Rentabilidade: Renda Fixa

Este projeto é uma ferramenta de terminal (CLI) desenvolvida em Python para simular a rentabilidade de investimentos em Renda Fixa, como CDBs e Tesouro Direto. O programa calcula o efeito dos juros compostos sobre aportes mensais e desconta o Imposto de Renda (IR) automaticamente, com base na tabela regressiva oficial do Brasil.

## 🛠️ Tecnologias Utilizadas

* **Linguagem:** Python 3.14

## 🧮 Como o Cálculo do IR foi Implementado?

A regra de negócio do Imposto de Renda na Renda Fixa no Brasil é regressiva: quanto mais tempo o dinheiro fica investido, menor a alíquota de imposto sobre o **lucro**. O algoritmo avalia o prazo da aplicação em dias (considerando 1 mês = 30 dias) e aplica o desconto apenas sobre o rendimento:

| Prazo do Investimento | Alíquota de IR |
| :--- | :--- |
| Até 180 dias (6 meses) | **22,5%** |
| De 181 a 360 dias (1 ano) | **20,0%** |
| De 361 a 720 dias (2 anos) | **17,5%** |
| Acima de 720 dias (+2 anos)| **15,0%** |

