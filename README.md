# American British Translator

This is my solution for the [American British Translator project on freeCodeCamp](https://www.freecodecamp.org/learn/quality-assurance/quality-assurance-projects/american-british-translator).

## 📌 Overview

This microservice translates text between American and British English using a predefined dictionary. It includes an API endpoint to perform the translation and returns a highlighted version showing the translated terms. Invalid or empty inputs are handled with appropriate error messages.

## 📡 API Endpoint

POST /api/translate  
Translates given text from one locale to another.

Request body:  
- text (required): the text to translate  
- locale (required): either american-to-british or british-to-american

Response examples:  
- { "text": "favorite", "translation": "favourite" }  
- { "error": "Required field(s) missing" }  
- { "error": "Invalid value for locale field" }  
- { "error": "No text to translate" }  
- { "translation": "Everything looks good to me!" }

Translated terms are wrapped in:  
<span class="highlight">translated_word</span>

## ⚙️ Technologies Used

- Node.js  
- Express.js  
- Mocha & Chai (for testing)  
- dotenv

## 🧪 Running Tests

Install dependencies and run the tests:  
npm install  
npm test

Tests include:  
- Translation logic  
- HTML highlighting  
- Handling of missing/invalid inputs

## 🛠️ Getting Started Locally

Clone the repository:  
git clone https://github.com/giannis07/fcc_american_british_translator.git  
cd fcc_american_british_translator

Install dependencies:  
npm install

Start the app:  
npm start

Visit the app at:  
http://localhost:3000

## 💻 Source Code

GitHub Repository: https://github.com/giannis07/fcc_american_british_translator
