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

1. Clone the repositor:

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

JWT_SECRET=any-secret

DATABASE_URL="database-url"

If you want to use Docker just run the following command

```
docker compose up
```

And use the URl already set on .env.example

5. Run database migrations:

```
npx prisma migrate dev
```

6. Start the application:

```
npm run dev
```

The application will be available at <http://localhost:3000>.
