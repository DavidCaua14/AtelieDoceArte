# Ateliê Doce e Arte

Ateliê Doce e Arte é um aplicativo para gerenciar a venda de doces

## Detalhes
| Tecnologia |
|---|
| Laravel 8 REST API
| React Native

## Resumo das Funcionalidaedes
- Gerenciar Produtos
- Gerenciar Categorias
- Login e Cadastro de Usuário

## Como executar?
**Importante:** É necessário ter o composer, NodeJs e o PHP ^7.3 ou ^8.0.
- Abra o terminal na pasta api e rode o seguinte comando: 
``` composer install ```
- Apos isso, configure o .env e execute o comando para criar as tabelas: 
``` php artisan migrate ```
- Após isso execute o comando para rodar a aplicação:
``` php artisan serve --host=0.0.0.0 --port=8000 ```

- Abra o terminal na pasta doceria e rode o seguinte comando: 
``` npm install ```
- Após isso execute o comando para rodar a aplicação: 
``` npm start ```

**Importante:** Baixe o expo go no seu celular e esteja na mesma rede que o backend está rodando e leia o qrcode do terminal da pasta doceria.

## Usuário Adminstrador
Faça o login com o usuário administrador para ter acesso a todas as funcionalidades. 

- Crie um usuário novo, vá ate o banco de dados e modifique o seu level para 10

## Documentação da API

#### Gerenciamento de Produtos

```http 
  POST /api/produto
  GET /api/produtos
  POST /api/produto/{id}
  GET /api/produto/{id}
  DELETE /api/produto/{id}
```

#### Gerenciamento de Categorias

```http 
  POST /api/categoria
  GET /api/categorias
  PUT /api/categoria/{id}
  GET /api/categoria/{id}
  DELETE /api/categoria/{id}
```

#### Login e Cadastro de Usuário

```http 
  POST /api/login
  POST /api/register
```