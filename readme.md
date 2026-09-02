# API de Livros

API desenvolvida com **FastAPI e MySQL** para gerenciamento de livros.

## Tecnologias

* Python
* FastAPI
* Uvicorn
* SQLAlchemy
* PyMySQL
* MySQL
* Pydantic Settings

## Sobre o projeto

O projeto consiste na criação de uma API para cadastro e gerenciamento de livros, utilizando FastAPI para as rotas e MySQL para armazenamento dos dados.

Entre as informações dos livros estão:

* ID
* Título
* Autor
* Ano de publicação
* Disponibilidade

## Funcionalidades

A API será desenvolvida para permitir:

* Cadastrar livros
* Listar livros
* Consultar um livro
* Atualizar livros
* Excluir livros

As operações serão realizadas através das rotas da API utilizando os métodos HTTP `POST`, `GET`, `PUT` e `DELETE`.

## Estrutura

```text
api-livros/
├── app/
│   ├── __init__.py
│   ├── database.py
│   └── main.py
├── database/
│   └── biblioteca_db.sql
├── .env
├── .gitignore
└── requirements.txt
```

## Execução

Crie e ative o ambiente virtual:

```bash
python -m venv .venv
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

Configure o banco de dados MySQL e o arquivo `.env`.

Depois, execute a aplicação:

```bash
uvicorn app.main:app --reload
```

A API ficará disponível localmente e poderá ser testada através da documentação automática do FastAPI.

## Documentação

Após iniciar o servidor:

```text
http://127.0.0.1:8000/docs
```

Também existe a rota de verificação:

```text
http://127.0.0.1:8000/health
```

## Status

🚧 Projeto em desenvolvimento.
