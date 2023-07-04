# Ignite Call Application

The Ignite Call application is a scheduling system built with Next.js, Prisma, and TypeScript. It allows users to register, set their availability, and allow others to schedule calls with them.

## Technologies Used

- **Next.js:** A React framework for building JavaScript applications. It is used for server-side rendering and generating static websites for React based web applications.

- **TypeScript:** A statically typed superset of JavaScript that adds optional types to the language. TypeScript speeds up your development experience by catching errors and providing fixes before you even run your code.

- **Prisma:** An open-source database toolkit. It replaces traditional ORMs and makes database access easy with an auto-generated and type-safe query builder that's tailored to your database schema.

- **Zod:** A library for creating, checking, and refining values of any type. It's used for form validation in this application.

- **React Hook Form:** A performant, flexible and extensible forms with easy-to-use validation.

## Database Schema

The application uses a MySQL database with the following tables:

- **User:** Stores user information including username, name, bio, email, avatar URL, and creation date.

- **Account:** Stores account information for each user.

- **Session:** Stores session information for each user.

- **UserTimeInterval:** Stores the time intervals for each user.

- **Scheduling:** Stores scheduling information for each user.

## Key Features

- **User Registration:** Users can register by providing their username, name, and other details.

- **User Profile Update:** Users can update their profile information.

- **Time Interval Selection:** Users can select their available time intervals.

- **Scheduling:** Other users can schedule a call with a registered user.

## Styling

The application uses the Ignite UI library for styling. Global styles are defined in the global.ts file.

## Authentication

The application uses NextAuth for authentication. The Prisma adapter is used to connect NextAuth with the Prisma Client.

## API Routes

The application uses Next.js API routes for server-side operations. For example, the *blocked-dates.api.ts* file handles fetching blocked dates for a user.
