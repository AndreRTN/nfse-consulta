# NFSe Consulta

## Objetivo
API RESTful em Spring Boot para consulta de créditos constituídos com front-end Angular. Fornece informações sobre número do crédito, NFS-e, data da constituição, valor do ISSQN e tipo do crédito.

## Pré-requisitos
- Docker
- Docker Compose
- Git


## Como subir o projeto completo

```bash
git clone --recursive https://github.com/seu-usuario/nfse-consulta.git
cd nfse-consulta
```

### Comando único para subir tudo:
```bash
docker-compose up --build
```

### Primeira execução (com rebuild):
```bash
docker-compose up --build -d
```

### Execuções subsequentes:
```bash
docker-compose up -d
```

## Comandos úteis

### Parar todos os serviços:
```bash
docker-compose down
```

### Rebuild completo (sem cache):
```bash
docker-compose build --no-cache
```

### Ver logs dos serviços:
```bash
docker-compose logs
```

### Ver logs de um serviço específico:
```bash
docker-compose logs nfse-frontend
docker-compose logs nfse-backend
```

## Acessos

- **Frontend**: http://localhost:4200
- **Backend API**: http://localhost:8084
- **Documentação API**: http://localhost:8084/api/swagger-ui.html
- **Kafka UI**: http://localhost:8080
- **PostgreSQL**: localhost:5432