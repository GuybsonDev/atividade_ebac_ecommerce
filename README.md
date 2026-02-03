# EDA — Olist (Ecommerce)

Este repositório contém a Análise Exploratória de Dados (EDA) do dataset Olist, utilizando **MySQL local**.

## Conteúdo principal
- Notebook: `ecommerce.ipynb`
- Dados (CSV): pasta `base_ecommerce/`
- Scripts auxiliares: `load_ecommerce.sql`, `fix_translation_col.sql`

## Escopo da análise
A análise cobre:
- Limpeza e preparação dos dados (padronização de datas/numéricos e tratamento de ausentes)
- Criação de colunas derivadas (ex.: tempo de entrega, atraso, valor por pedido)
- EDA com consultas SQL e visualizações
- Recomendações de gráficos e KPIs para dashboard
- Conclusão alinhada ao dashboard do Looker Studio

## Requisitos atendidos
- Cruzamento de múltiplas tabelas (orders, items, payments, customers, products)
- Uso de tabela com datas (orders)
- Tabelas com >5 colunas e >100 linhas
- Pelo menos 5 análises exploratórias distintas
- Visualizações diversas (barras, linha, histograma, dispersão, boxplot)

## Principais tabelas usadas
- `olist_orders_dataset`
- `olist_order_items_dataset`
- `olist_order_payments_dataset`
- `olist_customers_dataset`
- `olist_products_dataset`

## Execução do notebook
1) Ative o ambiente virtual:
   ```bash
   source .venv/bin/activate
   ```
2) Crie o banco de dados MYSQL:

3) Abra e execute `ecommerce.ipynb`.

## KPIs
- Receita total: 14.251.959,96
- Tempo médio de entrega: 12 dias
- Ticket médio: 98.666
- Pedidos totais: 99.441

## Observações
- O notebook usa consultas SQL diretamente no MySQL.
- As views foram usadas apenas no notebook para padronização. Caso não use views, é possível reproduzir as métricas com SQL direto nas tabelas.
