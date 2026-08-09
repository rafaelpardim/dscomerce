#  DSCommerce - API Rest & Modelo de Domínio / ORM



O **DSCommerce** é um sistema de e-commerce e back-end construído para demonstrar a implementação de um modelo de domínio complexo com **Mapeamento Objeto-Relacional (ORM)** via **Spring Data JPA / Hibernate**, contendo relacionamentos `1:N`, `N:N`, `1:1` e classe de associação com chave primária composta.

---

 Sumário
- [Características e Tecnologias](#-características-e-tecnologias)
- [Modelo de Domínio (UML)](#-modelo-de-domínio-uml)
- [Estrutura do Banco de Dados & ORM](#-estrutura-do-banco-de-dados--orm)
- [Casos de Uso Principais](#-casos-de-uso-principais)
- [Configuração do Ambiente](#-configuração-do-ambiente)
- [Como Executar o Projeto](#-como-executar-o-projeto)
- [Console do Banco H2](#-console-do-banco-h2)

---

##  Características e Tecnologias

- **Linguagem**: Java 21 (LTS)
- **Framework**: Spring Boot (Spring Data JPA, Spring Web)
- **Banco de Dados Em Memória**: H2 Database
- **IDE Recomendada**: IntelliJ IDEA
- **Gerenciador de Dependências**: Maven
- **Modelagem ORM**:
  - Relacionamento N:N clássico (`Product` ↔ `Category`)
  - Relacionamento N:N com classe de associação e chave composta (`OrderItem` com `@EmbeddedId` / `@Embeddable`)
  - Relacionamento 1:1 com reutilização de ID (`Order` ↔ `Payment` usando `@MapsId`)
  - Relacionamento 1:N (`User` ↔ `Order`)

---

