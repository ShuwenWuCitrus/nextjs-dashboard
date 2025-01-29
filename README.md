# Issue Tracker

A modern issue tracking application built with Next.js 14, featuring real-time updates, user authentication, and a clean, responsive interface.

## Features

- 📝 Create, edit, and delete issues
- 👥 User authentication with Google
- 📊 Dashboard with issue statistics and charts
- 🔍 Filter issues by status (Open, In Progress, Closed)
- 📱 Responsive design for all devices
- 👤 Assign issues to users
- 📝 Rich text editing with Markdown support
- ⚡ Real-time updates with React Query
- 🎨 Modern UI with Radix UI and Tailwind CSS

## Tech Stack

- **Framework:** Next.js 14
- **Database:** MySQL with Prisma ORM
- **Authentication:** NextAuth.js with Google provider
- **Styling:** Tailwind CSS + Radix UI
- **Charts:** Recharts
- **Forms:** React Hook Form + Zod validation
- **API:** REST API with Next.js API routes
- **State Management:** React Query
- **Markdown:** React Markdown + SimpleMDE editor

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
