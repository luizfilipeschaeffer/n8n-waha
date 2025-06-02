# n8n - Ambiente Docker

## Pré-requisitos
- [Docker](https://www.docker.com/get-started) instalado
- [Docker Compose](https://docs.docker.com/compose/install/) instalado

## Subindo o ambiente

1. **Clone o repositório (se necessário):**
   ```bash
   git clone https://github.com/luizfilipeschaeffer/n8n-waha
   cd n8n-waha
   ```

2. **Suba os containers:**
   ```bash
   docker-compose up -d
   ```

3. **Acesse os serviços:**
   - **n8n:** [http://localhost:5678](http://localhost:5678)
   - **Waha:** [http://localhost:3000](http://localhost:3000)
   - **Postgres:** localhost:5432 (user: default, senha: default)
   - **Redis:** localhost:6379 (user: default, senha: default)

## Volumes Persistentes
- Os dados dos serviços são mantidos nos volumes Docker declarados no `docker-compose.yml`.

## Parar o ambiente
```bash
docker-compose down
```

## Observações
- As variáveis de ambiente podem ser ajustadas conforme necessidade no arquivo `docker-compose.yml`.
- O serviço n8n está configurado para uso local e testes.

---
Dúvidas ou problemas? Abra uma issue no repositório. 