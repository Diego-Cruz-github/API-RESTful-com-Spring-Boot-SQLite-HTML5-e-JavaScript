# API RESTful com Spring Boot, SQLite, HTML5 e JavaScript

## Sobre o Projeto

Este é um projeto backend completo, desenvolvido com **Spring Boot**, utilizando práticas modernas de **Programação Funcional**, persistência com **SQLite**, **JPA**, **Hibernate** e **JDBC**, e integração com um frontend externo feito em **HTML5** e **JavaScript**.

A aplicação expõe uma **API RESTful** robusta e segura com suporte completo a operações **CRUD**, **cadastro em massa via REST**, e integração com ferramentas como **Postman**. Também possui proteção com **CORS** e **CSRF**, além do uso da biblioteca `org.json` para manipulação de dados JSON.

---

## 🧠 Destaques Técnicos

- ✅ Programação Funcional com Streams, Lambdas e Imutabilidade
- ✅ Cadastro em Massa via JSON (Bulk Insert)
- ✅ Integração com HTML5/JavaScript externo via Web Client
- ✅ API RESTful documentada e testável com Postman
- ✅ Persistência com SQLite, JPA, Hibernate e JDBC
- ✅ Segurança com CORS e CSRF
- ✅ Manipulação de dados com biblioteca JSON

---

## 🚀 Tecnologias Utilizadas

- Java 17
- Spring Boot 3
- JPA / Hibernate (ORM)
- JDBC
- SQLite
- Maven
- HTML5
- JavaScript (ES6+)
- Postman
- CORS / CSRF
- Biblioteca JSON (org.json)

---

## 🛠️ Funcionalidades

- API RESTful com endpoints para produtos e pedidos
- CRUD completo
- Cadastro em massa via REST
- Integração com frontend HTML5/JS
- Tratamento de exceções
- Segurança com CORS e CSRF

---

## 📦 Endpoints da API

### Produtos

| Método | Rota            | Descrição                        |
|--------|------------------|----------------------------------|
| GET    | `/products`      | Lista todos os produtos          |
| POST   | `/products`      | Cria um novo produto             |
| GET    | `/products/{id}` | Retorna um produto específico    |
| PUT    | `/products/{id}` | Atualiza um produto              |
| DELETE | `/products/{id}` | Deleta um produto                |

### Pedidos

| Método | Rota         | Descrição                          |
|--------|--------------|-------------------------------------|
| POST   | `/orders`    | Cria um novo pedido                 |
| GET    | `/orders/{id}` | Retorna um pedido específico      |

### Exemplo: Cadastro de Pedido

**POST `/orders`**
```json
{
  "userId": 1,
  "items": [
    {
      "productId": 1,
      "quantity": 2
    }
  ]
}
💾 Banco de Dados
A aplicação utiliza SQLite, um banco leve e baseado em arquivos. O acesso é feito via JPA/Hibernate e JDBC.

Configuração exemplo no application.properties:

properties
Copiar
Editar
spring.datasource.url=jdbc:sqlite:meu_banco_de_dados.db
spring.datasource.driver-class-name=org.sqlite.JDBC
spring.jpa.database-platform=org.hibernate.dialect.SQLiteDialect
🧪 Testes com Postman
Importe os endpoints da API no Postman.

Realize requisições CRUD.

Teste com dados em massa.

Teste headers de CORS e CSRF.

🌐 Frontend HTML5 + JavaScript
O projeto inclui um frontend que consome a API REST via fetch().

📁 Baixe o exemplo:
frontend-html-example.zip

Exemplo de uso no navegador:
javascript
Copiar
Editar
fetch('http://localhost:8080/products')
  .then(res => res.json())
  .then(data => console.log(data));
▶️ Como Executar
bash
Copiar
Editar
# Clone o projeto
git clone https://github.com/Diego-Cruz-github/projeto-Springboot.git

# Acesse o diretório
cd projeto-Springboot

# Execute com Maven
./mvnw spring-boot:run
A aplicação estará disponível em:
http://localhost:8080

👨‍💻 Autor
Diego Fonte Boa Cruz
LinkedIn

perl
Copiar
Editar
