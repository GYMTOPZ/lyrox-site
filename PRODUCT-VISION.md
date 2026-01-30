# Lyrox — Product Vision & Investor Context

## What Lyrox Is

Lyrox is not a chatbot. Lyrox is an AI coaching platform that lives inside the messaging apps your clients already use. No app to download. No account to create. No new habit to form. The client texts a number, and Lyrox becomes their coach.

## The Core Insight

Fitness coaches are bottlenecked by time. One coach can handle 20-30 clients before quality drops, responses slow down, and clients churn. Lyrox removes that bottleneck entirely. The coach brings their brand and their clients. Lyrox does everything else.

---

## How It Works — Platform Architecture

### Distribution: Meet Clients Where They Are

Lyrox connects to clients through whatever platform they already use:

**WhatsApp** — The coach gets a dedicated WhatsApp Business API number. Client texts that number. Lyrox responds instantly. Rich content (workouts, recipes, grocery lists) sends as link previews that open inside WhatsApp's in-app browser. The client never leaves the app.

**Telegram** — Same flow via Telegram Bot API. Client searches the bot name, starts chatting. Identical experience.

**SMS** — For clients who don't use messaging apps. Powered by Twilio. Lyrox texts through a regular phone number. Links open in the phone's browser.

**Email** — Beautiful HTML emails for workouts, meal plans, weekly summaries, progress reports. Rich content with links to the web interface for anything interactive.

The client picks their preferred channel. Lyrox adapts. The coach doesn't manage any of this.

### Rich Experiences: The Web Interface

Lyrox's conversations are text-based, but the product experiences are visual and interactive. When Lyrox sends a workout, a recipe, or a progress report, it sends a link preview card (like pasting a URL in WhatsApp). The client taps it and the full interface opens inside their messaging app's built-in browser.

This means:
- Workouts open in their own interface with video demonstrations
- Recipes open with step-by-step video guides
- Grocery lists open as interactive checklists with ordering capability
- Progress reports open as visual dashboards
- The client never leaves WhatsApp/Telegram/their messaging app

---

## Full Feature Set

### 1. Workout Programming
- Lyrox creates personalized workout plans based on the client's goals, equipment, and history
- Each workout has video demonstrations for every exercise
- The client accesses workouts through their own workout interface (via link preview in chat)
- Lyrox asks before sending: "Upper body push today. Want to keep it or switch something?"
- Adapts based on how the client feels, injuries, or schedule changes

### 2. Nutrition Planning
- Complete meal plans with macros (protein, carbs, fat, calories)
- Each meal has a video recipe the client can follow
- Meals open in their own recipe interface with ingredients, steps, and video
- Lyrox can create meals from what the user has in their fridge
- Macro tracking and daily nutrition targets

### 3. Grocery Lists
- Weekly grocery lists generated from the meal plan
- Interactive checklists the client can check off while shopping
- Can order groceries directly through Amazon Fresh integration (client connects their Amazon account)
- Lists update automatically when the meal plan changes

### 4. Proactive Communication
Lyrox doesn't wait for the client to reach out. Lyrox initiates:
- **Activity reminders** — "you haven't moved in 2 days. your body is noticing."
- **Workout confirmation** — "upper body push today. want to keep it or switch?"
- **Check-ins** — monitors client activity and reaches out when engagement drops
- **Progress photo requests** — asks for photos on a specific date every month
- **Movement reminders** — "remember to move today" when the client has been sedentary
- **Meal reminders** — sends meal suggestions before typical meal times

### 5. Form Analysis
- Client sends a video of their exercise form
- Lyrox analyzes the video and provides a form score (e.g., 7/10)
- Specific corrections with visual feedback
- Tracks form improvement over time

### 6. Progress Tracking
- Tracks weight, measurements, photos, workout performance
- Monthly progress photo comparisons
- Visual progress dashboards
- Goal tracking with projected completion dates
- Lyrox sees how active the user is or isn't and adjusts approach accordingly

### 7. Adaptive Intelligence
- Lyrox learns the coach's style and voice
- Adapts communication to each individual client's personality
- Adjusts workout intensity based on client feedback and performance
- Modifies nutrition plans based on progress, preferences, and what's available
- Gets smarter over time with every interaction

---

## Lyrox's Personality

Lyrox is not an enthusiastic fitness coach. Lyrox is not a corporate chatbot. Lyrox is the cool friend that everybody admires. The one who's calm, knows their stuff, and makes you feel like you've got this without being annoying about it.

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

