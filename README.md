# :Construção: - Project Movieflix

- Implementação das funcionalidades necessárias para que os teste do projeto passem;
- Desenvolvimento TDD de API Rest com Java e Spring Boot;
- Realização de casos de uso;
- Consultas a banco de dados relacional com Spring Data JPA;
- Tratamento de erros com respostas HTTP customizadas;
- Controle de acesso por perfil de usuário e rotas;

##

## 🖥️ - Layout:

![image](https://github.com/carloshenriquefs/movieflix/assets/54969405/6da6c09c-45df-47ab-bfa2-d98c8448d5c1)

![image](https://github.com/carloshenriquefs/movieflix/assets/54969405/10556ee9-a05d-469a-9135-1bdf32ca2db5)

![image](https://github.com/carloshenriquefs/movieflix/assets/54969405/1b6d0649-b8fe-424e-a7db-e21e18f75c75)

##

## [![My Skills](https://skillicons.dev/icons?i=figma&theme=light)](https://skillicons.dev) - Figma:

https://www.figma.com/file/6JQVnxKgKtVHLleSBBgRin/MovieFlix-front-listagem?type=design&node-id=0-1&mode=design

##

## 📋 - Diagrama:

![movieflix drawio](https://github.com/carloshenriquefs/movieflix/assets/54969405/93e1a557-f073-44ea-b1f0-d0714459d74c)

##

## 🔍 - Casos de Uso:

### 📽️ - Listar Filmes:

- [x] - O sistema aprensenta uma listagem dos nomes de todos gêneros, bem como uma listagem paginada com título, subtítulo, ano e imagem dos filmes, ordenada alfabeticamente por título;
- [x] - O usuário visitante ou membro seleciona, opcionalmente, um gênero;
- [x] - O sistema apresenta a listagem atualzada, restringindo somente ao gênero selecionado;

### 📽️ - Visualizar detalhes do filme:

- [x] - O usuário visitante ou membro seleciona um filme;
- [x] - O sistema informa título, subtítulo, ano, imagem e sinopose do filme, e também uma listagem dos textos das avaliações daquele filme juntamente com nome do usuário que fez cada avaliação;
- [x] - O usuário membro informa, opcionalmente, um texto para avaliação do filme;
- [x] - O sistema apresenta os dados atualizados, já parecendo também a avaliação feita pelo usuário;

- [x] - O sistema apresenta uma mensagem de que não é permitido texto vazio na avaliação;

##

### ✅ - Critérios:

##

- [x] - GET /genres deve retornar 401 para token inválido;
- [x] - GET /genres deve retornar 200 com todos gêneros para VISITOR logado;
- [x] - GET /genres deve retornar 200 com todos gêneros para MEMBER logado;
- [x] - GET /movies/{id} deve retornar 401 para token inválido;
- [x] - GET /movies/{id} deve retornar 200 com o filme para VISITOR logado;
- [x] - GET /movies/{id} deve retornar 200 com o filme para MEMBER logado;
- [x] - GET /movies/{id} deve retornar 404 para id inexistente;
- [x] - GET /movies deve retornar 401 para token inválido;
- [x] - GET /movies deve retornar 200 com página ordenada de filmes para VISITOR logado;
- [x] - GET /movies deve retornar 200 com página ordenada de filmes para MEMBER logado;
- [x] - GET /movies?genreId={id} deve retornar 200 com página ordenada de filmes filtrados por gênero;
- [x] - POST /reviews deve retornar 401 para token inválido;
- [x] - POST /reviews deve retornar 403 para VISITOR logado;
- [x] - POST /reviews deve retornar 201 com objeto inserido para MEMBER logado e dados válidos;
- [x] - POST /reviews deve retornar 422 para MEMBER logado e dados inválidos;
