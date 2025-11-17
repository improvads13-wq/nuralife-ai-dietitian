# NuraLife - Complete File Manifest

## Project Structure Overview

This document lists all files in the NuraLife AI Dietitian project organized by directory.

### Root Configuration Files
- package.json
- tsconfig.json
- vite.config.ts
- .gitignore
- index.html
- main.tsx
- App.tsx

### Deployment & Documentation
- README.md
- DEPLOY_TO_SUPABASE.md
- Attributions.md

### Styles
- styles/globals.css

### Utils Directory (18+ files)
- utils/auth.ts
- utils/ai-service.ts
- utils/database.ts
- utils/medical-api.ts
- utils/medical-dashboard-data.ts
- utils/GlobalVoiceSession.tsx
- utils/NuraLifeAgentProfiles.ts
- utils/RealtimeConnection.ts
- utils/RealtimeVoiceAgent.tsx
- utils/useVoiceSubtitles.tsx
- utils/dashboard/updateDashboardState.ts
- utils/onboarding/mapping.ts
- utils/supabase/client.ts
- utils/supabase/info.tsx

### Components Directory (64+ files)
#### Main Components
- components/Dashboard.tsx
- components/ChatInterface.tsx
- components/OnboardingFlow.tsx
- components/SignInScreen.tsx
- components/SignUpScreen.tsx
- components/ReportsTab.tsx
- components/SettingsTab.tsx
- components/GlobalOrbVoiceLayer.tsx
- components/PageTransition.tsx

#### Dashboard Components (6 AI Dashboards)
- components/WeightLossDashboard.tsx
- components/NutritionistDashboard.tsx
- components/MentalHealthDashboard.tsx
- components/PersonalCareDashboard.tsx
- components/RelationshipsDashboard.tsx
- components/MedicalCareDashboard.tsx

#### Tab Components
- components/NutritionistTabs.tsx
- components/MentalHealthTabs.tsx
- components/PersonalCareTabs.tsx
- components/Dashboard_ToggleBar_MedicalCare_v2.tsx
- components/Dashboard_ToggleBar_MentalHealth_v2.tsx
- components/Dashboard_ToggleBar_Nutritionist_v2.tsx
- components/Dashboard_ToggleBar_PersonalCare_v2.tsx
- components/Dashboard_ToggleBar_Relationships_v2.tsx

#### Utility Components
- components/AICompanionCarousel.tsx
- components/ActivityTimeline.tsx
- components/AmoebaOrb.tsx
- components/AmoebaOrb_StaticAura.tsx
- components/BrandingFooter.tsx
- components/ClearSessionButton.tsx
- components/ConfettiEffect.tsx
- components/DailyCheckIn.tsx
- components/DashboardContent.tsx
- components/DeploymentBanner.tsx
- components/HealthScoreRing.tsx
- components/InsightCard.tsx
- components/MealLoggingModal.tsx
- components/MiniChart.tsx
- components/MoodOrb.tsx
- components/NuraStream.tsx
- components/OnboardingQA.tsx
- components/ProgressRing.tsx
- components/QuickActionButtons.tsx
- components/QuickActionCard.tsx
- components/RecommendedActivities.tsx
- components/ScrollSelector.tsx
- components/StreakTracker.tsx
- components/SupabaseDebugger.tsx
- components/TaskCard.tsx
- components/TodaysFocus.tsx
- components/VoiceCard.tsx
- components/VoiceFeaturesBanner.tsx
- components/WelcomeScreen.tsx
- components/WordBurstSubtitle.tsx

#### Chat/Voice Components
- components/ChatScreen_v4.tsx
- components/UniversalChatScreen_v3.tsx
- components/VoiceChatScreen_v2.tsx

#### Figma Components
- components/figma/ImageWithFallback.tsx

#### UI Components (shadcn/ui - 42+ files)
- components/ui/accordion.tsx
- components/ui/alert-dialog.tsx
- components/ui/alert.tsx
- components/ui/aspect-ratio.tsx
- components/ui/avatar.tsx
- components/ui/badge.tsx
- components/ui/breadcrumb.tsx
- components/ui/button.tsx
- components/ui/calendar.tsx
- components/ui/card.tsx
- components/ui/carousel.tsx
- components/ui/chart.tsx
- components/ui/checkbox.tsx
- components/ui/collapsible.tsx
- components/ui/command.tsx
- components/ui/context-menu.tsx
- components/ui/dialog.tsx
- components/ui/drawer.tsx
- components/ui/dropdown-menu.tsx
- components/ui/form.tsx
- components/ui/hover-card.tsx
- components/ui/input-otp.tsx
- components/ui/input.tsx
- components/ui/label.tsx
- components/ui/menubar.tsx
- components/ui/navigation-menu.tsx
- components/ui/pagination.tsx
- components/ui/popover.tsx
- components/ui/progress.tsx
- components/ui/radio-group.tsx
- components/ui/resizable.tsx
- components/ui/scroll-area.tsx
- components/ui/select.tsx
- components/ui/separator.tsx
- components/ui/sheet.tsx
- components/ui/sidebar.tsx
- components/ui/skeleton.tsx
- components/ui/slider.tsx
- components/ui/sonner.tsx
- components/ui/switch.tsx
- components/ui/table.tsx
- components/ui/tabs.tsx
- components/ui/textarea.tsx
- components/ui/toggle-group.tsx
- components/ui/toggle.tsx
- components/ui/tooltip.tsx
- components/ui/use-mobile.ts
- components/ui/utils.ts

### Supabase Backend
#### Edge Functions
- supabase/functions/make-server-a2fc8e76/index.ts
- supabase/functions/make-server-a2fc8e76/kv_store.ts

#### Server Modules
- supabase/functions/server/index.tsx
- supabase/functions/server/auth.ts
- supabase/functions/server/onboarding.ts
- supabase/functions/server/ai-service.ts
- supabase/functions/server/medical-care.ts
- supabase/functions/server/openai-realtime.ts
- supabase/functions/server/kv_store.tsx

#### Migrations
- supabase/migrations/init.sql
- supabase/migrations/onboarding_tables.sql
- supabase/migrations/verify_onboarding.sql

### Shell Scripts
- deploy-edge-function.sh
- test-edge-function.sh

---

## Total File Count
- **Configuration**: 6 files
- **Documentation**: 3+ files
- **Styles**: 1 file
- **Utils**: 14+ files
- **Components**: 64+ files
- **Backend**: 10 files
- **Migrations**: 3 files
- **Scripts**: 2 files

**Grand Total: 100+ project files**

---

_Last updated: 2025-11-17_
