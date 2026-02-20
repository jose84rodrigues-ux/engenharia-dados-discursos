# 📊 Projeto de Engenharia de Dados  
## Análise de Discursos Parlamentares e Votações Legislativas

---

## 🎯 Objetivo do Projeto

Construir um pipeline de dados end-to-end utilizando arquitetura Medallion (Bronze → Silver → Gold) no Databricks, integrando dados estruturados e não estruturados para geração de insights analíticos sobre discursos parlamentares e votações legislativas.

---

## 🏢 Contexto de Negócio

Uma organização de análise política necessita monitorar discursos parlamentares e votações legislativas para identificar:

- Tendências temáticas ao longo do tempo
- Relação entre discurso e comportamento de voto
- Padrões partidários
- Evolução de posicionamentos políticos

Os dados são provenientes de múltiplas fontes e não possuem padronização, exigindo um pipeline robusto de ingestão, transformação e modelagem.

---

## 📦 Fontes de Dados

### 🔹 Dados Estruturados (CSV)

- deputados.csv
- votacoes.csv

### 🔹 Dados Não Estruturados (JSON)

- discursos.json (contendo texto livre)

---

## 🏗️ Arquitetura do Pipeline

O projeto segue a arquitetura Medallion:

Fontes → Bronze → Silver → Gold → Camada Analítica

### Bronze
Ingestão bruta dos dados com metadados e controle de governança.

### Silver
Limpeza, padronização, normalização e enriquecimento dos dados.

### Gold
Modelagem analítica com tabelas otimizadas para consumo e visualização.

---

## 🛡️ Qualidade e Governança

Regras implementadas:

- Campos obrigatórios
- Datas válidas
- Mínimo de tokens nos discursos
- Controle de ingestão
- Particionamento estratégico
- Registro em catálogo

---

## 📂 Estrutura do Projeto

engenharia-dados-discursos/
│
├── notebooks/ # Scripts e notebooks do pipeline
├── data_sample/ # Dados fictícios
├── docs/ # Documentação técnica
└── src/ # Scripts auxiliares


---

## 🛠️ Tecnologias Utilizadas

- Databricks
- Apache Spark
- Delta Lake
- Unity Catalog
- Python
- SQL

---

## 📌 Conclusão

O projeto demonstra a construção de um pipeline completo de Engenharia de Dados, aplicando boas práticas de governança, qualidade, modelagem e performance, além de gerar insights estratégicos a partir de dados estruturados e não estruturados.
