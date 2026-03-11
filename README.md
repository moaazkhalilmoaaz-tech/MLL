# MLL Bot
MLL Bot is an all-in-one Discord bot combining Moderation, Automation, Economy, Leveling, Dashboard management, Fun & Games, and Advanced Features in a single bot.

Features
1. Moderation

Ban / Unban / Kick members

Clear messages

Lock / Unlock channels

Hide / Show channels

Mute / Unmute (Text + Voice + Timeout)

Move / Come members

Role management (add/remove/list)

Change Nickname

Warn system (add/remove/list warnings)

Auto Moderation / Spam Filter (optional) – filter bad words, links, mentions

2. Automation

Auto Reply: Responds to keywords with optional embeds, allowed roles, and allowed channels

Auto React: Automatically reacts to messages in specific channels

Auto Line: Sends images or custom lines automatically in specified channels

3. Economy System

Credits system (view, transfer, add/remove, tax)

Leaderboard with pagination

Commands: /credits, /leaderboard, or prefix commands

Customizable economy settings via Dashboard

4. Leveling System

XP from chat messages and voice activity

Commands: /profile, /rank, /top, prefix p/r/t

Leveling works only in specified channels

Admin-only commands for /set-level and /set-xp

5. Auto Role

Assigns Member role automatically to new members

Assigns Bot role automatically to bots

6. Persistent Mute

Restores mute roles for members who rejoin

Automatically updates new channels to restrict muted members

7. Dashboard / Web Panel

Manage all bot settings via a web interface

Settings include:

Prefix

Auto Reply / React / Line

Economy / Credits

Permissions

Allowed Channels / Roles

Built with NestJS + Pug templates

Provides a REST API for advanced integrations

8. Ticket / Support System

Users can open support tickets

Admins can manage tickets from Dashboard

Optional automated ticket logs

9. Logging System

Logs all moderation actions (Ban / Kick / Mute / Role changes)

Detailed audit for server admins

10. Custom Commands

Server owners can create custom commands without coding

Supports embeds, replies, and role/channel restrictions

11. Music / Audio Features

Play music from YouTube / Spotify

Music commands: Play, Pause, Resume, Skip, Queue, Stop

Works in voice channels

12. Reminder / Scheduler

Set personal reminders or server-wide scheduled messages

Supports recurring reminders

13. Reaction Roles / Self Roles

Members can assign themselves roles by reacting to messages

Supports multiple reactions per message

14. Custom Level Rewards

Assign server roles automatically on level-up

Configurable rewards via Dashboard

15. Stats / Server Insights

View server statistics: total members, daily messages, active voice users

Graphs available in Dashboard

16. Fun / Games Commands

Trivia / Hangman / Tic Tac Toe / Coin Flip / Dice Roll

Enhances server engagement and activity

17. Security / Server Protection

Works only in allowed servers (ALLOWED_SERVERS)

Automatically leaves unauthorized servers

Tech Stack

Backend: NestJS, Necord, discord.js

Database: PostgreSQL + TypeORM

Dashboard: Pug templates + REST API

Environment Variables
BOT_TOKEN=                 # Discord Bot Token
DATABASE_URL=               # PostgreSQL connection string
JWT_SECRET=                 # JWT secret for Dashboard
ADMIN_SECRET=               # Admin auth secret
ALLOWED_SERVERS=            # Comma-separated guild IDs
PORT=                       # Dashboard / API port
Installation
git clone <repository-url>
cd <repository-folder>
npm install
npm run start
Project Structure
src
 ├─ commands             # All bot commands
 ├─ listeners            # Event listeners (message, voice, join/leave)
 ├─ services             # Core services (Moderation, Economy, Leveling, Auto systems)
 ├─ api                  # Dashboard & REST API endpoints
 ├─ database             # TypeORM entities, migrations
 └─ discord              # Necord + Discord.js integration
Usage
Commands

Prefix commands: p / r / t
Slash commands: /ban, /credits, /profile, etc.

Admin-only channels for moderation commands and leveling adjustments are configurable via Dashboard.

Notes

Fully customizable via Dashboard

Supports multi-server operation

Highly scalable and modular

Can serve as a replacement for MEE6 / Dyno / ProBots
