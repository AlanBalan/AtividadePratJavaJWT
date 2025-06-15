# Atividade prática - Java JWT Authentication API

## → Tecnologias

- Java 17
- Spring Boot 3+
- Spring Security
- JWT 
- H2 Database
- JPA
- Maven

## → Funcionalidades

- Cadastro de usuários com perfis ADMIN ou USER;
- Login com geração de token JWT;
- Proteção de rotas através de autenticação via token;
- Operações CRUD de usuários;
- Controle de acesso baseado em permissões.

## → Endpoints principais

### Autenticação

POST /auth/register
- Realiza o cadastro de um novo usuário (ADMIN ou USER)

POST /auth/login
- Autentica o usuário e retorna o token JWT

### Usuários

GET /user
- Retorna todos os usuários (acesso restrito a ADMIN)

GET /user/{id}
- Retorna os dados de um usuário específico

DELETE /user/{id}
- Remove um usuário (apenas ADMIN pode realizar)

PUT /user/editar
- Atualiza o próprio perfil do usuário autenticado

PUT /user/{id}
- Atualiza qualquer usuário (acesso restrito a ADMIN)


