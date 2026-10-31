# 📚 Synonyms & Antonym Finder — Interactive Vocabulary & Dictionary Explorer

Synonyms & Antonym Finder is a modern, responsive, and interactive web application designed to help users explore English vocabulary effortlessly[span_0](start_span)[span_0](end_span). Powered by the free **Free Dictionary API**, Synonyms & Antonym Finder provides comprehensive word definitions, phonetics, audio pronunciations, contextual usage examples, and navigable synonyms and antonyms—all within an intuitive and elegant single-page user interface[span_1](start_span)[span_1](end_span).

## ✨ Features

- ⚡ **Priority Quick Synonyms & Antonyms:** Search any word to instantly see top-priority quick synonyms and antonyms displayed upfront before full part-of-speech definitions (noun, verb, adjective, adverb)[span_2](start_span)[span_2](end_span).
- 🔊 **Audio Pronunciation with Web Speech Fallback:** Listen to clear pronunciations using native API audio tracks with automatic Web Speech API synthesis fallback for continuous voice availability[span_3](start_span)[span_3](end_span).
- 🏷️ **Interactive Synonym & Antonym Badges:** Clickable green (synonym) and red (antonym) pills that immediately trigger a new search for seamless vocabulary exploration[span_4](start_span)[span_4](end_span).
- 🌓 **Dark & Light Mode Toggle:** Full thematic support for user comfort across day and night sessions[span_5](start_span)[span_5](end_span).
- 📜 **Search History Tracking:** Quickly access recently searched terms stored locally across sessions[span_6](start_span)[span_6](end_span).
- 📱 **Fully Responsive UI:** Built using Tailwind CSS, ensuring smooth rendering across mobile devices, tablets, desktop monitors, and Smart TVs[span_7](start_span)[span_7](end_span).

## 🛠️ Tech Stack & Dependencies

Synonyms & Antonym Finder is engineered as a zero-dependency, single-file lightweight web application[span_8](start_span)[span_8](end_span):

- **Frontend Core:** HTML5, Modern Vanilla JavaScript (ES6+)[span_9](start_span)[span_9](end_span)
- **Styling & UI:** [Tailwind CSS v3](https://tailwindcss.com/) (loaded via CDN)[span_10](start_span)[span_10](end_span)
- **Icons:** [FontAwesome 6.4](https://fontawesome.com/)[span_11](start_span)[span_11](end_span)
- **API Integration:** Native Browser `fetch()` API[span_12](start_span)[span_12](end_span)
- **Audio Output:** HTML5 `<audio>` Element & Web Speech API fallback[span_13](start_span)[span_13](end_span)

## 🌐 API Details

Synonyms & Antonym Finder integrates with the public **Free Dictionary API**[span_14](start_span)[span_14](end_span):

- **Endpoint URL:** `https://api.dictionaryapi.dev/api/v2/entries/en/{word}`[span_15](start_span)[span_15](end_span)
- **HTTP Method:** GET[span_16](start_span)[span_16](end_span)
- **Authentication:** None required (Open & Free)[span_17](start_span)[span_17](end_span)
- **Response Format:** JSON array containing phonetic transcriptions, audio file URLs, meanings, definitions, example sentences, synonyms, and antonyms[span_18](start_span)[span_18](end_span).

### Example JSON Payload Structure

```json
[
  {
    "word": "candid",
    "phonetic": "/ˈkændɪd/",
    "phonetics": [
      {
        "text": "/ˈkændɪd/",
        "audio": "[https://api.dictionaryapi.dev/media/pronunciations/en/candid-us.mp3](https://api.dictionaryapi.dev/media/pronunciations/en/candid-us.mp3)"
      }
    ],
    "meanings": [
      {
        "partOfSpeech": "adjective",
        "definitions": [
          {
            "definition": "Frank; outspoken; open and sincere.",
            "example": "He gave a candid assessment of the situation."
          }
        ],
        "synonyms": ["honest", "direct", "frank"],
        "antonyms": ["dishonest", "secretive"]
      }
    ]
  }
]
