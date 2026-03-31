 📊 Data Pipeline com Databricks (ETL de Vendas)

 🚀 Visão Geral

Este projeto implementa um pipeline de dados completo utilizando o Databricks, seguindo a arquitetura **Medallion (Bronze, Silver, Gold)** para processamento e análise de dados de vendas.

Os dados são processados desde a ingestão até a camada analítica (Gold), prontos para consumo por ferramentas de BI como Power BI.



 🏗️ Arquitetura do Projeto

    text
Fonte de Dados (CSV)
        ↓
Bronze (dados brutos)
        ↓
Silver (dados limpos e tratados)
        ↓
Gold (dados agregados e analíticos)
        ↓
(Próximo passo: Power BI)




   ⚙️ Tecnologias Utilizadas

* Databricks
* PySpark
* Delta Lake
* SQL
* GitHub



   📂 Estrutura do Projeto

    text
pipeline-databricks/
│
├── notebooks/
│   ├── 01_bronze.py
│   ├── 02_silver.py
│   ├── 03_gold.py
│   └── 04_analytics.py
│
├── data/
│   └── sales_data.csv
│
├── README.md
└── requirements.txt
  



   🔹 Camadas do Pipeline

     🟤 Bronze Layer

* Ingestão dos dados brutos (CSV)
* Armazenamento em formato Delta
* Base para processamento posterior



     ⚪ Silver Layer

* Limpeza de dados
* Remoção de duplicatas
* Tratamento de valores nulos
* Conversão de tipos de dados



     🟡 Gold Layer

* Criação de tabelas analíticas
* Agregações por:

  * Categoria
  * Produto
  * Mês
* Estrutura otimizada para análise



   📊 Métricas Geradas

* Receita total
* Quantidade de vendas
* Vendas por categoria
* Vendas por produto
* Evolução mensal



   🔁 Orquestração

O pipeline pode ser automatizado com Jobs do Databricks para execução diária.



   🚧 Próximos Passos

* Integração com Power BI para visualização
* Implementação de ingestão incremental
* Uso de APIs como fonte de dados
* Monitoramento e logging do pipeline



  🧠 Aprendizados

Este projeto demonstra conhecimentos em:

* Engenharia de dados
* ETL com PySpark
* Arquitetura Medallion
* Modelagem de dados
* Processamento distribuído com Spark



   📌 Como Executar

1. Criar cluster no Databricks
2. Executar os notebooks na ordem:

   * Bronze
   * Silver
   * Gold
3. Validar as tabelas criadas



   👨‍💻 Autor

Projeto desenvolvido para fins de estudo e evolução em Engenharia de Dados.


