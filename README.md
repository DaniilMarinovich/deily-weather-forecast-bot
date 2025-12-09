# 🌤️ Daily Weather Forecast Bot

A Telegram bot built with Node.js and TypeScript that sends current weather forecasts and daily automatic updates to subscribed users.

## 🚀 Features
- **Instant Forecast:** Get real-time weather data using the `/weather` command.
- **Daily Scheduler:** Automatically sends weather reports at a specific time (powered by `node-cron`).
- **User Management:** Stores user preferences and chat IDs in MongoDB.
- **Type Safety:** Written in TypeScript for reliable code.

## 🛠️ Tech Stack
- **Runtime:** Node.js
- **Language:** TypeScript
- **Database:** MongoDB (via Mongoose)
- **Libraries:**
  - `node-telegram-bot-api` (Telegram interaction)
  - `axios` (Weather API requests)
  - `node-cron` (Task scheduling)
  - `express` (Server/Health check)

## ⚙️ Installation & Setup

### 1. Prerequisites
Ensure you have **Node.js** and **npm** installed. You will also need a running MongoDB instance (local or Atlas).

### 2. Clone the repository
```bash
git clone [https://github.com/DaniilMarinovich/daily-weather-forecast-bot.git](https://github.com/DaniilMarinovich/daily-weather-forecast-bot.git)
cd daily-weather-forecast-bot
```

### 3. Install dependencies
```bash
npm install
```

### 4. Configuration
Create a `.env` file in the root directory and fill in your credentials:
```bash
BOT_TOKEN=your_telegram_bot_token_from_botfather
WEATHER_API_KEY=your_openweathermap_api_key
MONGO_URI=mongodb://localhost:27017/weather-bot
```
Note: If you use MongoDB Atlas, replace the MONGO_URI with your connection string.

### 5. Build the project
Compile the TypeScript code into JavaScript (the output will be in the dist/ folder):
```bash
npm run build
```

### 6. Run the bot
Start the production server:
```bash
npm start
```

### 📂 Project Structure
`
├── src/
│   ├── index.ts       # Entry point
│   ├── models/        # Mongoose schemas (User, etc.)
│   └── ...
├── dist/              # Compiled JavaScript (generated after build)
├── .env               # Environment variables
├── package.json       # Dependencies and scripts
└── tsconfig.json      # TypeScript configuration
`
### 📝 License

This project is licensed under the MIT License.
