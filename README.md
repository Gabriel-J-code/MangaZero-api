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
- [x] **Fase 1:** [Documentação](https://docs.google.com/document/d/13SXX82LuXVu4r3rC-4H9vGxtesry345oRv08JfcVAi8/edit?usp=sharing).
   * [x] Escopo
   * [x] Requisitos
   * [ ] Histórias de Usuário  e Cenários BDD
   * [ ] Arquitetura e Modelagem (UML, definição de frameworks, fluxos)
   * [ ] Prototipação (Figma)
   * [ ] Configuração do Workspace (Kanban)
   * [ ] Preparação do Ambiente de Desenvolvimento
- [ ] **Fase 2:** Mapeamento de Entidades (JPA/SQL Server) e Endpoints REST básicos.
- [ ] **Fase 3:** Documentação da API com **Swagger / Springdoc OpenAPI**.
- [ ] **Fase 4:** Conteinerização da API e BD via **Docker Compose**.
- [ ] **Fase 5:** Implementação de mensageria assíncrona com **RabbitMQ**.
- [ ] **Fase 6:** Camada de Caching com **Redis** para rotas de alta leitura.
- [ ] **Fase 7:** Deploy na **Google Cloud Platform (GCP)**.


## 🚀 Como Rodar o Projeto Localmente (Apenas quando o projeto passar da Fase 2)

### Pré-requisitos
- **Java 17** ou superior
- **Docker** e **Docker Compose**
- **Maven 3.8+**

### Passos para Execução

1. **Clone o repositório**   

2. **Suba os serviços externos (SQL Server, Redis, RabbitMQ) via Docker**:

```console
Bash
docker compose up -d
```
Execute a aplicação Spring Boot:
```console
Bash
./mvnw spring-boot:run
```
## 📄 Documentação da API
Quando a aplicação estiver em execução, você pode visualizar e testar os endpoints interativamente através do Swagger UI:

* **Swagger UI**: http://localhost:8080/swagger-ui.html
* **OpenAPI Docs (JSON)**: http://localhost:8080/v3/api-docs

