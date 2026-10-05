# RoasterLee Telegram Mini App

Configured owner Telegram ID: **401102212**
Bot username: **@roasterlee_bot**

## Included
- Private Telegram authentication
- Owner/staff approval
- BV55: Brazil 50% + Robusta Vietnam 50%
- LV55: Laos 50% + Robusta Vietnam 50%
- Customer orders
- Automatic bean requirements
- 6 kg roast-batch suggestions
- Pending / Done production status
- SQLite database

## Easiest deployment
1. Create a new web service on a Node/Docker hosting provider (Railway, Render, Fly.io, etc.).
2. Upload this project or connect a Git repository containing it.
3. Add an environment variable named `BOT_TOKEN` and paste your @roasterlee_bot token there. Do NOT put the token into source code or send it to other people.
4. Deploy. The host will give you an HTTPS URL such as `https://your-app.example.com`.
5. Open Telegram **@BotFather** → `/mybots` → choose **@roasterlee_bot** → **Bot Settings** → **Menu Button** (or configure Mini App) → enter the HTTPS URL from step 4.
6. Open @roasterlee_bot and launch its Mini App. Telegram ID 401102212 is already the owner.
7. A staff member opens the Mini App once. Their account appears as pending. Reopen/refresh your Owner app and press **Approve**.

## Important
Telegram Mini Apps must be served over HTTPS in production. Keep BOT_TOKEN secret. If the token is ever exposed, revoke/regenerate it in BotFather.

## Run locally (optional)
Install Node.js 20+, run `npm install`, set `DEV_MODE=true`, then `npm start`. Open http://localhost:3000. DEV_MODE bypasses Telegram authentication and must never be enabled on a public deployment.
