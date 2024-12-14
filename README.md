# Projeto de Segmentação de Clientes

## Visão Geral

Este projeto foca na **Segmentação de Clientes** utilizando dados de uma campanha de marketing. O objetivo principal é agrupar clientes com base em seus comportamentos e hábitos de compra, fornecendo insights para estratégias de marketing. A análise e o agrupamento dos clientes permitem que ocorra melhor compreensão sobre os clientes e personalize seus serviços para maximizar o engajamento e a rentabilidade.

---

## Roteiro

1. [Descrição dos Dados](#descrição-dos-dados)
2. [Fluxo do Projeto](#fluxo-do-projeto)
3. [Resultados e Insights](#resultados-e-insights)
4. [Tecnologias Utilizadas](#tecnologias-utilizadas)

---

## Descrição dos Dados

O conjunto de dados contém informações sobre clientes, comportamento de compras e respostas a campanhas de marketing. Principais características incluem:

- **Demográficos**: `Year_Birth`, `Education`, `Marital_Status`
- **Comportamentais**: `Income`, `Kidhome`, `Teenhome`, `Recency`, `NumWebPurchases`, `NumCatalogPurchases`
- **Produtos**: `MntWines`, `MntFruits`...
- **Promoções**: `AcceptedCmp1` a `AcceptedCmp5`, `Response`
- **Atividade no Site**: `NumWebVisitsMonth`

---

## Fluxo do Projeto

1. **Carregamento dos Dados**: Importação e limpeza do conjunto de dados.
2. **EDA**: Visualização de padrões, identificação de outliers e tratamento de valores ausentes.
3. **Engenharia de Recursos**: Criação de novas variáveis e normalização dos gastos com produtos.
4. **Agrupamento**: Aplicação do algoritmo **K-Means** para segmentar clientes em clusters.
5. **Análise**: Interpretação de cada cluster para identificar padrões e fornecer insights.

---

## Resultados e Insights

### Perfis dos usuários

#### **Cluster 0**
- Grupo com renda moderada e alto volume de compras, especialmente na categoria de vinhos.
- Clientes mais velhos, geralmente com filhos em casa.
- Fidelizados, mas com menor ticket médio por compra.

#### **Cluster 1**
- Clientes mais jovens e com menor poder aquisitivo.
- Menos ativos e menos responsivos a promoções.
- Preferem lojas físicas e visitam frequentemente o site.

#### **Cluster 2**
- Clientes mais jovens com renda moderada.
- Grupo mais ativo, comprando frequentemente em promoções.
- Preferem lojas físicas e têm maior afinidade por produtos premium.

#### **Cluster 3**
- Clientes de alta renda com maior nível educacional.
- Maior ticket médio e alta fidelidade.
- Preferem catálogos e lojas físicas, com destaque para categorias de carnes e vinhos.

### Insights

- **Cluster 0**: Grupo valioso devido ao alto volume de compras. Estratégias devem focar na manutenção da fidelidade.
- **Cluster 1**: Necessita de atenção para evitar churn. Promoções voltadas para produtos infantis podem ser eficazes.
- **Cluster 2**: Clientes engajados que valorizam descontos. Campanhas exclusivas podem aumentar o engajamento.
- **Cluster 3**: Clientes de alto valor que preferem serviços premium. O foco deve ser na retenção e experiências personalizadas.

---

## Tecnologias Utilizadas

- **Linguagem de Programação**: Python 3.x
- **Bibliotecas**:
  - Manipulação de Dados: `pandas`, `numpy`
  - Visualização de Dados: `matplotlib`, `seaborn`
  - Machine Learning: `scikit-learn`
  - Utilitários: `pickle`
