# Laboratório: API RESTful com Jakarta EE

Projeto desenvolvido para a disciplina de Sistemas Distribuídos. Implementa uma API REST simples utilizando **JAX-RS** e **EJB Stateless**, rodando sobre o servidor **WildFly**.

## Pré-requisitos
Apenas o **Docker** instalado. Não é necessário instalar Java ou Maven localmente.

## Como Rodar

### 1. Construir a Imagem
No terminal, dentro da pasta do projeto:

```bash
docker build -t lab-api .

```

### 2. Iniciar o Servidor

```bash
docker run -d -p 8080:8080 --name lab-api-container lab-api

```

### 3. Testar a API

Abra no navegador ou use o `curl`:

**URL:**
`http://localhost:8080/HelloAPI/api/hello/SeuNome`

**Resposta Esperada:**

> Olá, SeuNome! Bem-vindo à API EJB com Jakarta EE.


### 4. Parar e Limpar

Para parar o servidor e remover o container:

```bash
docker stop lab-api-container
docker rm lab-api-container

```