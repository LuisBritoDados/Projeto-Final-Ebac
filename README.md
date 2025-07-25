# Projeto Análise de E-Commerce da Olist Store
Este projeto foi desenvolvido como parte do curso de Formação em Análise de Dados da EBAC, com o objetivo de aplicar ferramentas como PySpark, Excel e Looker Studio na análise de um e-commerce real, utilizando dados públicos da empresa Olist.

## Etapas do Projeto

### 1. Tratamento de Dados
- Conversão de datas e valores (`timestamp`, `double`)
- Padronização de formato monetário (remover `R$`, trocar vírgulas por pontos)
- Enriquecimento com colunas de `ano`, `mês`, `hora`, `dia da semana`
- Correção de localização geográfica (`estado + ", Brasil"`)

### 2. Análise Exploratória (EDA)
- Volume total de vendas por mês, categoria e estado
- Ticket médio por categoria e por UF
- Parcelamento médio por tipo de produto
- Frequência de pedidos por hora e dia da semana
- Distribuição dos clientes por região

### 3. Análises Estatísticas
- Cálculo de **desvio padrão** do valor total por pedido
- Aplicação de **regressão linear** para investigar a relação entre preço, frete e valor final
- Identificação de **clientes recorrentes**

### 4. Exportação para Visualização
- Geração de dataset final consolidado (`df_final.csv`)
- Campos preparados para filtros no Looker (ex: `mês`, `UF`, `categoria`, `dia_semana`)
