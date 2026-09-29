# Hello FastAPI

Aplicação simples desenvolvida com FastAPI para o exercício prático de Docker, GitHub Actions e Container Registry.

## Executando localmente

Instale as dependências:

```bash
pip install -r requirements.txt
```

Execute a aplicação:

```bash
uvicorn app.main:app --reload
```

A aplicação estará disponível em:

```text
http://localhost:8000
```

Endpoint:

```text
GET /hello
```

Resposta:

```text
"Hello World"
```

## Executando com Docker

Construir a imagem:

```bash
docker build -t hello-fastapi:1.0 .
```

Executar o container:

```bash
docker run -p 8080:8000 hello-fastapi:1.0
```

Testar:

```bash
curl http://localhost:8080/hello
```