### Demo Conversation — "3 Months In"

The landing page chat demo shows a real relationship, not a first interaction. This is what Lyrox looks like when it already knows someone — their sleep, their knee injury, their taste, their goals. The conversation flows through a single day:

**1. Morning — Lyrox initiates with context**
> "morning. you slept 5 hours last night so i made today's workout lighter. your knee has been feeling better so i added goblet squats back in."
> [Link Preview: Lower Body (Light) — 4 exercises · video demos · 40 min · adjusted for recovery → lyrox.ai/workout]

**2. Real life — dinner at a restaurant**
> Client: "going out to dinner tonight at nobu. what should i order"
> "get the black cod miso. 38P, 12C, 22F. skip the rice, get the edamame side instead. that keeps you under your macros and you still enjoy it."

**3. Bad day — Lyrox adapts everything**
> Client: "honestly i feel like crap today"
> "yeah 5 hours of sleep will do that. skip the gym, go for a 20 min walk instead. i adjusted your meals for today too, a little more carbs to keep your energy up."
> [Link Preview: Today's Adjusted Meals — 3 meals · higher carbs · comfort food that still works → lyrox.ai/meals]

**4. Fridge situation — makes a meal from what's available**
> Client: "only have eggs and some leftover chicken"
> "that's enough. made you something quick."
> [Link Preview: Chicken Egg Scramble — 41P · 3C · 18F · 340 cal · video recipe 1:20 → lyrox.ai/meal]

**5. Proactive groceries with ordering**
> "by the way you're running low on groceries. here's this week's list, you can order straight from there."
> [Link Preview: Weekly Groceries — 9 items · order on amazon · estimated $47 → lyrox.ai/groceries]

**6. Progress reveal — Lyrox brings it up because it's time**
> "hey it's been 3 months. look at this."
> [Link Preview: Your 3-Month Progress — down 11 lbs · squat 95 to 155 · waist down 2 inches → lyrox.ai/progress]
> Client: "wow i didn't even realize"
> "that's the point. you just showed up and it happened. keep going, you're halfway there."

**Why this conversation works:**
- Lyrox initiates, not the client. It's proactive, not reactive.
- It knows context without being told (sleep data, knee history, grocery levels).
- It adapts the entire day when the client feels bad — not just one thing.
- Rich content (workouts, meals, groceries, progress) shows as link preview cards that open in full interfaces, not walls of text in chat.
- The personality is a cool friend, not an enthusiastic coach. Lowercase, no emoji, direct.
- The white-label demo shows "Coach Emilio" — clients think they're talking to their coach, not to Lyrox.

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

**For coaches:** $100/mo per coach (not per client). Unlimited clients. The coach was paying $400/mo for a human assistant that could handle 30 clients. Lyrox handles unlimited clients for $100/mo.

**Unit economics at scale:**
| Coaches | Annual Revenue |
|---------|---------------|
| 10 | $840K |
| 40 | $3.36M |
| 100 | $8.4M |

---

## The Moat

1. **Zero friction distribution** — No app download. No account creation. Lyrox lives in WhatsApp, Telegram, SMS, email. The client just texts.
2. **Network effects** — Every coach interaction makes Lyrox smarter at coaching. Every client interaction improves personalization.
3. **Switching cost** — Lyrox accumulates months of training data, nutrition history, progress photos, and personal preferences. Leaving means losing all of that context.
4. **White-label stickiness** — Lyrox IS the coach's brand. Clients don't know it's AI. They think it's their coach.

---

## The Vision

"Shopify had stores. Uber had drivers. Lyrox has coaches."

Lyrox is not a fitness app. Lyrox is infrastructure for the coaching economy. Every fitness coach in the world needs what Lyrox provides. The fitness coaching market is $14B and growing. Lyrox is the operating system coaches run their businesses on.

---

## What People Dream Of — The Roadmap

These are the things every person wishes their coach could do. Some Lyrox already does. The rest is the roadmap.

### Already Built
- **"Just tell me what to do"** — Wake up, everything is ready. Workout, food, grocery list. No decisions.
- **"Know me without me explaining"** — Lyrox remembers everything. Bad knee, hated exercises, stressful days, travel schedule. Never forgets.
- **"Catch me before I fall off"** — Lyrox notices when you stop engaging. Reaches out proactively, not with guilt but with an easy alternative.
- **"Be available when I need you"** — 2 AM food anxiety. Sunday night meal prep. Right after a bad workout. Lyrox is there at that exact moment.
- **"Don't make me feel stupid"** — Explains things like a friend, not a textbook. Never condescending.
- **"Show me I'm making progress"** — Visual proof. Weight, measurements, photos, performance tracking. Monthly comparisons.
- **"Create meals from what I have"** — Tell Lyrox what's in your fridge, get a meal with macros and a video recipe.

### Building Next
- **"What can I eat at this restaurant?"** — Send Lyrox the menu (or just the restaurant name), Lyrox picks the best option for your macros.
- **"I feel like garbage today"** — Lyrox adjusts the entire day automatically. Lighter workout. Comfort food that still hits macros. Check-in later.
- **"My wedding is in 8 weeks"** — Lyrox builds an 8-week plan backward from any target date. Reverse-engineers the timeline.
- **"I want to look like this"** — Send a reference photo. Lyrox estimates the body fat difference and builds a realistic timeline with milestones.
- **Sleep tracking integration** — Lyrox reads your sleep data. Slept 4 hours? Workout intensity drops automatically. No questions asked.
- **Wearable data (Apple Watch, Garmin, Whoop)** — Heart rate, steps, recovery score, stress levels. Lyrox adapts everything in real time based on your body's actual state.
- **Location-aware coaching** — Traveling? Lyrox detects your location, sends hotel room workouts and nearby restaurant options that fit your macros.
- **Period/cycle tracking** — Lyrox adjusts workout intensity and nutrition around hormonal cycles. No awkwardness, just smart adaptation.
- **Sick day / kids sick / life happens** — Lyrox detects schedule disruption and automatically pivots. No-equipment home workout. Simpler meals. Zero guilt.

### The Dream (Future)
- **Voice coaching** — Lyrox talks to you during workouts through your earbuds. Counts reps, cues form, adjusts rest periods in real time.
- **Smart scale integration** — Step on the scale, data goes straight to Lyrox. Trends, not daily fluctuations.
- **Social accountability** — Optional: Lyrox connects you with others on similar journeys. Not a social network. Just knowing someone else is grinding too.
- **Coach dashboard** — The coach sees everything. Every client's progress, engagement, risk of churning. Lyrox flags who needs human attention.

---

## Is Coaching About to Die?

No. Coaching is about to split.

Every coaching relationship has two parts: the **human part** (empathy, motivation, accountability, the feeling that someone believes in you) and the **execution part** (programming workouts, calculating macros, answering questions at 2 AM, sending reminders, tracking progress, adjusting plans).

The human part is irreplaceable. No AI will ever replicate the feeling of your coach texting you after a bad day because they genuinely care. That's why clients pay. That's why they stay.

The execution part is a bottleneck. It's repetitive, time-consuming, and it's the reason coaches cap out at 20-30 clients. It's the reason they burn out. It's the reason they quit.

**Lyrox handles the execution.** All of it. 24/7. Instantly. Perfectly. The coach keeps the human part — the relationship, the brand, the trust. But now they can have that relationship with 100 clients instead of 25.

### What This Actually Means

Coaching isn't dying. It's becoming **scalable**.

Before Lyrox, coaching was a job. You traded time for money. More clients meant more hours, worse quality, and eventually burnout. The ceiling was your calendar.

After Lyrox, coaching is a **business**. The coach is the CEO. They set the vision, build their brand, acquire clients. Lyrox runs the operation. The ceiling is gone.

This is the same pattern that played out in every industry that got automated at the execution layer:

- **Shopify** didn't kill retail. It turned shopkeepers into e-commerce entrepreneurs.
- **Uber** didn't kill driving. It turned car owners into business operators.
- **Canva** didn't kill design. It turned everyone into a designer.

Lyrox doesn't kill coaching. It turns coaches into business owners who happen to use AI as their operating system.

### The Market Shift

The fitness coaching market is $14B and growing. But the vast majority of coaches never scale past $5K/month because they physically can't handle more clients. They're selling their time, not their expertise.

Lyrox unlocks the other 80% of that market — the coaches who have the knowledge and the brand but not the bandwidth. Give them Lyrox, and a $5K/month coach becomes a $20K/month business.

### Why Now

Three things converged:

1. **AI is finally good enough.** Large language models can hold nuanced, personalized conversations that feel human. Two years ago this wasn't possible.
2. **Messaging is universal.** WhatsApp has 2B users. Everyone already knows how to text. Zero friction.
3. **Coaches are desperate.** The creator economy exploded. There are more fitness coaches than ever, and they're all drowning in the same operational bottleneck.

The timing isn't early. The timing is now.

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
