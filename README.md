# Dependencias
* Node.js
* MongoDB Community Server
* NPM
    * Express
    * Mongoose
    * Bcrypt
    * Jsonwebtoken
    * Dotenv

# Como Testar?
1. Cadastrar o Usuário
    * Método: POST
    * URL: http://localhost:3000/api/signup
    * CORPO:
    ```json
    {
        "username": "usuario1",
        "password": "senha123"
    }
    ```
2. Fazer Login
    * Método: POST
    * URL: http://localhost:3000/api/login
    * CORPO:
    ```json
    {
        "username": "usuario1",
        "password": "senha123"
    }
    ```
3. Acessar Rota Protegida
    * Método: GET
    * URL: http://localhost:3000/api/protected
    * HEADER: Authorization Bearer **seu_token_aqui**

## Environment Variables
* JWT_SECRET
* MONGODB_URI