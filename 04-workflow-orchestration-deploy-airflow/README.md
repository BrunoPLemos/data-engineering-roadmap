# Workflow Orchestration e Deploy com Airflow

## 📋 Sobre

Este módulo ensina **orquestração de workflows de dados** usando Apache Airflow, desde conceitos básicos até deploy em produção. Você aprenderá a criar, agendar e monitorar pipelines de dados complexos.

**Objetivo Educacional**: Dominar Apache Airflow para orquestração de pipelines de dados, incluindo criação de DAGs, operadores, sensores e deploy em ambientes cloud.

## 🎯 Objetivos de Aprendizado

- **Apache Airflow**: Entender arquitetura e conceitos fundamentais
- **DAGs (Directed Acyclic Graphs)**: Criar workflows de dados
- **Operadores**: Usar diferentes tipos de operadores (Python, SQL, Bash)
- **Sensores**: Aguardar condições antes de executar tarefas
- **XComs**: Compartilhar dados entre tarefas
- **Deploy**: Fazer deploy de Airflow em produção (AWS, GCP, Azure)
- **Monitoramento**: Usar UI do Airflow para monitorar execuções

## 📁 Estrutura do Módulo

```
04-workflow-orchestration-deploy-airflow/
├── exemplo_00.py              # Introdução básica ao Airflow
├── exemplo_01.py              # Primeiro DAG simples
├── exemplo_02/                # DAGs com dependências
├── exemplo_03/                # Operadores Python
├── exemplo_04/                # Operadores SQL
├── exemplo_05/                # Sensores e condições
├── exemplo_06/                # DAGs complexos
├── exemplo_07/                # Deploy e produção
├── pic/                       # Diagramas e imagens
└── README.md                  # Este arquivo
```

## 🛠️ Tecnologias e Ferramentas

- **Apache Airflow**: Plataforma de orquestração de workflows
- **Python**: Linguagem para criar DAGs
- **Docker**: Containerização do Airflow
- **PostgreSQL**: Banco de metadados do Airflow
- **Cloud Services**: AWS, GCP, Azure para deploy

## 📦 Pré-requisitos

- Python 3.8+ instalado
- Docker e Docker Compose (para exemplos com containers)
- Conhecimento básico de Python
- Conhecimento básico de SQL

## 🚀 Como Usar

### Instalação Local

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/lvgalvao/data-engineering-roadmap.git
   cd data-engineering-roadmap/04-workflow-orchestration-deploy-airflow
   ```

2. **Instale o Airflow**:
   ```bash
   pip install apache-airflow
   ```

3. **Inicialize o Airflow**:
   ```bash
   airflow db init
   airflow users create \
     --username admin \
     --firstname Admin \
     --lastname User \
     --role Admin \
     --email admin@example.com
   ```

4. **Inicie o webserver e scheduler**:
   ```bash
   # Terminal 1
   airflow webserver --port 8080
   
   # Terminal 2
   airflow scheduler
   ```

5. **Acesse a UI**: http://localhost:8080

### Execução dos Exemplos

Cada exemplo pode ser executado independentemente:

```bash
# Exemplo básico
python exemplo_00.py

# Exemplo com DAG
python exemplo_01.py
```

## 📚 Conteúdo das Aulas

### Exemplo 00: Introdução
- Conceitos básicos do Airflow
- Estrutura de um DAG
- Primeiros passos

### Exemplo 01: DAG Simples
- Criar primeiro DAG
- Executar tarefas básicas
- Entender execução

### Exemplo 02: Dependências
- Definir dependências entre tarefas
- Usar `>>` e `<<` operators
- Execução paralela

### Exemplo 03: Operadores Python
- PythonOperator
- Executar funções Python
- Passar parâmetros

### Exemplo 04: Operadores SQL
- SQLOperator
- Executar queries SQL
- Conexões com bancos

### Exemplo 05: Sensores
- FileSensor
- TimeSensor
- Condições de execução

### Exemplo 06: DAGs Complexos
- Múltiplas dependências
- Branching
- Error handling

### Exemplo 07: Deploy
- Deploy em cloud
- Configuração de produção
- Monitoramento

## 🔗 Conexões com a Formação

- **Pré-requisitos**: 
  - Projeto 01 (Data Project Foundations) para entender pipelines
  - Conhecimento de Python e SQL
- **Próximos passos**: 
  - Projeto 08 (Databricks) para orquestração em cloud
  - Módulo de Cloud AWS em `06-cloud-aws-para-dados/`

## 📖 Recursos Adicionais

- [Documentação do Airflow](https://airflow.apache.org/docs/)
- [Tutoriais do Airflow](https://airflow.apache.org/docs/apache-airflow/stable/tutorial/index.html)
- [Best Practices do Airflow](https://airflow.apache.org/docs/apache-airflow/stable/best-practices.html)

## 👤 Autor

**Luciano Filho** - [lvgalvaofilho@gmail.com](mailto:lvgalvaofilho@gmail.com)

---

**Parte da Formação Profissional em Engenharia de Dados - [Jornada de Dados](https://suajornadadedados.com.br/)**

