# API RESTful com Spring Boot, SQLite, HTML5 e JavaScript

## Sobre o Projeto
Este é um projeto backend completo, desenvolvido com **Spring Boot**, utilizando práticas modernas de **Programação Funcional**, persistência com **SQLite**, **JPA**, **Hibernate** e **JDBC**, e integração com um frontend externo feito em **HTML5** e **JavaScript**.  
A aplicação expõe uma **API RESTful** robusta e segura com suporte completo a operações **CRUD**, **cadastro em massa via REST**, e integração com ferramentas como **Postman**. Também possui proteção com **CORS** e **CSRF**, além do uso da biblioteca `org.json` para manipulação de dados JSON.

---

## 🧠 Destaques Técnicos
✅ Programação Funcional com Streams, Lambdas e Imutabilidade  
✅ Cadastro em Massa via JSON (Bulk Insert)  
✅ Integração com HTML/JavaScript externo via Web Client  
✅ API RESTful documentada e testável com Postman  
✅ Persistência com SQLite, JPA, Hibernate e JDBC  
✅ Segurança com CORS e CSRF  
✅ Manipulação de dados com biblioteca JSON  

---

## 🚀 Tecnologias Utilizadas
- Java 22  
- Spring Boot 3  
- JPA / Hibernate (ORM)  
- JDBC  
- SQLite  
- Maven  
- HTML  
- JavaScript (ES6+)  
- Postman  
- CORS / CSRF  
- Biblioteca JSON (`org.json`)  

---

## 📦 Endpoints da API

### Produtos

| Método | Rota             | Descrição                      |
|--------|------------------|--------------------------------|
| `GET`  | `/products`      | Lista todos os produtos        |
| `POST` | `/products`      | Cria um novo produto           |
| `GET`  | `/products/{id}` | Retorna um produto específico  |
| `PUT`  | `/products/{id}` | Atualiza um produto            |
| `DELETE` | `/products/{id}` | Deleta um produto              |

### Pedidos

| Método | Rota           | Descrição                      |
|--------|---------------|--------------------------------|
| `POST` | `/orders`     | Cria um novo pedido            |
| `GET`  | `/orders/{id}`| Retorna um pedido específico   |

---

## 🔄 Exemplo: Cadastro de Pedido
```json
POST /orders
{
  "userId": 1,
  "items": [
    {
      "productId": 1,
      "quantity": 2
    }
  ]
}
```

---

## 💾 Banco de Dados
```properties
spring.datasource.url=jdbc:sqlite:meu_banco_de_dados.db
spring.datasource.driver-class-name=org.sqlite.JDBC
spring.jpa.database-platform=org.hibernate.dialect.SQLiteDialect
```

---

## 🧪 Testes com Postman
```md
- Importar os endpoints da API no Postman  
- Realizar requisições CRUD  
- Testar cadastro em massa via JSON  
- Validar headers de CORS e CSRF  
```

---

## 🌐 Frontend HTML5 + JavaScript
```javascript
fetch('http://localhost:8080/products')
  .then(response => response.json())
  .then(data => console.log(data))
  .catch(error => console.error('Erro:', error));
```

---

## ▶️ Como Executar
```bash
# Clone o projeto
git clone https://github.com/Diego-Cruz-github/projeto-Springboot.git

# Acesse o diretório
cd projeto-Springboot

# Execute com Maven
./mvnw spring-boot:run
```
A aplicação estará disponível em:  
🔗 `http://localhost:8080`

---

## 👨‍💻 Autor
**Diego Fonte**  
📌 [LinkedIn](https://www.linkedin.com/in/diegof90)
