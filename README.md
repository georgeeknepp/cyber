## Telegram Bot Template for Vercel

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2FPonomareVlad%2FTeleVercelBot&env=TELEGRAM_BOT_TOKEN&envDescription=Telegram%20Bot%20Token%20from%20%40BotFather&project-name=telegram-bot&repo-name=telegram-bot)

### Run locally

#### 1. Install [Vercel CLI](https://vercel.com/docs/cli)

```bash
npm i -g vercel
```

#### 2. Install [VK Tunnel](https://dev.vk.com/libraries/tunnel)

```bash
npm i -g @vkontakte/vk-tunnel
```

#### 3. Then run local dev server with tunnel

```bash
npm run dev-with-tunnel
```

And open link from terminal (ends with `*.wormhole.vk-apps.com`) to set WebHook

Now you can make some changes in [bot.mjs](bot.mjs)

[Documentation for TeleBot](https://github.com/mullwar/telebot)

### Template structure:

- [api/telegram.mjs](api/telegram.mjs) — Endpoint function for WebHooks
- [api/setWebhook.mjs](api/setWebhook.mjs) — Function for setting WebHook URL

###### P.S. Don't forget to remove or restrict [api/setWebhook.mjs](api/setWebhook.mjs) function before going to production
