# Pets Adoption API

API RESTful para gerenciamento de adoção de pets, construída com FastAPI e SQLite.

## Sobre

Esta API permite criar, listar, atualizar e deletar registros de pets disponíveis para adoção. Desenvolvida com FastAPI para alta performance e SQLite como banco de dados leve e integrado.

## Tecnologias

- Python 3.12  
- FastAPI  
- Uvicorn (servidor ASGI)  
- SQLAlchemy (ORM)  
- SQLite

## Como rodar

1. Clone o repositório:

```bash
git clone https://github.com/JoaoVtrMorais/pets-adoption-api.git
cd pets-adoption-api
```
2. (Opcional) Crie um ambiente virtual:

```bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate     # Windows
```

3. Instale as dependências:

```bash
pip install -r requirements.txt
```

4. Execute a aplicação com Uvicorn:

```bash
uvicorn run:app --reload
```

A API estará disponível em `http://localhost:8000/`.

# Endpoints

- `GET /pets` – Lista todos os pets disponíveis para adoção

- `GET /pets/{pet_id}` – Retorna detalhes de um pet específico

- `POST /pets` – Adiciona um novo pet para adoção

- `PUT /pets/{pet_id}` – Atualiza informações de um pet

- `DELETE /pets/{pet_id}` – Remove um pet do sistema

