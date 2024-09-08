# CRUD FASTAPI POSTGRES STREAMLIT

#### Projeto de CRUD com Back e Front-end utilizandos os seguintes recursos e frameworks:

    * `Postgres`: Banco de Dados (SGBD) Utilizado na Aplicação.
    * `Sqlalchemy`: Biblioteca para Conexão e Comunicação com Banco de Dados. Ele é um ORM (Object Relational Mapper), que é uma técnica de mapeamento objeto-relacional que permite fazer a comunicação com o banco de dados utilizando objetos.
    * `Pydantic`: Biblioteca de Validação de Dados. Responsável pelo Schema e validação dos Dados Recebidos e Enviados via API.
    * `FastAPI`: Framework web para construir APIs com Python. Responsável por gerir nossas Rotas.
    * `Uvicorn`: Servidor web assíncrono, que é baseado no ASGI, que é uma especificação para servidores web assíncronos. O Uvicorn é o servidor web recomendado pelo FastAPI, e é o servidor que vamos utilizar nesse projeto.
    * `Requests`: Biblioteca para fazer requisições HTTP com Python.
    * `Pandas`: Biblioteca para manipulação de dados com Python.
    * `Streamlit`: Biblioteca para construir aplicações web com Python. Ele é muito utilizado para construir dashboards, e também para construir aplicações que consomem APIs.


####  Instalação via docker

```bash
docker-compose up -d --build
```

####  Nossa estrutura de pastas e arquivos

```bash
├── backend
│   ├── Dockerfile # arquivo de configuração do Docker
│   ├── crud.py # arquivo com as funções de CRUD utilizando o SQL Alchemy ORM
│   ├── database.py # arquivo com a configuração do banco de dados utilizando o SQL Alchemy 
│   ├── main.py
│   ├── models.py # arquivo com a modelagem das tabelas utilizando o SQL Alchemy 
│   ├── requirements.txt
│   ├── router.py # rotas de acesso a API utilizando FastAPI
│   └── schemas.py # arquivo com as validações de dados utilizando Pydantic
```

```bash
├── frontend
│   ├── .streamlit # arquivo com configurações globais do Streamlit
│   ├── app.py # arquivo com as configurações do frontend, utilizando o Streamlit
│   ├── Dockerfile # arquivo de configuração do Docker 
│   ├── requirements.txt
```