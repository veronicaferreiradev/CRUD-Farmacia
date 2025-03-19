# 🏥 CRUD-Farmacia

Este projeto é um **backend** para uma farmácia, desenvolvido com **Spring Boot**, que permite o gerenciamento de **produtos** e **categorias** através de uma API REST.

## 🚀 Tecnologias Utilizadas
- **Java 17**
- **Spring Boot**
- **Spring Data JPA**
- **MySQL**
- **Hibernate**
- **Maven**
- **Postman/Insomnia** (para testes)

---

## 📋 **Requisitos do Projeto**
### ✅ **1. Configuração Inicial**
- Criar um repositório no GitHub chamado **CRUD-Farmacia**.
- Criar um projeto no **Spring Boot** seguindo boas práticas.
- Configurar o banco de dados no arquivo `application.properties`.
- Testar a aplicação e validar a configuração do `pom.xml` e `application.properties`.
- Criar uma branch **`configurando-o-Projeto`** e subir as alterações.

### ✅ **2. CRUD de Categoria**
- Criar a entidade **Categoria** e implementar os **6 métodos CRUD** (`GET`, `POST`, `PUT`, `DELETE`).
- **Não há relacionamento de entidades nesta etapa.**
- Criar uma branch **`CRUD-Categoria`** e subir as alterações.

### ✅ **3. CRUD de Produto com Relacionamento**
- Criar a entidade **Produto** e implementar os **6 métodos CRUD**.
- Relacionar **Produto** com **Categoria** (One-to-Many).
- Criar uma branch **`CRUD-produto`** e subir as alterações.

---

## 🔧 **Configuração do Banco de Dados**
No arquivo **`src/main/resources/application.properties`**, configure seu banco MySQL:

```properties
spring.datasource.url=jdbc:mysql://localhost:3306/db_farmacia
spring.datasource.username=root
spring.datasource.password=senha
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.jpa.properties.hibernate.format_sql=true
spring.sql.init.mode=always
