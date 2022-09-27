# API OO Trix

Uma API orienta a objetos para gerenciamento de transferências bancárias.

Essa API é usada como exemplo didático para o bloco de Arquitetura de Software do Curso de Desenvolvimento Web da Trybe.

<details>
  <summary>Branches no repositório</summary>

  1. `main`: Configurações de linter e configurações gerais;
  2. `application-course`: Conteúdo ensinado no course;
  3. `application-live-lectures`: Conteúdo ensinado no course juntamente com a aula ao vivo;
  4. `application-course-part-2`: Conteúdo ensinado no course;
  5. `application-live-lectures-part-2`: Conteúdo ensinado no course juntamente com a aula ao vivo

</details>

## Rodando a aplicação inicial via Docker

- Clone o repositório via `HTTPS`:

```bash
  git clone https://github.com/tryber/poo-trix.git
```

- Ou via `SSH`:

```bash
  git clone git@github.com:tryber/poo-trix.git
```

- Vá até a branch desejada:

```bash
  git checkout BRANCH_NAME
```

- Inicie os contêineres via Docker Compose:
  
```bash
  docker-compose up -d
```

> 👀 Observação: Dois contêineres serão subidos, um para a aplicação Node TypeScript, denominado `trix` e outro para o banco de dados MongoDB, denominado `trix_db`

- Para acessar o contêiner do banco de dados, basta seguir os comando abaixo:

  ```bash
    docker exec -it trix_db bash
  ```

  - Agora dentro do contêiner, execute o comando abaixo para ter acesso ao terminal do MongoDB:

  ```bash
    mongo
  ```

  > 👀 Observação: Aqui você pode executar comandos como: `show dbs`, `use COLLECTION_NAME`, `show collections` e etc...

- Para acessar o contêiner da aplicação, basta seguir os comando abaixo:

```bash
  docker exec -it trix bash
```

- Dentro do contêiner instale as dependências:

```bash
  npm i
```

## Lista de endpoints

> ⚠️ Dica: Há uma coleção dos endpoints em formato JSON para importação na extensão [Thunder Client](https://marketplace.visualstudio.com/items?itemName=rangav.vscode-thunder-client) do VS Code no arquivo `thunder-trix.json`

<details>
  <summary>Como importar a coleção no Thunder Client</summary>

  1. Abra a aba da extensão Thunder Client;
  2. Clique na aba Collections;
  3. Clique no menu de opções;
  4. Clique em Import;
  5. Escolha o arquivo `thunder-trix.json`;
  6. Clique em OK.

</details>

### 1° Dia

- Feitos no course:
  - POST `/transfer`;
- Feitos na aula ao vivo:
  - PUT `/transfer/:id`;
- Para serem feitos no exercício do dia:
  - GET `/transfer`;
  - GET `/transfer/:key`;

### 2° Dia

🚧 Em construção... 🚧
