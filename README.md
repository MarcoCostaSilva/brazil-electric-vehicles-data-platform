# ⚡ Electric Vehicles Data Platform – Brazil  
# ⚡ Plataforma de Dados de Veículos Elétricos – Brasil

---

## 📌 Overview | Visão Geral

🇺🇸  
This project implements a complete Data Engineering and Analytics platform focused on the Brazilian electric and hybrid vehicle fleet. It integrates data collection, relational modeling, ETL processes, and interactive dashboards for statistical analysis and public policy insights.

The system was developed as a Scientific Initiation Project in the Bachelor’s Degree in Statistics and is based on official data from SENATRAN, made available through the Fórum VE platform.

🇧🇷  
Este projeto implementa uma plataforma completa de Engenharia e Análise de Dados voltada à frota brasileira de veículos elétricos e híbridos. Integra coleta de dados, modelagem relacional, processos de ETL e dashboards interativos para análise estatística e suporte a políticas públicas.

O sistema foi desenvolvido como Projeto de Iniciação Científica no Bacharelado em Estatística, utilizando dados oficiais do SENATRAN disponibilizados via plataforma Fórum VE.

---

## 📊 Key Statistics | Estatísticas Principais

- Total Fleet | Frota Total: **487,114 veículos**
- Manufacturers | Fabricantes: **123**
- Models | Modelos: **560**
- Market Leader | Líder de mercado: **BYD (~33.6%)**
- Strong regional concentration in Southeast and South regions

---

## 🎯 Objectives | Objetivos

### 🇺🇸 General Objective
To implement a relational MySQL database for consolidation, validation, and statistical analysis of electric vehicle data, integrated with an interactive visualization platform.

### 🇧🇷 Objetivo Geral
Implementar um banco de dados relacional em MySQL para consolidação, validação e análise estatística de dados de veículos elétricos, integrado a uma plataforma interativa de visualização.

### Specific Goals | Objetivos Específicos

- Data extraction and normalization from SENATRAN/Fórum VE
- Relational schema design with referential integrity
- ETL pipeline implementation using Python
- Development of interactive dashboards with Streamlit
- Automated export of reports (CSV, Excel, DOCX, PDF)
- Reproducible and documented analytics workflow

---

## 🏗 System Architecture | Arquitetura do Sistema

The platform follows a layered architecture:

### 1️⃣ Data Layer | Camada de Dados
MySQL relational database with normalized tables:

- `regiao`
- `estado`
- `cidade`
- `fabricante`
- `modelo`
- `tecnologia`
- `classificacao_veiculo`
- `tipo_modelo_cidade`

Referential integrity ensured via primary and foreign keys.

### 2️⃣ Processing Layer | Camada de Processamento
Python ETL scripts:

- Data extraction
- Cleaning and normalization (Pandas)
- Loading into MySQL using `mysql-connector-python`

### 3️⃣ Presentation Layer | Camada de Apresentação
Interactive dashboards built with:

- Streamlit
- Plotly
- Pandas aggregations
- Parameterized SQL queries

---

## 🔎 Analytical Dimensions | Dimensões Analíticas

The platform supports analysis across:

- Spatial distribution (Region / State / City)
- Technology types (BEV, PHEV, HEV, FCEV, MHEV)
- Temporal evolution (since 1973)
- Market structure (Manufacturers and Models)
- Fleet growth patterns

---

## 🌎 Public Policy Alignment | Alinhamento com Políticas Públicas

This project supports data-driven decision-making aligned with:

- UN SDGs (7, 9, 11, 12, 13)
- Rota 2030 Program
- PNME (National Electric Mobility Policy)
- PNE 2050 (National Energy Plan)

---

## 📂 Project Structure | Estrutura do Projeto

```
banco-veiculos-eletricos/
│
├── veiculos/                 # ETL and data processing scripts
├── dashboard_streamlit.py    # Main Streamlit application
├── requirements.txt
├── docs/
│   └── er_diagram.png        # Entity-Relationship diagram
└── README.md
```

---

## 🛠 Technologies Used | Tecnologias Utilizadas

- Python  
- Pandas  
- MySQL  
- SQL (Normalized Relational Modeling)  
- Streamlit  
- Plotly  
- OpenPyXL  
- FPDF  
- GeoPandas  
- Folium  

---

## 🚀 How to Run | Como Executar

### 1️⃣ Clone repository

```bash
git clone https://github.com/MarcoCostaSilva/banco-veiculos-eletricos.git
cd banco-veiculos-eletricos
```

### 2️⃣ Install dependencies

```bash
pip install -r requirements.txt
```

### 3️⃣ Configure database connection

Create a `.streamlit/secrets.toml` file with:

```
[database]
host = "your_host"
user = "your_user"
password = "your_password"
database = "your_database"
```

### 4️⃣ Run Streamlit app

```bash
streamlit run dashboard_streamlit.py
```

---

## 📈 Analytical Outputs | Resultados Analíticos

- Regional concentration analysis
- Technology adoption trends
- Market share evolution
- Interactive filtering by region, state, city, model, technology
- Exportable analytical reports

---

## 📌 Future Improvements | Melhorias Futuras

- Automated API integration
- Cloud database optimization
- Performance indexing strategies
- Predictive modeling of fleet growth
- Geographic clustering analysis
- Deployment on scalable cloud infrastructure

---

## 🧩 Skills Demonstrated | Competências Demonstradas

✔ Relational Database Modeling  
✔ Data Engineering (ETL)  
✔ SQL Optimization  
✔ Dashboard Development  
✔ Public Policy Data Analysis  
✔ Statistical Interpretation  
✔ Data Visualization  

---

## 👤 Author | Autor

Marco Aurélio Costa da Silva  
Data Scientist | Data-Oriented Full Stack Developer | Statistical Modeling  

GitHub: https://github.com/MarcoCostaSilva  
LinkedIn: https://linkedin.com/in/marco-costadasilva  
Academic CV (Lattes Platform – Brazil): https://lattes.cnpq.br/8887305754672433
