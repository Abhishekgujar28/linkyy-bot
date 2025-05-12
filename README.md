# Telegram Bot

A Telegram bot built with python-telegram-bot library.

## Deployment to Heroku

1. Create a new Heroku app:
```bash
heroku create your-app-name
```

2. Set up environment variables in Heroku:
```bash
heroku config:set TELEGRAM_BOT_TOKEN=your_bot_token
```

3. Deploy to Heroku:
```bash
git init
git add .
git commit -m "Initial commit"
git push heroku main
```

4. Scale the worker dyno:
```bash
heroku ps:scale worker=1
```

## Local Development

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Create a `.env` file with your bot token:
```
TELEGRAM_BOT_TOKEN=your_bot_token
```

3. Run the bot:
```bash
python Bot.py
```

## Environment Variables

- `TELEGRAM_BOT_TOKEN`: Your Telegram bot token from BotFather 