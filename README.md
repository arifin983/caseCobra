# CaseCobra

CaseCobra is a mobile case (cover) designing and making website where users can create custom phone covers according to their desired design.

## Table of Contents

- [CaseCobra](#casecobra)
  - [Table of Contents](#table-of-contents)
  - [Features](#features)
  - [Tech Stack](#tech-stack)
    - [Frontend](#frontend)
    - [State Management](#state-management)
    - [Authentication](#authentication)
    - [Backend](#backend)
    - [Dev Tools](#dev-tools)
  - [Prerequisites](#prerequisites)
  - [Getting Started](#getting-started)
  - [Scripts](#scripts)
  - [Environment Variables](#environment-variables)
  - [Deployment](#deployment)
  - [Contact](#contact)
  - [License](#license)

## Features

- Custom phone case designing
- Image upload and manipulation
- Real-time preview of the design
- Multiple options for colors, models, materials, and finishes
- Configuration saving and loading
- Hosted on Vercel at [http://xyz](http://xyz)

## Tech Stack

### Frontend

- Next.js
- React
- Tailwind CSS
- Framer Motion
- Radix UI
- Headless UI
- Lucide React

### State Management

- React Query

### Authentication

- KindeAuth

### Backend

- Prisma with PostgreSQL
- Stripe
- Uploadthing for image uploads
- Resend

### Dev Tools

- TypeScript
- ESLint
- Tailwind CSS

## Prerequisites

- Node.js >= 14.0.0
- PostgreSQL database

## Getting Started

1. Clone the repository:

    ```sh
    git clone https://github.com/your-username/casecobra.git
    cd casecobra
    ```

2. Install dependencies:

    ```sh
    npm install
    ```

3. Set up the PostgreSQL database:

    - Create a new PostgreSQL database.
    - Copy the `.env.example` file to `.env` and update the `DATABASE_URL` with your PostgreSQL connection string.

4. Generate Prisma Client:

    ```sh
    npx prisma generate
    ```

5. Run database migrations:

    ```sh
    npx prisma migrate dev
    ```

6. Start the development server:

    ```sh
    npm run dev
    ```

    The application will be available at [http://localhost:3000](http://localhost:3000).

## Scripts

- `dev`: Starts the development server.
- `build`: Builds the application for production.
- `start`: Starts the production server.
- `lint`: Runs ESLint to lint the codebase.

## Environment Variables

The project uses the following environment variables:

- `DATABASE_URL`: PostgreSQL connection string.
- `NEXT_PUBLIC_STRIPE_KEY`: Public Stripe API key.
- `STRIPE_SECRET_KEY`: Secret Stripe API key.
- `UPLOADTHING_KEY`: Key for Uploadthing API.
- `RESEND_API_KEY`: API key for Resend.

## Deployment

The application is hosted on Vercel at [http://xyz](http://xyz).

## Contact

For any inquiries, please contact [arifuddin.danin@gmail.com](mailto:arifuddin.danin@gmail.com).

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
