# Internship Alert System 🚀

An automated system that scrapes internship listings daily, stores them in Google Sheets, and sends instant notifications to Telegram — ensuring you never miss an opportunity.


## 📌 Features

* **Daily Internship Scraping** – Uses [Apify](https://apify.com) to scrape internships from a target URL every midnight.
* **Google Sheets Integration** – Stores and updates internship details (Job Title & URL).
* **Duplicate Check** – Only adds new internships; updates existing entries if needed.
* **Telegram Notifications** – Sends internship alerts directly to your Telegram via a custom bot.
* **Automated Schedule** – Runs on a daily schedule without manual intervention.


## 🛠 Tech Stack

* **Apify** – For web scraping
* **n8n** – For workflow automation
* **Google Sheets API** – For storing internship data
* **Telegram Bot API** – For sending notifications


## ⚙️ Workflow Logic

1. **Scrape Data** – Apify Actor fetches internship listings from the given URL.
2. **Check Google Sheets** – Compares scraped internships with existing entries.
3. **Add / Update Entry** – If internship is new → append row. If existing → update.
4. **Send Telegram Alert** – Job title + URL sent to Telegram channel/group/user.

---

## 📅 Schedule

* Runs **every day at midnight (00:00)**.


## 📂 Google Sheet Structure

| Job Title          | URL                                        |
| ------------------ | ------------------------------------------ |
| Example Internship | [https://example.com](https://example.com) |


## 🚀 How to Use

1. Create a **Telegram Bot** via [BotFather](https://t.me/botfather) & get the bot token + chat ID.
2. Set up an **Apify Actor** to scrape your internship site.
3. Connect Google Sheets API & create your sheet.
4. Build workflow in **n8n** or similar automation tool.
5. Schedule it to run daily.


## 📸 Demo

🎥 https://lnkd.in/gszA7ufH


## 📌 Author

👩‍💻 Developed by anmgs


