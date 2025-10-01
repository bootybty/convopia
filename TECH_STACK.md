# Convopia - Tech Stack

## Frontend
- **Next.js 15.5** (App Router, React Server Components)
- **React 19** (latest)
- **TypeScript** (strict mode)
- **Tailwind CSS** (utility-first styling)
- **shadcn/ui** (component library - copy-paste, not dependency)

## Backend
- **Next.js Server Actions** (form handling, mutations)
- **Next.js API Routes** (REST endpoints when needed)

## Database & Backend Services
- **Supabase**
  - PostgreSQL database
  - Authentication (social logins, email/password)
  - Storage (file uploads, screenshots)
  - Real-time subscriptions (live updates)
  - Row Level Security (privacy controls)
  - Full-text search (built-in Postgres)
  - pgvector (semantic search med AI embeddings)

## Hosting & Deployment
- **Vercel**
  - Auto-scaling
  - Edge Functions
  - Edge Runtime support
  - Zero-config deployment
  - Built-in analytics

## Development Tools
- **TypeScript** (type-safety across stack)
- **Supabase CLI** (local development, migrations)
- **Prisma** eller **Drizzle ORM** (optional - hvis vi vil have type-safe queries udover Supabase client)
- **ESLint + Prettier** (code quality)

## Future Considerations
- **Meilisearch/Typesense** (hvis Supabase search ikke er nok ved scale)
- **Sentry** (error tracking)
- **Posthog** (analytics & feature flags)
- **Vercel AI SDK** (hvis vi skal integrere AI features)

## Why This Stack?
- ✅ **SEO-optimized** (Next.js SSR critical for discoverability)
- ✅ **Real-time ready** (Supabase subscriptions for live feeds)
- ✅ **Type-safe** (TypeScript + Supabase generated types)
- ✅ **Scalable** (handles millions of conversations)
- ✅ **Modern DX** (Turbopack, hot reload, shadcn components)
- ✅ **Cost-effective** (generous free tiers to start)
- ✅ **AI-ready** (pgvector for semantic search)
- ✅ **2025-proof** (cutting edge, industry standard tools)
