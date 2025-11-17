# 🚀 Deploy to Supabase - Complete Guide

## ✅ Prerequisites Checklist

- [ ] Supabase CLI installed (`npm install -g supabase`)
- [ ] GitHub repository cloned locally
- [ ] Supabase project created (Project ID: `osvudolcsmrxtvyufnil`)
- [ ] OpenAI API key ready

---

## 📦 Step 1: Clone Repository

```bash
git clone https://github.com/improvads13-wq/nuralife-ai-dietitian.git
cd nuralife-ai-dietitian
```

---

## 🔑 Step 2: Login to Supabase

```bash
npx supabase login
```

This will open your browser for authentication.

---

## 🔗 Step 3: Link to Your Project

```bash
npx supabase link --project-ref osvudolcsmrxtvyufnil
```

Enter your database password when prompted.

---

## 🗄️ Step 4: Run Database Migrations

```bash
# Create KV store table (required for backend)
npx supabase db push

# Or manually run migrations:
npx supabase db execute --file supabase/migrations/init.sql
npx supabase db execute --file supabase/migrations/onboarding_tables.sql
```

---

## 🌐 Step 5: Deploy Edge Function

**THIS IS THE CRITICAL STEP**

```bash
npx supabase functions deploy make-server-a2fc8e76
```

Expected output:
```
Deploying make-server-a2fc8e76 (project ref: osvudolcsmrxtvyufnil)
✓ Function deployed successfully
```

---

## 🔐 Step 6: Set Environment Variables

Set your OpenAI API key as a secret:

```bash
npx supabase secrets set OPENAI_API_KEY=your_openai_api_key_here
```

Verify:
```bash
npx supabase secrets list
```

---

## ✅ Step 7: Verify Deployment

Test the health endpoint:

```bash
curl https://osvudolcsmrxtvyufnil.supabase.co/functions/v1/make-server-a2fc8e76/health
```

Expected response:
```json
{"status":"ok","version":"1.1.4","timestamp":"2024-..."}
```

---

## 🎨 Step 8: Install Frontend Dependencies

```bash
npm install
```

---

## 🚀 Step 9: Start Development Server

```bash
npm run dev
```

Your app will be running at `http://localhost:5173`

---

## 🔧 Troubleshooting

### 404 Errors

If you see 404 errors:
1. Check if Edge Function is deployed: `npx supabase functions list`
2. Redeploy: `npx supabase functions deploy make-server-a2fc8e76`
3. Check logs: `npx supabase functions logs make-server-a2fc8e76`

### Database Connection Issues

```bash
# Check database status
npx supabase db status

# Reset if needed (⚠️ WARNING: This deletes all data)
npx supabase db reset
```

### Authentication Issues

1. Go to https://supabase.com/dashboard/project/osvudolcsmrxtvyufnil/auth/providers
2. Enable Email provider
3. Configure Google OAuth if needed

---

## 📊 Monitoring

View logs in real-time:

```bash
# Edge Function logs
npx supabase functions logs make-server-a2fc8e76 --follow

# Database logs
npx supabase db logs
```

---

## 🎉 Success!

Once all steps are complete, your NuraLife app should be fully functional with:
- ✅ Edge Functions deployed
- ✅ Database tables created
- ✅ Authentication working
- ✅ AI voice interactions enabled
- ✅ All 6 dashboards functional

Visit `http://localhost:5173` and create an account to get started!

---

## 📚 Additional Resources

- [Supabase CLI Documentation](https://supabase.com/docs/guides/cli)
- [Edge Functions Guide](https://supabase.com/docs/guides/functions)
- [NuraLife GitHub Repository](https://github.com/improvads13-wq/nuralife-ai-dietitian)
