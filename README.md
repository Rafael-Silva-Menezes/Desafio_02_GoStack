# Desafio_02_GoStack

Desafio desenvolvido pela Rocketseat para criarmos uma aplicação usando os conhecimentos obtidos no módulo "Back-end com Node.js"

A aplicação consiste em :

POST /repositories: A rota recebe title, url e techs dentro do corpo da requisição, sendo a URL o link para o github desse repositório. Ao cadastrar um novo projeto, ele é armazenado dentro de um objeto no seguinte formato: { id: "uuid", title: 'Desafio Node.js', url: 'http://github.com/...', techs: ["Node.js", "..."], likes: 0 };

GET /repositories: Rota que lista todos os repositórios;

PUT /repositories/:id: A rota altera apenas o title, a url e as techs do repositório que possua o id igual ao id presente nos parâmetros dela;

DELETE /repositories/:id: A rota deleta o repositório com o id presente nos parâmetros da rota;

POST /repositories/:id/like: A rota aumenta o número de likes do repositório específico escolhido através do id presente nos parâmetros dela, a cada chamada, o número de likes é aumentado em 1;
