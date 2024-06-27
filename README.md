# Curso Spring Boot 3 JPA

Este projeto é um exemplo de aplicação usando Spring Boot 3 e JPA (Java Persistence API). Ele foi desenvolvido como parte de um workshop para demonstrar a criação e o gerenciamento de entidades e repositórios em um contexto de uma aplicação web.

## Estrutura do Projeto

O projeto está organizado da seguinte forma:

.mvn/
src/
├── main/
│ └── java/
│ └── com/
│ └── educandoweb/
│ └── course/
│ ├── config/
│ │ └── TestConfig.java
│ ├── entities/
│ │ ├── enums/
│ │ └── pk/
│ │ ├── Category.java
│ │ ├── Order.java
│ │ ├── OrderItem.java
│ │ ├── Payment.java
│ │ ├── Product.java
│ │ └── User.java
│ ├── repositories/
│ │ ├── CategoryRepository.java
│ │ ├── OrderItemRepository.java
│ │ ├── OrderRepository.java
│ │ ├── ProductRepository.java
│ │ └── UserRepository.java
│ ├── resources/
│ │ ├── exceptions/
│ │ ├── CategoryResource.java
│ │ ├── OrderResource.java
│ │ ├── ProductResource.java
│ │ └── UserResource.java
│ ├── services/
│ │ ├── exceptions/
│ │ ├── CategoryService.java
│ │ ├── OrderService.java
│ │ ├── ProductService.java
│ │ └── UserService.java
│ └── CourseApplication.java
├── test/
│ └── java/
│ └── com/
│ └── educandoweb/
│ └── course/
│ └── resources/
│ └── TestConfig.java
.gitignore
mvnw
mvnw.cmd
pom.xml


### Pacotes

- **config**: Contém classes de configuração.
- **entities**: Contém classes de entidade JPA.
  - **pk**: Contém classes de chave primária compostas.
- **repositories**: Contém interfaces de repositório JPA.
- **resources**: Contém classes de controle REST.
  - **exceptions**: Contém classes de tratamento de exceções para recursos.
- **services**: Contém classes de serviço.
  - **exceptions**: Contém classes de tratamento de exceções para serviços.

### Entidades

- `Category.java`
- `Order.java`
- `OrderItem.java`
- `Payment.java`
- `Product.java`
- `User.java`

### Repositórios

- `CategoryRepository.java`
- `OrderItemRepository.java`
- `OrderRepository.java`
- `ProductRepository.java`
- `UserRepository.java`

### Recursos

- `CategoryResource.java`
- `OrderResource.java`
- `ProductResource.java`
- `UserResource.java`

### Serviços

- `CategoryService.java`
- `OrderService.java`
- `ProductService.java`
- `UserService.java`

## Funcionalidades

- CRUD de usuários, produtos, pedidos e categorias.
- Associação muitos-para-muitos com atributos adicionais.
- Manipulação de exceções personalizada.
- Métodos para cálculo de subtotal e total.

## Como Executar

### Pré-requisitos

- Java 17 ou superior.
- Maven 3.6.0 ou superior.

### Passos

# Clone o repositório
git clone https://github.com/seu-usuario/workshop-springboot3-jpa-cursojava.git

# Navegue até o diretório do projeto
cd workshop-springboot3-jpa-cursojava

# Execute a aplicação
./mvnw spring-boot:run

# A aplicação estará disponível em http://localhost:8080

# Endpoints
GET /categories: Lista todas as categorias.
POST /categories: Adiciona uma nova categoria.
GET /users: Lista todos os usuários.
POST /users: Adiciona um novo usuário.

# Para mais detalhes sobre os endpoints, consulte as classes no pacote resources.




