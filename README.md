# Desafio Técnico – Engenharia de Dados (SQL)

Este repositório contém a resolução dos 4 desafios propostos no teste, utilizando **SQL** executado via **pandasql (SQLite)** em um notebook (Google Colab).

## Estrutura
- `data/`: arquivos CSV do desafio
- `notebook/teste_eng_dados.ipynb`: notebook com as soluções comentadas

## Como rodar no Google Colab
1. Abra o notebook `teste_eng_dados.ipynb` no Colab
2. Faça upload dos arquivos CSV
3. Execute todas as células em ordem

## Assunções e decisões
- Em para identificar “últimos 12 meses” e “trimestre atual”, foi utilizada a **data máxima presente no dataset** (e não a data do sistema), garantindo reprodutibilidade.
- Foi aplicado `NULLIF` para evitar divisão por zero em percentuais e ticket médio.

## Conteúdo
- Desafio 1: Faturamento bruto mensal (últimos 12 meses), nº pedidos e ticket médio.
- Desafio 2: Ranking top 10 sellers por crescimento de GMV (trimestre atual vs anterior, min 50 pedidos em ambos).
- Desafio 3: Pedidos com desconto total > 40% do valor bruto (exclui cancelados).
- Desafio 4: Produtos com unidades > 1000 que nunca foram o item de maior valor unitário no pedido.
