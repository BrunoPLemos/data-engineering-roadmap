# Deploy de Aplicações de Dados

## 📋 Sobre

Este módulo fornece uma **introdução prática ao Docker** para deploy de aplicações de dados. Você aprenderá a empacotar e implantar eficientemente aplicações de dados, incluindo uma ETL em Python, um banco de dados PostgreSQL e um dashboard interativo usando Streamlit, tudo dentro de containers Docker.

**Objetivo Educacional**: Dominar Docker e Docker Compose para deploy de aplicações de dados em ambientes de desenvolvimento e produção.

## 🎯 Objetivos de Aprendizado

- **Docker**: Entender conceitos de containerização
- **Docker Compose**: Orquestrar múltiplos containers
- **Deploy de ETLs**: Containerizar pipelines de dados
- **Deploy de Bancos de Dados**: Usar PostgreSQL em containers
- **Deploy de Dashboards**: Publicar aplicações Streamlit
- **Deploy em Cloud**: Publicar aplicações em serviços cloud

![Solução](./pics/arquitetura.png)

## Cinco Motivos para Aprender Docker em Nosso Workshop

1. **Ensino do Zero**: Independentemente do seu nível de experiência prévia, vamos começar com os conceitos básicos de Docker, assegurando que todos os participantes tenham uma compreensão sólida dos fundamentos para construir sobre eles.

2. **Facilidade para Subir o Deploy**: Demonstraremos como Docker simplifica o processo de deploy de aplicações, permitindo que você foque na construção e no aprimoramento de suas aplicações, em vez de gastar tempo com configurações complexas de ambiente.

3. **Solução Versátil**: Docker é uma ferramenta poderosa que resolve uma variedade de problemas de desenvolvimento e operações, facilitando a colaboração entre equipes e melhorando a eficiência no ciclo de vida de desenvolvimento de software.

4. **Vantagens de Utilizar Docker na Cloud**: Explore como Docker se integra perfeitamente com serviços de cloud, potencializando a escalabilidade, a portabilidade e a eficiência dos recursos em ambientes de cloud computing.

5. **Solução Moderna**: Aprenda sobre as práticas atuais de desenvolvimento e operações que estão moldando o futuro da tecnologia. Docker é uma habilidade essencial em muitas áreas de TI, incluindo engenharia de dados, e dominá-la abrirá novas oportunidades profissionais.

## Agenda

### Parte 1: Introdução ao Docker (9:00 - 10:30)

- **9:00 - 9:15**: Boas-vindas e Introdução
- **9:15 - 9:45**: Docker e o Ecossistema de Cloud
- **9:45 - 10:00**: Introdução ao Heroku
- **10:00 - 10:30**: Prática: Deploy de uma Aplicação Simples no Docker

### Intervalo (10:30 - 11:00)

### Parte 2: Aplicações de Dados Avançadas com Docker (11:00 - 13:00)

- **11:00 - 11:30**: Deploy de um Banco de Dados PostgreSQL com Docker
- **11:30 - 12:15**: Construção de uma Solução de Dashboard com Streamlit e DuckDB
- **12:15 - 12:55**: Projeto Integrado: Dashboard com Dados do PostgreSQL
- **12:55 - 13:00**: Conclusão e Encerramento

## 📁 Estrutura do Projeto

```
02-deploy-data-apps/
├── src/
│   ├── dashboard/          # Dashboard Streamlit
│   │   ├── app.py          # Aplicação Streamlit
│   │   ├── Dockerfile      # Container do dashboard
│   │   └── requirements.txt
│   ├── collector/          # ETL de coleta de dados
│   │   ├── Dockerfile      # Container da ETL
│   │   └── requirements.txt
│   └── postgres/           # Configuração PostgreSQL
├── pics/
│   └── arquitetura.png     # Diagrama da arquitetura
├── pyproject.toml          # Dependências Poetry
└── README.md               # Este arquivo
```

## 🛠️ Tecnologias e Ferramentas

- **Docker**: Containerização de aplicações
- **Docker Compose**: Orquestração de containers
- **PostgreSQL**: Banco de dados relacional
- **Streamlit**: Framework para dashboards
- **DuckDB**: Banco de dados analítico
- **Python**: Linguagem de programação

## 📦 Pré-requisitos

- Docker e Docker Compose instalados
- Conhecimento básico de Python
- Conhecimento básico de SQL
- Editor de código (recomendado: VSCode)

**Vídeos recomendados**:
- Python + VSCode + Git
- Poetry para gerenciamento de dependências

## 🚀 Como Usar

Cada diretório no repositório contém um `README.md` com instruções específicas sobre como construir e executar as aplicações correspondentes usando Docker.

### Execução Rápida

1. **Clone o repositório**:
   ```bash
   git clone https://github.com/lvgalvao/data-engineering-roadmap.git
   cd data-engineering-roadmap/02-fundamentos-dados/02-deploy-data-apps
   ```

2. **Siga as instruções** em cada subdiretório:
   - `src/dashboard/`: Deploy do dashboard
   - `src/collector/`: Deploy da ETL
   - `src/postgres/`: Configuração do banco

## 📚 Conteúdo do Workshop

### Parte 1: Introdução ao Docker (9:00 - 10:30)
- Docker e o Ecossistema de Cloud
- Introdução ao Heroku
- Prática: Deploy de uma Aplicação Simples no Docker

### Parte 2: Aplicações de Dados Avançadas (11:00 - 13:00)
- Deploy de um Banco de Dados PostgreSQL com Docker
- Construção de uma Solução de Dashboard com Streamlit e DuckDB
- Projeto Integrado: Dashboard com Dados do PostgreSQL

## 🔗 Conexões com a Formação

- **Pré-requisitos**: 
  - Módulo 01 (Git e GitHub)
  - Conhecimento básico de Python
- **Próximos passos**: 
  - Projeto 03 (CRUD API) para aplicar Docker em aplicações completas
  - Módulo de Cloud AWS em `06-cloud-aws-para-dados/`

## 📖 Recursos Adicionais

- [Documentação do Docker](https://docs.docker.com/)
- [Documentação do Docker Compose](https://docs.docker.com/compose/)
- [Documentação do Streamlit](https://docs.streamlit.io/)

---

**Parte da Formação Profissional em Engenharia de Dados - [Jornada de Dados](https://suajornadadedados.com.br/)**
