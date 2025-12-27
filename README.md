# ⏱️ Minutes to Win It (aka Loco-Host)

**An automated live quiz platform that turns boring meeting notes into a gamified showdown.**

![Project Status](https://img.shields.io/badge/Status-Live-success)
![Tech Stack](https://img.shields.io/badge/Tech-n8n%20%7C%20Gemini%20%7C%20Firebase-orange)

## 🧐 The Problem
Meeting organizers struggle to verify if attendees are actually listening. Google Forms are boring, and engagement drops after the presentation ends.

## 💡 The Solution
A fully automated pipeline where:
1.  **n8n** reads meeting notes.
2.  **Gemini AI** extracts key facts and generates MCQs.
3.  Questions are synced to a **Google Sheet**.
4.  A custom **Web App** (Firebase) runs a real-time multiplayer game.

## 📂 Project Structure
* **`/frontend`**: The custom HTML5/JS game engine. Features real-time syncing, speed scoring, and avatars.
* **`/automation`**: The n8n workflow JSON file. Import this to run the AI question generator.

## 🚀 How to Run
1.  **Setup the Backend:**
    * Import the JSON from `/automation` into n8n.
    * Connect your Gemini API Key and Google Sheet ID.
2.  **Setup the Game:**
    * Open `/frontend/index.html`.
    * Add your Firebase Config and Sheet ID.
    * Host on Netlify or GitHub Pages!

## 📸 Features
* ✅ **Real-time Leaderboard** (Updates instantly)
* ✅ **Speed Scoring** (Faster answer = More points)
* ✅ **Olympic Podium Victory Screen**
* ✅ **Admin Panel** with Kick/Reset controls

---
*Built with ❤️ for GDG Events.*
