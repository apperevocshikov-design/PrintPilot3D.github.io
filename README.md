# PrintPilot 3D Telegram Mini App

Production-ready frontend for a Telegram Mini App that calculates 3D printing quotes from STL, OBJ, 3MF and GCODE files.

## Run

```bash
npm install
npm run dev
```

## Build

```bash
npm run build
```

## Telegram bot setup

1. Deploy `dist/` to an HTTPS host.
2. Open BotFather and set the Mini App URL with `/setmenubutton` or create a Web App button.
3. Use the deployed URL as the Web App URL.
4. The app already loads `telegram-web-app.js`, calls `ready()` and `expand()`, and uses Telegram share/open-link APIs when available.

For backend order intake, listen to `web_app_data` in your bot and parse the JSON payload from the Mini App.
