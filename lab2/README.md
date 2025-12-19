# API de Estoque - Python

API REST desenvolvida com FastAPI para gerenciamento simples de aparelhos, utilizando XML para persistência de dados.

## Instalação

Crie e ative seu ambiente virtual, depois instale as dependências:

```bash
pip install -r requirements.txt
```

## Configuração

Antes da primeira execução, gere o arquivo de configuração necessário:

```bash
python config.py
```

## Como rodar

Inicie o servidor:

```bash
uvicorn app:app --reload
```