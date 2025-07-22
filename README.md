# Converso - AI Teaching Platform

A real-time AI-powered learning platform that creates personalized educational companions for interactive voice-based learning sessions.
> Build custom AI tutors with different voices, teaching styles, and subjects to enhance your learning experience through natural conversations.

## Features

- **AI Learning Companions** - Create personalized AI tutors for various subjects
- **Real-time Voice Conversations** - Interactive voice sessions with AI companions using Vapi
- **Multi-subject Support** - Math, Science, Language, History, Coding, Economics, and more
- **User Authentication** - Secure login with Clerk (Google OAuth support)
- **Companion Management** - Create, bookmark, and organize learning companions
- **Session Tracking** - Track learning progress and session history
- **Subscription Plans** - Tiered access with companion limits and premium features
- **Responsive Design** - Mobile-friendly interface with Tailwind CSS
- **Voice Customization** - Choose between male/female voices with casual/formal styles

## Tech Stack

- **Frontend**: Next.js 15, React 19, TypeScript
- **Styling**: Tailwind CSS, Radix UI components
- **Authentication**: Clerk
- **Database**: Supabase (PostgreSQL)
- **Voice AI**: Vapi.ai (real-time voice conversations)
- **Form Handling**: React Hook Form with Zod validation
- **Animations**: Lottie React
- **Monitoring**: Sentry
- **Deployment**: Vercel-ready

## Installation

```bash
# Clone the repository
git clone https://github.com/hayashi13597/lms-saas-app.git
cd lms-saas-app

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Fill in your API keys and configuration

# Run the development server
npm run dev
```

## Environment Setup

Create a `.env.local` file with the following variables:

```env
# Clerk Authentication
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=your_clerk_publishable_key
CLERK_SECRET_KEY=your_clerk_secret_key
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_IN_FALLBACK_REDIRECT_URL=/
NEXT_PUBLIC_CLERK_SIGN_UP_FALLBACK_REDIRECT_URL=/

# Supabase Database
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key

# Vapi Voice AI
NEXT_PUBLIC_VAPI_WEB_TOKEN=your_vapi_token

# Sentry Monitoring
SENTRY_AUTH_TOKEN=your_sentry_token
```

## Project Structure

```
├── app/                    # Next.js app router pages
│   ├── companions/         # Companion library and sessions
│   ├── my-journey/         # User dashboard and progress
│   └── subscription/       # Pricing and plans
├── components/             # Reusable UI components
├── lib/                    # Utilities and database actions
├── types/                  # TypeScript type definitions
├── constants/              # App constants and configuration
└── public/                 # Static assets
```

## Demo

[Live Demo](https://lms-saas-app-six.vercel.app/)

## Key Features Explained

- **Companion Builder**: Create AI tutors with custom names, subjects, topics, voices, and teaching styles
- **Voice Sessions**: Real-time conversations with AI using speech-to-text and text-to-speech
- **Progress Tracking**: Monitor learning sessions and companion usage
- **Bookmarking**: Save favorite companions for quick access
- **Search & Filter**: Find companions by subject, topic, or keywords


## License

This project is licensed under the MIT License.
