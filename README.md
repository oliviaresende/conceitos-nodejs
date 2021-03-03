# Conceitos do Node.js

Essa será uma aplicação para armazenar repositórios do seu portfólio, que irá permitir a criação, listagem, atualização e remoção dos repositórios, e além disso permitir que os repositórios possam receber "likes".

****
## *Sobre o projeto* ⭐️
### *Principais funcionalidades:*

- POST /repositories: A rota deve receber title, url e techs dentro do corpo da requisição, sendo a URL o link para o github desse repositório. Ao cadastrar um novo projeto, ele deve ser armazenado dentro de um objeto no seguinte formato: { id: "uuid", title: 'Desafio Node.js', url: 'http://github.com/...', techs: ["Node.js", "..."], likes: 0 }; Certifique-se que o ID seja um UUID, e de sempre iniciar os likes como 0.

- GET /repositories: Rota que lista todos os repositórios;

- PUT /repositories/:id: A rota deve alterar apenas o title, a url e as techs do repositório que possua o id igual ao id presente nos parâmetros da rota;

- DELETE /repositories/:id: A rota deve deletar o repositório com o id presente nos parâmetros da rota;

- POST /repositories/:id/like: A rota deve aumentar o número de likes do repositório específico escolhido através do id presente nos parâmetros da rota, a cada chamada dessa rota, o número de likes deve ser aumentado em 1;

### *Tecnologias usadas:*

- [Node](https://nodejs.org/en/);
- [Express](https://expressjs.com/pt-br/);
- [Jest](https://jestjs.io/);

****
## *Como instalar e rodar ?* 🚀
###  *Pré-requisitos:*
1. Ter o **[Node js](https://nodejs.org/en/) instalado** e junto dele a **[Yarn](https://yarnpkg.com/)**;

2. **Clonar o repositório** em sua máquina, usando comando abaixo em seu terminal:

```
  git clone https://github.com/oliviaresende/concepts-nodejs.git
```

3. **Acessar o repositório**:

```
  cd concepts-nodejs
```

4. Agora basta **instalar as dependências** do seu projeto, digitando no terminal:

```
  yarn install
```

5. E por ultimo dar o comando para **rodar** seu projeto:

```
  yarn dev
```

 > *Obs: O projeto irá rodar no http://localhost:3333*

 ****

### Como executar os testes usando o Jest ? 🚀

Para ver os testes em ação, basta executar o seguinte comando:

```
  yarn test
```

 ****
