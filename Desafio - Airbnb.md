# Airbnb Data Warehouse - Otimização de Preços

Este projeto aplica conceitos de Data Warehouse (Modelo BRMW) para analisar a variação de preços do Airbnb com base na localização e sazonalidade.

## Desafio de Negócio
Analisar como a localização geográfica e a sazonalidade influenciam o preço das diárias para permitir estratégias de precificação dinâmica.

##  Arquitetura do Modelo (Star Schema)
O projeto foi estruturado em um modelo estrela para otimizar as consultas analíticas:
- **Tabela Fato**: `fato_anuncios` (Preços, métricas e temporadas).
- **Dimensões**: `dim_localizacao`, `dim_imovel`, `dim_host`.


## Principais Insights
- Identificação de bairros com alta sensibilidade sazonal.
- Ranking de regiões com melhor custo-benefício por estação.
- Normalização de dados brutos (CSV) para um ambiente analítico íntegro.

## Como Executar
1. Execute os scripts do arquivo anexado
2. Certifique-se de importar o arquivo `listings.csv` na tabela de staging antes de rodar o processo de ETL.
