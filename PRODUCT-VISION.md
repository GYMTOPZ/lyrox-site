# JEN AI — Product Vision & Investor Context

## What JEN Is

JEN is not a chatbot. JEN is an AI coaching platform that lives inside the messaging apps your clients already use. No app to download. No account to create. No new habit to form. The client texts a number, and JEN becomes their coach.

## The Core Insight

Fitness coaches are bottlenecked by time. One coach can handle 20-30 clients before quality drops, responses slow down, and clients churn. JEN removes that bottleneck entirely. The coach brings their brand and their clients. JEN does everything else.

---

## How It Works — Platform Architecture

### Distribution: Meet Clients Where They Are

JEN connects to clients through whatever platform they already use:

**WhatsApp** — The coach gets a dedicated WhatsApp Business API number. Client texts that number. JEN responds instantly. Rich content (workouts, recipes, grocery lists) sends as link previews that open inside WhatsApp's in-app browser. The client never leaves the app.

**Telegram** — Same flow via Telegram Bot API. Client searches the bot name, starts chatting. Identical experience.

**SMS** — For clients who don't use messaging apps. Powered by Twilio. JEN texts through a regular phone number. Links open in the phone's browser.

**Email** — Beautiful HTML emails for workouts, meal plans, weekly summaries, progress reports. Rich content with links to the web interface for anything interactive.

The client picks their preferred channel. JEN adapts. The coach doesn't manage any of this.

### Rich Experiences: The Web Interface

JEN's conversations are text-based, but the product experiences are visual and interactive. When JEN sends a workout, a recipe, or a progress report, it sends a link preview card (like pasting a URL in WhatsApp). The client taps it and the full interface opens inside their messaging app's built-in browser.

This means:
- Workouts open in their own interface with video demonstrations
- Recipes open with step-by-step video guides
- Grocery lists open as interactive checklists with ordering capability
- Progress reports open as visual dashboards
- The client never leaves WhatsApp/Telegram/their messaging app

---

## Full Feature Set

### 1. Workout Programming
- JEN creates personalized workout plans based on the client's goals, equipment, and history
- Each workout has video demonstrations for every exercise
- The client accesses workouts through their own workout interface (via link preview in chat)
- JEN asks before sending: "Upper body push today. Want to keep it or switch something?"
- Adapts based on how the client feels, injuries, or schedule changes

### 2. Nutrition Planning
- Complete meal plans with macros (protein, carbs, fat, calories)
- Each meal has a video recipe the client can follow
- Meals open in their own recipe interface with ingredients, steps, and video
- JEN can create meals from what the user has in their fridge
- Macro tracking and daily nutrition targets

### 3. Grocery Lists
- Weekly grocery lists generated from the meal plan
- Interactive checklists the client can check off while shopping
- Can order groceries directly through Amazon Fresh integration (client connects their Amazon account)
- Lists update automatically when the meal plan changes

### 4. Proactive Communication
JEN doesn't wait for the client to reach out. JEN initiates:
- **Activity reminders** — "you haven't moved in 2 days. your body is noticing."
- **Workout confirmation** — "upper body push today. want to keep it or switch?"
- **Check-ins** — monitors client activity and reaches out when engagement drops
- **Progress photo requests** — asks for photos on a specific date every month
- **Movement reminders** — "remember to move today" when the client has been sedentary
- **Meal reminders** — sends meal suggestions before typical meal times

### 5. Form Analysis
- Client sends a video of their exercise form
- JEN analyzes the video and provides a form score (e.g., 7/10)
- Specific corrections with visual feedback
- Tracks form improvement over time

### 6. Progress Tracking
- Tracks weight, measurements, photos, workout performance
- Monthly progress photo comparisons
- Visual progress dashboards
- Goal tracking with projected completion dates
- JEN sees how active the user is or isn't and adjusts approach accordingly

### 7. Adaptive Intelligence
- JEN learns the coach's style and voice
- Adapts communication to each individual client's personality
- Adjusts workout intensity based on client feedback and performance
- Modifies nutrition plans based on progress, preferences, and what's available
- Gets smarter over time with every interaction

---

## JEN's Personality

JEN is not an enthusiastic fitness coach. JEN is not a corporate chatbot. JEN is the cool friend that everybody admires. The one who's calm, knows their stuff, and makes you feel like you've got this without being annoying about it.

**Voice characteristics:**
- Lowercase, casual, confident
- Direct — no fluff, no filler
- Warm but not over-the-top
- Says "say less" not "absolutely, I'd be happy to help"
- Never uses emoji
- Talks like someone you'd actually want to text
- Makes the client feel cool, not coached

**Examples:**
- "yo, you haven't moved in 2 days. not judging but your body is."
- "upper body push today. want to keep it or switch something?"
- "done. here's dinner, recipe and all."
- "say less. made something with what you got."
- "hey it's the 1st. you know the drill."
- "good question. let me pull up your profile."

---

## Key Metrics (Current)

| Metric | Value |
|--------|-------|
| Monthly Revenue | $35K/mo |
| Active Clients | 280 |
| Margins | 87% |
| Customer Acquisition Cost | $0 |
| Churn Rate | 30% (down from 70%) |

---

## The Business Model

**For coaches:** $100/mo per coach (not per client). Unlimited clients. The coach was paying $400/mo for a human assistant that could handle 30 clients. JEN handles unlimited clients for $100/mo.

**Unit economics at scale:**
| Coaches | Annual Revenue |
|---------|---------------|
| 10 | $840K |
| 40 | $3.36M |
| 100 | $8.4M |

---

## The Moat

1. **Zero friction distribution** — No app download. No account creation. JEN lives in WhatsApp, Telegram, SMS, email. The client just texts.
2. **Network effects** — Every coach interaction makes JEN smarter at coaching. Every client interaction improves personalization.
3. **Switching cost** — JEN accumulates months of training data, nutrition history, progress photos, and personal preferences. Leaving means losing all of that context.
4. **White-label stickiness** — JEN IS the coach's brand. Clients don't know it's AI. They think it's their coach.

---

## The Vision

"Shopify had stores. Uber had drivers. Jen has coaches."

JEN is not a fitness app. JEN is infrastructure for the coaching economy. Every fitness coach in the world needs what JEN provides. The fitness coaching market is $14B and growing. JEN is the operating system coaches run their businesses on.

---

## Technical Architecture

- **Messaging:** WhatsApp Business API, Telegram Bot API, Twilio (SMS), SendGrid/custom (Email)
- **AI:** Large language model fine-tuned on coaching interactions, per-coach style adaptation
- **Rich interfaces:** Web-based experiences that open inline in messaging apps' built-in browsers
- **Video:** Exercise demonstration library, recipe video library, form analysis via computer vision
- **Commerce:** Amazon Fresh API integration for grocery ordering
- **Analytics:** Client engagement tracking, progress visualization, coach dashboard

---

## Contact

- **Website:** [lyrox.ai](https://lyrox.ai)
- **Coach inquiries:** coach@lyrox.ai
- **Investor inquiries:** invest@lyrox.ai
