## Executing the project

### Clone the repository and submodules

```bash
 $ git clone --recurse-submodules https://github.com/JoaoLiima/payever-workspace.git
```

### Install dependencies

Get inside `payever-api` and install the dependencies with:

```bash
$ npm install
```

or

```bash
$ yarn install
```

### Executing the application

Inside `payever-workspace` there is an .env.example file, create a .env file based on that one and then execute:

```bash
$ sudo docker-compose up
```

### Using the application

Once the application is up and runnig, you can access the endpoints with insomnia or postman. There are currently 4 endpoist:

GET /api/user/{userId}
GET /api/user/{userId}/avatar
DELETE /api/user/{userId}/avatar
POST /api/user - for this one, you need to send a JSON body, here is an example:

```bash
  {
    "email": "email@test.com",
    "first_name": "Test",
    "last_name": "Mail"
  }
```

## Tech stack

> - [NodeJS](https://nodejs.org/en/)
> - [NestJS](https://nestjs.com/)
> - [TypeScript](https://www.typescriptlang.org/)
> - [Axios](https://axios-http.com/ptbr/docs/intro)
> - [Jest](https://jestjs.io/)
> - [Docker](https://www.docker.com/)
