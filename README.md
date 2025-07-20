# MyOKR - Objectives and Key Results Management Platform

A comprehensive web-based OKR management application with user authentication, organizational hierarchy, and progress tracking.

## Features

- **Authentication**: Secure login with Replit Auth
- **Organizational Hierarchy**: Organizations → Departments → Teams → Users
- **OKR Management**: Create, track, and manage objectives and key results
- **Progress Tracking**: Real-time progress updates and analytics
- **Modern UI**: Responsive design with Tailwind CSS and shadcn/ui components

## Tech Stack

- **Frontend**: React 18, TypeScript, Vite, Tailwind CSS
- **Backend**: Node.js, Express.js, TypeScript
- **Database**: PostgreSQL with Drizzle ORM
- **Authentication**: Replit Auth (OpenID Connect)
- **UI Components**: shadcn/ui with Radix UI primitives

## Prerequisites

- Node.js 18 or higher
- PostgreSQL database
- Replit account for authentication

## Environment Variables

Create a `.env` file with the following variables:

```env
DATABASE_URL=your_postgresql_connection_string
SESSION_SECRET=your_session_secret_key
REPL_ID=your_replit_id
ISSUER_URL=https://replit.com/oidc
REPLIT_DOMAINS=your_domain.com
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/myokr.git
cd myokr
```

2. Install dependencies:
```bash
npm install
```

3. Set up your environment variables in `.env`

4. Push database schema:
```bash
npm run db:push
```

5. Start the development server:
```bash
npm run dev
```

The application will be available at `http://localhost:5000`

## Deployment

### Option 1: Vercel (Recommended)

1. Fork this repository to your GitHub account
2. Connect your GitHub repository to Vercel
3. Add environment variables in Vercel dashboard
4. Deploy

### Option 2: Railway

1. Fork this repository
2. Connect to Railway
3. Add environment variables
4. Deploy

### Option 3: Heroku

1. Fork this repository
2. Create a Heroku app
3. Connect to your GitHub repository
4. Add environment variables
5. Deploy

## Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm run start` - Start production server
- `npm run db:push` - Push database schema changes

## License

MIT License
