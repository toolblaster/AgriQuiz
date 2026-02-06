AgriQuiz: Free Agriculture Mock Test & Exam Prep

AgriQuiz is a lightweight, high-performance Single Page Application (SPA) designed to help students prepare for competitive agriculture exams like ICAR JRF, IBPS AFO, NABARD, and State Agriculture exams.

It features a robust question bank of 407+ bilingual questions (English & Hindi) and requires no login or backend server, running entirely in the browser.

🚀 Key Features

Bilingual Questions: Toggle-free experience; questions appear in both English and Hindi simultaneously.

Offline-First: All data is loaded upfront; works seamlessly even with unstable internet.

No Login Required: Instant access for students; progress is saved automatically to localStorage.

Smart Study Modes:

Normal Mode: Sequential learning (Q1 to Q407).

Shuffle Mode: Randomizes question order to prevent pattern memorization.

Quick 10 Mode: Generates a mini-quiz of the next 10 unanswered questions for rapid revision.

Mistakes Mode: specialized filter to review only questions answered incorrectly.

Bookmark Filter: Save difficult questions for later review.

Deep Linking: Share specific questions with friends using unique URLs (e.g., ?id=123).

Data Persistence:

Auto-save progress (last question, answers, bookmarks).

Backup & Restore: Export progress to a .json file and import it on another device.

Performance:

Mobile-first responsive design.

Dark Mode / Light Mode support.

WCAG AA compliant high-contrast colors.

📂 Project Structure

AgriQuiz/
├── index.html          # Core application logic and UI
├── js/
│   ├── style.css       # Centralized styling (Dark/Light mode, Responsiveness)
│   ├── part1.js        # Question Data Part 1
│   ├── part2.js        # Question Data Part 2
│   ├── part3.js        # Question Data Part 3
│   └── part4.js        # Question Data Part 4
├── favicon/            # Icons and Web Manifest
│   ├── android-chrome-*.png
│   ├── favicon.ico
│   └── site.webmanifest
├── legal/              # Compliance documents
│   ├── about.html
│   ├── privacy.html
│   └── terms.html
├── robots.txt          # SEO crawler directives
└── sitemap.xml         # Search engine map


🛠️ Tech Stack

HTML5: Semantic structure and accessibility.

CSS3: Custom variables for theming, Flexbox/Grid for layout, and media queries for mobile optimization.

Vanilla JavaScript (ES6+): No frameworks (React/Vue/Angular) used. Keeps the app extremely fast and lightweight (<1MB total).

LocalStorage API: For persisting user state without a database.

🚀 How to Run

Clone or Download the repository.

Open index.html in any modern web browser.

That's it! No npm install, no build steps, no server required.

⚙️ Customization

Modifying Questions

Questions are stored in the js/ folder split into multiple files (part1.js, etc.) to keep file sizes manageable. The format is:

window.quizData = window.quizData || [];
window.quizData.push({
    id: 1,
    questionEn: "Question in English?",
    questionHi: "Question in Hindi?",
    options: ["Option A", "Option B", "Option C", "Option D"],
    answer: 0 // Index of correct option (0 = A, 1 = B, etc.)
});


Changing Themes

Colors are defined as CSS variables in js/style.css under the :root (Light Mode) and [data-theme="dark"] selectors.

📱 Mobile Optimizations

The interface automatically adapts for screens smaller than 600px:

Compact button sizes.

Reduced font sizes for questions to prevent scrolling fatigue.

Condensed dashboard layout.

🤝 Contributing

Fork the repository.

Create a new branch for your feature (git checkout -b feature/AmazingFeature).

Commit your changes (git commit -m 'Add some AmazingFeature').

Push to the branch (git push origin feature/AmazingFeature).

Open a Pull Request.

📄 License

This project is open-source and free to use for educational purposes.

Built with ❤️ by ToolBlaster.com
