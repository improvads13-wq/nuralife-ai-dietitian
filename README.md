# 🌿 NuraLife - AI-Powered Wellness Companion

**A fully interactive, mobile-first AI dietitian and wellness app featuring realtime voice interaction, emotional intelligence, and beautiful glassmorphism design.**

![NuraLife Banner](https://via.placeholder.com/1200x400/5EEAD4/FFFFFF?text=NuraLife+AI+Wellness)

---

## ✨ Features

### 🎯 Six AI-Powered Wellness Dashboards
- **Weight Loss** (Vita) - Fitness tracking, meal planning, workout schedules
- **Nutritionist** (Nourish) - Nutrition insights, macro tracking, recipe suggestions
- **Mental Health** (Zen) - Mood tracking, mindfulness exercises, stress management
- **Personal Care** (Lumina) - Self-care routines, sleep tracking, skincare
- **Relationships** (Harmony) - Communication insights, relationship wellness
- **Medical Care** (Pulse) - Health metrics, medication reminders, symptom tracking

### 🎙️ Realtime Voice Interaction
- OpenAI Realtime API integration
- Natural voice conversations with AI companions
- Multiple voice accents and languages
- Dictation powered by OpenAI Whisper
- Voice choice persistence

### 🔐 Complete Authentication System
- Email/password signup and signin
- Google OAuth integration
- Password reset functionality
- Protected routes and session management
- Comprehensive error handling

### 🎨 Beautiful Design System
- **Apple Health meets Pixar** aesthetic
- Warm aqua-mint gradients with lavender glows
- Glassmorphism effects throughout
- Mood-adaptive orb system
- Floating glimmer particle effects
- Smooth animations with Motion (Framer Motion)

### 💾 Full Backend Integration
- Supabase Edge Functions
- PostgreSQL database with KV store
- User data persistence
- Dashboard state management
- Medication tracking
- Symptom scanner with AI triage
- Medical reports upload

---

## 🚀 Quick Start

See [DEPLOY_TO_SUPABASE.md](./DEPLOY_TO_SUPABASE.md) for complete deployment instructions.

```bash
# Clone repository
git clone https://github.com/improvads13-wq/nuralife-ai-dietitian.git
cd nuralife-ai-dietitian

# Install dependencies
npm install

# Deploy Edge Functions (CRITICAL STEP)
npx supabase link --project-ref osvudolcsmrxtvyufnil
npx supabase functions deploy make-server-a2fc8e76

# Set OpenAI API key
npx supabase secrets set OPENAI_API_KEY=your_key_here

# Start development server
npm run dev
```

Visit `http://localhost:5173`

---

## 📁 Project Structure

```
nuralife-ai-dietitian/
├── supabase/
│   ├── functions/
│   │   ├── make-server-a2fc8e76/     ← Main Edge Function
│   │   │   ├── index.ts              ← API endpoints
│   │   │   └── kv_store.ts           ← Database utilities
│   │   └── server/                   ← Modular backend
│   │       ├── index.tsx
│   │       ├── auth.ts
│   │       ├── onboarding.ts
│   │       ├── ai-service.ts
│   │       ├── medical-care.ts
│   │       ├── openai-realtime.ts
│   │       └── kv_store.tsx
│   └── migrations/
│       ├── init.sql
│       ├── onboarding_tables.sql
│       └── verify_onboarding.sql
├── components/                       ← React components (64 files)
├── utils/                            ← Utilities and helpers
├── styles/globals.css                ← Design system
├── App.tsx                           ← Main app
└── package.json
```

---

## 🔧 Technology Stack

### Frontend
- **React 18** - UI framework
- **TypeScript** - Type safety
- **Tailwind CSS 4** - Styling
- **Motion (Framer Motion)** - Animations
- **Lucide React** - Icons
- **shadcn/ui** - Component library
- **Recharts** - Data visualization

### Backend
- **Supabase** - Backend as a Service
  - Authentication
  - PostgreSQL Database
  - Edge Functions (Deno runtime)
  - Row Level Security
- **Hono** - Web server framework
- **OpenAI API**
  - GPT-4o-mini for text responses
  - Whisper for speech-to-text
  - Realtime API for voice conversations

---

## 📄 License

MIT License - feel free to use this project for personal or commercial purposes.

---

## 🙏 Acknowledgments

- Built with [Figma Make](https://figma.com)
- UI components from [shadcn/ui](https://ui.shadcn.com)
- Powered by [Supabase](https://supabase.com)
- AI by [OpenAI](https://openai.com)

---

**🌟 If you find this project helpful, please give it a star!**
