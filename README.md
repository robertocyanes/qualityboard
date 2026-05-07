QualityBoard
📌 Sobre o Projeto

O QualityBoard é um sistema moderno de gerenciamento de tarefas inspirado no projeto Board da DIO, porém evoluído para uma arquitetura profissional baseada em microsserviços.

O objetivo do projeto é demonstrar conhecimentos sólidos em:

Java moderno
Spring Boot
Microsserviços
Segurança com JWT
Docker
API Gateway
Service Discovery
Testes automatizados
Qualidade de software
Arquitetura backend
Documentação profissional

♦️ Arquitetura do Projeto:
QualityBoard/
│
├── discovery-service/
├── gateway-service/
├── auth-service/
├── user-service/
├── board-service/
├── task-service/
├── notification-service/
├── docker-compose.yml
└── README.md

🚀 Tecnologias Utilizadas:
Backend
Java 21
Spring Boot 3
Spring Cloud
Spring Security
Spring Data JPA
Maven
Banco de Dados
PostgreSQL
Microsserviços
Eureka Server
Spring Cloud Gateway
Segurança
JWT Authentication
BCrypt Password Encoder
Testes
JUnit 5
Mockito
MockMvc
Testcontainers
Cypress
Documentação
Swagger/OpenAPI
DevOps
Docker
Docker Compose
GitHub Actions

🔶 Microsserviços
discovery-service

Responsável pelo registro e descoberta de microsserviços utilizando Eureka Server.

Porta
8761
gateway-service

Responsável pelo roteamento central das APIs.

Funcionalidades:
roteamento
autenticação
filtros globais
controle de acesso
Porta
8080
auth-service

Responsável pela autenticação da aplicação.

Funcionalidades:
login
geração de JWT
refresh token
validação de token
Endpoints
POST /auth/login
POST /auth/refresh
user-service

Responsável pelo gerenciamento de usuários.

Funcionalidades:
cadastro
atualização
exclusão
listagem
board-service

Responsável pelos boards da aplicação.

Funcionalidades:
criar board
atualizar board
remover board
listar boards
task-service

Responsável pelas tarefas.

Funcionalidades:
criar tarefas
alterar status
prioridade
datas
comentários
movimentação entre colunas
notification-service

Responsável pelas notificações e logs futuros.

Futuras melhorias:
envio de email
eventos
webhooks

♦️ Modelagem
User
UUID id;
String name;
String email;
String password;
Role role;
LocalDateTime createdAt;
Board
UUID id;
String name;
String description;
UUID ownerId;
LocalDateTime createdAt;
Task
UUID id;
String title;
String description;
TaskStatus status;
TaskPriority priority;
UUID boardId;
LocalDate deadline;
LocalDateTime createdAt;

♦️ Segurança
O projeto utiliza autenticação JWT com rotas protegidas.

Recursos implementados:
JWT Authentication
BCrypt
Roles
Rotas protegidas
Authorization Filters

📚 Swagger
Documentação automática disponível em:
http://localhost:8080/swagger-ui.html

🟦 Docker
O projeto utiliza Docker Compose para subir toda a infraestrutura.

Containers
PostgreSQL
Eureka Server
API Gateway
Microsserviços
Executar
docker-compose up --build


♦️ Como Executar o Projeto:

1. Clonar o repositório
git clone https://github.com/seuusuario/QualityBoard.git
2. Entrar na pasta
cd QualityBoard
3. Subir containers
docker-compose up --build
4. Executar microsserviços
mvn spring-boot:run

✅ Testes
Tipos de testes implementados:

Unitários
Services
Validations
Rules
Integração
Controllers
Repositories
E2E
Cypress
Cobertura esperada
80%+

✅ Qualidade de Software
O projeto segue boas práticas de desenvolvimento:

Clean Code
SOLID
Arquitetura em camadas
Tratamento global de exceções
Logs estruturados
Validação de entrada
DTO Pattern

✅ Melhorias em Relação ao Projeto Original
Melhorias adicionadas
Microsserviços
Docker
JWT
Swagger
PostgreSQL
Gateway API
Eureka
Testes automatizados
Cypress
CI/CD
Estrutura profissional
Documentação completa

✅ Melhorias Futuras
Próximas implementações
Kafka
Redis
RabbitMQ
Kubernetes
Observabilidade
Prometheus
Grafana
ELK Stack
Cache distribuído

🔷 Screenshots
Futuramente adicionar
Swagger
Docker containers
Endpoints
Dashboard

✅ Objetivo Profissional
O QualityBoard foi desenvolvido para demonstrar conhecimentos reais de backend moderno utilizando tecnologias amplamente utilizadas no mercado.

O foco principal do projeto é:
arquitetura
qualidade
escalabilidade
testes
organização
boas práticas

Autor:
Roberto César Yanes

Likedin: robertocyanes

