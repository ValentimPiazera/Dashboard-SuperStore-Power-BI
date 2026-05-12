# Dashboard SuperStore - Power BI

Dashboard analítico desenvolvido no Power BI Desktop com base no dataset **SuperStore** do Kaggle, focado em métricas de vendas, lucro e desempenho por região, segmento e categoria de produto.

---

## Arquivo

| Arquivo | Descrição |
| --- | --- |
| `dashboard_superstore.pbix` | Arquivo Power BI com modelo de dados e relatório |
| `Sample - Superstore.csv` | Base de dados original extraída do Kaggle |

## Gráficos

| Visual | Tipo | Descrição |
| --- | --- | --- |
| **Total Profit** | Cartão (KPI) | Exibe o lucro total acumulado |
| **Sold Amount of Unities** | Cartão (KPI) | Total de unidades vendidas |
| **Average Discounts Given** | Cartão (KPI) | Média de descontos aplicados nas vendas |
| **Profit by Segment** | Gráfico de Rosca | Distribuição do lucro por segmento de cliente |
| **Profit by Region** | Gráfico de Barras | Comparativo de lucro entre as regiões |
| **Profit by Sub-Category** | Mapa de Árvore (Treemap) | Lucro proporcional por sub-categoria de produto |
| **Mapa Geográfico** | Mapa | Distribuição geográfica por cidade, estado e país |

---

## Filtros (Slicers)

O dashboard conta com **5 slicers interativos** que permitem filtrar todos os visuais simultaneamente:

| Slicer | Campo |
| --- | --- |
| Estado | `State` |
| Categoria / Sub-Categoria | `Category`, `Sub-Category` |
| Modal de Envio | `Ship Mode` |
| Sub-Categoria | `Sub-Category` |
| Segmento | `Segment` |

## Dataset Utilizado

- **Fonte:** [Superstore Dataset — Kaggle](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)
- **Domínio:** Varejo / E-commerce
- **Campos principais utilizados:** `City`, `State`, `Country`, `Region`, `Category`, `Sub-Category`, `Segment`, `Ship Mode`, `Profit`, `Quantity`, `Discount`

## Como usar

1. Faça o download do arquivo `dashboard_superstore.pbix`
2. Abra no **Power BI Desktop** (versão abril/2026 ou superior recomendada)
3. Utilize os slicers no painel para filtrar por estado, categoria, segmento, modal de envio e sub-categoria
4. Os visuais serão atualizados automaticamente conforme os filtros selecionados

---
