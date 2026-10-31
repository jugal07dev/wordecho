# 📚 Synonyms & Antonyms Finder — Interactive Vocabulary & Thesaurus Explorer

**Synonyms & Antonyms Finder** is a modern, responsive single-page web application designed for students, writers, and language enthusiasts to explore English vocabulary effortlessly. Built with modern web standards, Synonyms & Antonyms Finder provides comprehensive definitions, phonetics, audio pronunciations, usage examples, and navigable synonyms and antonyms—all within an intuitive glassmorphism interface.

---

## ✨ Features

- 🔍 **Real-Time Word Lookup:** Search any English word to view rich definitions categorized by part of speech (noun, verb, adjective, adverb).
- 🔊 **Audio Pronunciation:** Listen to spoken pronunciations powered by native Web Speech API synthesis with fallback audio playback.
- 🏷️ **Interactive Tag Navigation:** Click on any green (synonym) or red (antonym) pill to immediately trigger a dynamic search for that term.
- 🌓 **Dark & Light Mode:** Full thematic switching with smooth CSS transitions, retaining user preferences across sessions.
- 📜 **Search History:** Tracks recent queries stored locally via browser `localStorage` for fast re-searches.
- 📱 **Fully Responsive UI:** Built with Tailwind CSS to ensure seamless display on mobile phones, tablets, laptops, and Smart TVs.

---

## 👥 Authors & Contributors

This project was developed collaboratively as a two-person team:

* **Jugal Chettri** (Roll No: `24SV0019`) — API Integration, Asynchronous Data Handling & JavaScript Logic
* **Simran Rai** (Roll No: `24SV0005`) — Frontend UI/UX, Tailwind CSS Styling & Responsive Design

---

## 🛠️ Tech Stack & Dependencies

Synonyms & Antonyms Finder is engineered as a zero-dependency, single-file lightweight web application:

- **Frontend Core:** HTML5, Modern Vanilla JavaScript (ES6+)
- **Styling & UI:** [Tailwind CSS v3](https://tailwindcss.com/) (loaded via CDN)
- **Iconography:** [Lucide Icons](https://lucide.dev/)
- **Data Fetching:** Native Browser `fetch()` API (Asynchronous Promises)
- **Audio Output:** Web Speech API & HTML5 Audio Interface

---

## 🌐 API Details

Synonyms & Antonyms Finder combines data asynchronously from two public REST APIs:

### 1. Free Dictionary API
- **Purpose:** Fetches definitions, phonetics, parts of speech, and contextual example sentences.
- **Endpoint:** `https://api.dictionaryapi.dev/api/v2/entries/en/{word}`
- **HTTP Method:** `GET`
- **Authentication:** None required

### 2. Datamuse API
- **Purpose:** Fetches categorized synonym and antonym collections.
- **Endpoints:** 
  - Synonyms: `https://api.datamuse.com/words?rel_syn={word}`
  - Antonyms: `https://api.datamuse.com/words?rel_ant={word}`
- **HTTP Method:** `GET`
- **Authentication:** None required

---

## 🚀 Getting Started & Local Setup

Since Synonyms & Antonyms Finder is built as a portable single-file application (`index.html`), setup requires zero package managers (`npm`/`yarn`) or build compilers.

### Prerequisites
- Any modern web browser (Google Chrome, Mozilla Firefox, Apple Safari, Microsoft Edge).

### Running Locally
1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/wordecho.git
   cd wordecho
   ```
2. **Launch the app:**
   - Double-click `index.html` to open it directly in your browser.
   - Or serve it using a simple HTTP server:
     ```bash
     # Using Python 3
     python -m http.server 8000
     ```
     Then navigate to `http://localhost:8000` in your web browser.

---

## ☁️ Deployment

WordEcho is optimized for fast static deployment:

- **GitHub Pages:** Navigate to **Settings > Pages**, set the Branch to `main` (or `master`), and click **Save**.
- **Netlify:** Drag and drop the project folder onto [app.netlify.com/drop](https://app.netlify.com/drop).
- **Vercel:** Import your GitHub repository into Vercel for instant static hosting.

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
