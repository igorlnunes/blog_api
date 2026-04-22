# 🚀 DIO Blog API

Bem-vindo ao **DIO Blog API**! Esta é uma solução moderna e assíncrona desenvolvida com **FastAPI**, projetada para gerenciar posts de blog com eficiência e segurança.

O projeto foi construído seguindo as melhores práticas de desenvolvimento Python, utilizando programação assíncrona para alta performance e uma arquitetura limpa e organizada.

---

## 🛠️ Tecnologias Utilizadas

O projeto utiliza um stack tecnológico robusto e atual:

*   **Python 3.11+** 🐍
*   **FastAPI**: Framework web de alta performance. ⚡
*   **SQLAlchemy & Databases**: Para interação assíncrona com o banco de dados. 🗄️
*   **Alembic**: Gerenciamento de migrações de banco de dados. 🔄
*   **Pydantic**: Validação de dados e configurações. ✅
*   **Poetry**: Gerenciamento de dependências e ambientes virtuais. 📦
*   **Pytest**: Suíte de testes automatizados. 🧪

---

## ✨ Funcionalidades

*   **Autenticação JWT**: Segurança robusta para proteção de rotas. 🔐
*   **Gestão de Posts**: CRUD completo (Criar, Ler, Atualizar, Deletar). 📝
*   **Arquitetura Assíncrona**: Pronta para lidar com múltiplas requisições simultâneas. 🚀
*   **Documentação Automática**: Swagger UI e ReDoc prontos para uso. 📖

---

## 🚀 Como Executar o Projeto

Siga os passos abaixo para configurar e rodar a aplicação em seu ambiente local.

### 1. Pré-requisitos

Certifique-se de ter instalado:
*   [Python 3.11+](https://www.python.org/)
*   [Poetry](https://python-poetry.org/)

### 2. Instalação de Dependências

No diretório raiz do projeto, execute:
```bash
poetry install
```

### 3. Configuração de Ambiente

Crie um arquivo `.env` na raiz do projeto (use o `.env.example` como base):
```bash
cp .env.example .env
```
Edite o arquivo `.env` e configure sua `DATABASE_URL`. Por padrão, o projeto utiliza SQLite:
`DATABASE_URL="sqlite:///./blog.db"`

### 4. Migrações do Banco de Dados

Para criar as tabelas necessárias no banco de dados, execute as migrações do Alembic:
```bash
poetry run alembic upgrade head
```

### 5. Execução da API

Inicie o servidor de desenvolvimento:
```bash
poetry run uvicorn src.main:app --reload
```
A API estará disponível em: `http://localhost:8000` 🌐

---

## 📖 Documentação

Uma das grandes vantagens do FastAPI é a documentação automática. Com o servidor rodando, acesse:

*   **Swagger UI**: [http://localhost:8000/docs](http://localhost:8000/docs)
*   **Redoc**: [http://localhost:8000/redoc](http://localhost:8000/redoc)

---

## 🧪 Testes

Para garantir a qualidade do código, execute a suíte de testes:
```bash
poetry run pytest
```

---

## 🌐 Deploy

O projeto inclui um script `render-deploy.sh` configurado para facilitar o deploy em plataformas como o Render.

---

<p align="center">
  Desenvolvido com ❤️ durante a trilha de Python da DIO.
</p>
