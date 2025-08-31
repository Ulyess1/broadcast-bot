# Discord Broadcast Bot

A Discord bot that allows server owners to **broadcast messages via DM** to their server members.  
Built with **discord.js** and **express.js**.

---

## 🚀 Features
- Broadcast (`!bc`) command with options:
  - 🟢 Send to **only online members**
  - 🟠 Send to **members with a specific role**
  - 🔵 Send to **all members**
  - ❌ Cancel broadcast
- Interactive confirmation with ✅ / ❌ reactions
- Auto-leaves servers **not in your VIP list**
- Configurable **prefix**, **owners**, and **delay between messages** to avoid rate limits
- Custom bot **status & activity**
- Keeps alive with Express server (useful for Replit/Heroku hosting)

---

## 📂 Project Structure

---

## ⚙️ Installation & Setup

1. Clone the repository:
   ```bash
   git clone <URL>
2. Install dependencies :
   ```bash
   npm install
4. Configure your bot:
```bash
   - Create a config.json file:
   {
  "Prefix": "!",
  "Time": 5000,
  "owners": ["YOUR_DISCORD_USER_ID"],
  "Vip": ["YOUR_SERVER_ID"]
}
```
-Prefix → Bot command prefix (default !)

-Time → Delay (in ms) between DMs (default 5000 = 5s)

-owners → List of Discord user IDs that can use the broadcast command

-Vip → List of server IDs where the bot is allowed to stay
4. Add your bot token in index.js:
 client.login("YOUR_BOT_TOKEN");
5. Start The Bot:
   node index.js
