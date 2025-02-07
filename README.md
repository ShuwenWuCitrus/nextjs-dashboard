# Issue Tracker

A modern issue tracking application built with Next.js 14, featuring server-side rendering, user authentication, and a responsive interface.

## Features

- Create, edit, and delete issues with real-time validation
- User authentication with Google OAuth
- Dashboard with issue statistics and status visualization
- Filter and manage issues by status (Open, In Progress, Closed)
- Responsive design optimized for all devices
- Issue assignment and user management
- Rich text descriptions with Markdown support

## Tech Stack

### Frontend

- Next.js 14 with App Router and Server Components
- TypeScript for type safety
- Radix UI components with Tailwind CSS
- Server-side rendering for optimal performance

### Backend

- MySQL database with Prisma ORM
- NextAuth.js for authentication
- RESTful API endpoints
- Secure data validation with Zod

## Getting Started

### Prerequisites

- Node.js 18+
- MySQL database
- Google OAuth credentials

### Installation

1. Clone the repository:

```bash
git clone https://github.com/ShuwenWuCitrus/nextjs-dashboard.git
cd nextjs-dashboard
```

2. Install dependencies:

```bash
npm install
```

3. Set up environment variables:

```bash
# Create a .env file with the following variables
DATABASE_URL="mysql://user:password@localhost:3306/issue_tracker"
GOOGLE_CLIENT_ID="your_google_client_id"
GOOGLE_CLIENT_SECRET="your_google_client_secret"
NEXTAUTH_URL="http://localhost:3000"
NEXTAUTH_SECRET="your_nextauth_secret"
```

4. Run database migrations:

```bash
npx prisma migrate dev
```

5. Start the development server:

```bash
npm run dev
```

## Architecture Highlights

- Server Components for efficient data fetching and rendering
- Type-safe database operations with Prisma ORM
- Secure authentication flow with NextAuth.js
- Modular component architecture for maintainability
- Responsive UI built with Radix UI primitives
- Form validation using Zod schema validation

## Database Schema

The application uses the following main models:

- **Issue:** Tracks individual issues with title, description, status, and assignee
- **User:** Stores user information and authentication details
- **Account:** Manages OAuth accounts
- **Session:** Handles user sessions

## API Routes

- `GET /api/issues` - Get all issues
- `POST /api/issues` - Create a new issue
- `PATCH /api/issues/:id` - Update an issue
- `DELETE /api/issues/:id` - Delete an issue
- `GET /api/users` - Get all users

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Next.js](https://nextjs.org/)
- [Prisma](https://www.prisma.io/)
- [NextAuth.js](https://next-auth.js.org/)
- [Radix UI](https://www.radix-ui.com/)
- [Tailwind CSS](https://tailwindcss.com/)

```

```
