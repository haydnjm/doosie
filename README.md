# AI Recipe Generator

A personalized recipe assistant that emails you three curated recipes every Saturday morning, helping you plan your weekly meals and generate shopping lists effortlessly.

## Pre-reqs
- [Supabase](https://supabase.com/) project for DB + auth
- [Resend](https://resend.com/) account for sending emails
- [Google Gemini API key](https://ai.google.dev/gemini-api/docs/quickstart) for recipe generation
- [Stability AI API key and credits](https://stability.ai/api) for image generation

## Features

- Automated weekly recipe suggestions
- Email delivery every Saturday morning
- App for managing shopping lists/viewing recipe instructions (TODO)

## Environment Variables

Create a `.env` file in the root directory with the following variables:

| Variable | Description | Required |
|----------|-------------|-----------|
| SUPABASE_URL | Your Supabase project URL | Yes |
| SUPABASE_SERVICE_API_KEY | Supabase service role API key | Yes |
| SUPABASE_ANON_API_KEY | Supabase anonymous API key | Yes |
| RESEND_API_KEY | API key for email service (Resend) | Yes |
| GEMINI_API_KEY | Google Gemini API key for AI features | Yes |
| STABILITY_API_KEY | Stability AI API key | Yes |
| TEST_RUN | Test environment flag | No |

## Setup

### 1. Install Dependencies

```bash
npm install
```

### 2. Create .env file

```bash
cp .env.example .env
```

### 3. Configure Supabase (for local dev)

```bash
supabase init
supabase start
```

### 4. Run the app

```bash
npm run start
```



# Todos:
- [ ] Front end which fetches shopping list
- [ ] Auth, multi-user lists