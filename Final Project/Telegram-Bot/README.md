# 🌊 Early Warning System (EWS) Telegram Bot
<img width="313" height="353" alt="image" src="https://github.com/user-attachments/assets/e2b3bbc0-873e-417d-91e2-0ea91a477296" />

An automated water level monitoring and flood early warning system for the Sukapura River area. This bot integrates directly with a Supabase database to provide real-time information and emergency notifications to community members and group administrators.

<br>

## 📊 About
The Early Warning System (EWS) Bot is designed to continuously monitor water level fluctuations and disseminate crucial information to prevent the adverse impacts of flooding. Key features include:
- Automated Monitoring: Checks sensor data every 30 seconds.
- Status Change Notifications: Provides instant alerts when the alert status rises or falls.
- Hourly Routine Reports: Sends a summary of water conditions to the group every hour.
- Historical Analysis: Provides daily statistical data and the last 24 hours of history directly in the chat.
- Automatic Welcome System: Sends usage instructions via Private Message (DM) to new group members.

<br>

## 🚀 Features
- **Real-time Alerts**: Automated notifications for Alert Levels 1, 2, and 3.
- **Water Level Status**: Use the /status command to view current conditions and location.
- **Daily Reports**: Use the /report command to view today's average, highest, and lowest points.
- **24-Hour History**: Use the /history command to view water trends in 30-minute intervals over the last day.
- **Admin Control**: Specific commands and monitoring management accessible only to group administrators.
- **Multi-timezone Support**: All time data is automatically converted to Western Indonesia Time (WIB).

<br>

## 🛠️ Technology Stack
- **Language**: Python 3.x.
- **Telegram Framework**: python-telegram-bot (v20+).
- **Database**: Supabase (PostgreSQL + REST API).
- **Time Handling**: pytz for Asia/Jakarta timezone management.
- **Data Analysis**: statistics & collections for historical data processing.

<br>

## 📦 Installation

### Prerequisites
- Python 3.10+
- Bot Token from @BotFather
- Supabase Project (URL & Anon Key)

<br>

## ⚙️ Setup
1. **📂 Clone the Repository**
   - `git clone <repository-url>`
   - `cd ews-bot-telegram`

2. **📥 Install Dependencies**
   - `pip install python-telegram-bot requests pytz`

3. **🔑 Environment Configuration**
   Update the following variables in the source code:
   - `BOT_TOKEN`: Your Telegram Bot API Token.
   - `GROUP_ID`: The Telegram Group ID where notifications will be sent.
   - `SUPABASE_URL`: Your Supabase project URL.
   - `SUPABASE_KEY`: Your Supabase anonymous key.

4. **⚡ Run the Bot**
   ```bash
   python main.py
   
<br>

## 📊 Monitoring Levels
The system uses a 4-tier classification based on water height:

- 🔴 **Alert 1 (> 400 cm)**: Danger! Immediate evacuation instructions are sent.

- 🟠 **Alert 2 (300 - 400 cm)**: High Alert. Preparation for evacuation and securing assets.

- 🟡 **Alert 3 (200 - 299 cm)**: Warning. Securing important items and increasing vigilance.

- 🟢 **Alert 4 (< 200 cm)**: Normal. Routine monitoring continues.

<br>
  
## 📱 Bot Commands
- **/status** - Check current water level and alert status.

- **/report** - Statistical summary of data throughout the current day.
- **/history** - List of water history every 30 minutes for the last 24 hours.

- **/help** - Usage guide and list of available commands.

<br>

## ⚠️ Security Warning
**Never share files containing your BOT_TOKEN or SUPABASE_KEY publicly. Use Environment Variables for production deployment.**
