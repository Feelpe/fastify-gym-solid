# Fastify Gym SOLID 

![TypeScript](https://img.shields.io/badge/typescript-%23007ACC.svg?style=for-the-badge&logo=typescript&logoColor=white) ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=for-the-badge&logo=node.js&logoColor=white) ![Fastify](https://img.shields.io/badge/fastify-%23000000.svg?style=for-the-badge&logo=fastify&logoColor=white) ![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=for-the-badge&logo=vite&logoColor=white) ![Prisma](https://img.shields.io/badge/Prisma-3982CE?style=for-the-badge&logo=Prisma&logoColor=white) ![ESLint](https://img.shields.io/badge/ESLint-4B3263?style=for-the-badge&logo=eslint&logoColor=white) 

This project is a Gym Management System designed to provide essential functionalities for gym users and administrators. It covers a range of features, including user registration, authentication, profile retrieval, check-in history, searching for nearby gyms, checking in at gyms, and registering new gyms.

## Functional 

1. User Management:

- Users can register an account.
- Users can authenticate using their credentials.
- Users can retrieve their profiles.

2. Check-In:

- Users can check in at a gym.
- Users can validate their check-ins.
- Users can view their check-in history.
- Users cannot check in twice on the same day.
- Users must be within 100 meters of the gym to check-in.

3. Gym Management:

- Users can search for gyms nearby (within 10km).
- Users can search for gyms by name.
- Users can view the number of check-ins at a gym.

4. Admin Operations:

- Admins can register a new gym.
- Admins can validate user check-ins.
- Admins can register with a unique email.

## Getting Started

Ensure you have the following tools installed:

Node.js
PostgreSQL

1. Clone the repository:

```
git clone https://github.com/Feelpe/fastify-gym-solid
```

2. Enter the project directory:

```
cd fastify-gym-solid
```

3. Install dependencies:

```
npm install
```

4. Create a .env file based on the provided .env.example and fill in the required credentials.

5. Run database migrations:

```
npx prisma db push
```

6. Start the application:

```
npm run dev
```

The application will be available at http://localhost:3000.

## RFs (Requisitos funcionais)

- [x] Deve ser possível se cadastrar;
- [x] Deve ser possível se autenticar;
- [x] Deve ser possível obter o perfil de um usuário logado;
- [x] Deve ser possível obter o número de check-ins realizados pelo usuário logado;
- [x] Deve ser possível o usuário obter seu histórico de check-ins;
- [x] Deve ser possível o usuário buscar academias próximas (até 10km);
- [x] Deve ser possível Deve ser possível o usuário buscar academias pelo nome;
- [x] Deve ser possível o usuário realizar check-in em uma academia;
- [x] Deve ser possível validar o check-in de um usuário;
- [x] Deve ser possível cadastrar uma academia;

## RNs (Regras de negócio)

- [x] O usuário não deve poder se cadastrar com um e-mail duplicado;
- [X] O usuário não pode fazer 2 check-ins no mesmo dia;
- [X] O usuário não pode fazer check-in se não estiver perto (100m) da academia;
- [x] O check-in só pode ser validade até 20 minutos após criado;
- [x] O check-in só pode ser validado por administradores;
- [x] A academia só pode ser cadastrada por administradores;

## RNFs (Requisitos não-funcionais)

- [x] A senha do usuário precisa estar criptografado;
- [x] Os dados da aplicação precisa estar persistido em um banco PostgreSQL;
- [x] Todas as listas de dados precisam estar paginadas com 20 itens por página;
- [x] O usuário deve ser identificados por um JWT (JSON Web Token);
