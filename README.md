# MangaZero 📚⚡

O **MangaZero** é a API Backend de uma plataforma de catálogo e leitura de mangás e quadrinhos. Este projeto foi desenvolvido com o propósito de aplicar na prática uma arquitetura resiliente e escalável no ecossistema **Java & Spring Boot**, progredindo por etapas desde o banco relacional até o deploy em nuvem.

---

## 🎯 Objetivo & Casos de Uso

A API é responsável por gerenciar todo o ecossistema do catálogo:
- **Gestão de Catálogo:** Cadastro e consulta de obras, capítulos, gêneros e tags.
- **Cache de Alta Performance:** Otimização da busca de quadrinhos populares.
- **Processamento Assíncrono:** Notificação e processamento em segundo plano para novos lançamentos.

---

## 🛠️ Tech Stack & Arquitetura

A aplicação evolui seguindo a integração das seguintes tecnologias:

1. **Java 17+ & Spring Boot:** Lógica de negócio e construção da API REST.
2. **SQL Server:** Banco de dados relacional principal.
3. **Swagger (OpenAPI 3):** Documentação interativa e contratos dos endpoints HTTP.
4. **Docker & Docker Compose:** Conteinerização da API e dos serviços auxiliares.
5. **RabbitMQ:** Mensageria assíncrona para comunicação por eventos.
6. **Redis:** Cache em memória para otimização de consultas pesadas.
7. **GCP (Google Cloud Platform):** Hospedagem da aplicação na nuvem.

---

## 🗺️ Roadmap de Evolução

- [x] **Fase 1:** Mapeamento de Entidades (JPA/SQL Server) e Endpoints REST básicos.
- [ ] **Fase 2:** Documentação da API com **Swagger / Springdoc OpenAPI**.
- [ ] **Fase 3:** Conteinerização da API e BD via **Docker Compose**.
- [ ] **Fase 4:** Implementação de mensageria assíncrona com **RabbitMQ**.
- [ ] **Fase 5:** Camada de Caching com **Redis** para rotas de alta leitura.
- [ ] **Fase 6:** Deploy na **Google Cloud Platform (GCP)**.


## 🚀 Como Rodar o Projeto Localmente

### Pré-requisitos
- **Java 17** ou superior
- **Docker** e **Docker Compose**
- **Maven 3.8+**

### Passos para Execução

1. **Clone o repositório:**
   ```bash
   git clone [https://github.com/seu-usuario/comic-reader-api.git](https://github.com/seu-usuario/comic-reader-api.git)
   cd comic-reader-api

2. **Suba os serviços externos (SQL Server, Redis, RabbitMQ) via Docker**:

```console
Bash
docker compose up -d
Execute a aplicação Spring Boot:
```
```console
Bash
./mvnw spring-boot:run
```
## 📄 Documentação da API
Quando a aplicação estiver em execução, você pode visualizar e testar os endpoints interativamente através do Swagger UI:

* **Swagger UI**: http://localhost:8080/swagger-ui.html
* **OpenAPI Docs (JSON)**: http://localhost:8080/v3/api-docs
## 📖 Documentação Adicional
Para detalhes detalhados sobre diagramas de classe, modelos de banco e especificações arquiteturais, acesse a nossa [Wiki do Repositório](https://github.com/Gabriel-J-code/MangaZero-api/wiki).