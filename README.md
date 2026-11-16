# web-development-task-3

Interactive Personal Portfolio Website (Week 3: JavaScript) — Yethendra Sai Gantala
An interactive personal portfolio website built for Week 3: JavaScript - Making Websites Interactive, extending the Week 1 HTML5 and Week 2 CSS3 portfolio with client-side scripting, DOM manipulation, event handling, real-time form validation, and `localStorage` persistence.
Author: Yethendra Sai Gantala
Repository: saigantala/web-development-task-3
GitHub Profile: github.com/saigantala
LinkedIn: Yethendra Sai Gantala
Project Overview
This project demonstrates client-side JavaScript fundamentals by transforming a static styled portfolio into an interactive web experience. All JavaScript logic is cleanly separated into `script.js` and linked to `index.html`, using reusable functions, event listeners, dynamic DOM updates, and browser `localStorage`.
JavaScript Theory Concepts Covered
Client-Side Scripting: Executing JavaScript directly in the user's browser to respond to user actions without full page reloads.
Variables, Data Types & Operators: `const` and `let`, strings, booleans, arrays, objects, template literals, and logical/comparison operators.
Functions & Event Handling: Reusable named functions (`toggleDarkMode()`, `goToSlide()`, `validateForm()`, `renderGoals()`) wired to `click`, `input`, and `submit` events via `addEventListener`.
DOM Manipulation: Selecting elements (`getElementById`, `querySelectorAll`), toggling classes (`classList.toggle`), updating attributes (`setAttribute`, `removeAttribute`), and dynamically creating elements (`document.createElement`, `appendChild`).
Browser Storage (`localStorage`): Saving and restoring user preferences (dark/light theme and custom learning goals) across page refreshes using `localStorage.getItem` and `localStorage.setItem`.
Client-Side Form Validation: Real-time field checks on `input` and final validation on `submit` with inline error feedback and live character counting.
Project Structure
```text
web-development-task-3/
├── index.html          # Semantic HTML5 structure linked to style.css & script.js
├── style.css           # External stylesheet with light/dark theme variables & responsive grid
├── script.js           # External JavaScript for interactivity, DOM updates & validation
├── README.md           # Project documentation, JS theory, and testing evidence
└── images/
    └── profile.jpg     # Portrait photo of Yethendra Sai Gantala
```
Interactive Features Implemented
Dark / Light Mode Toggle (`localStorage`): Switches between light and dark CSS variable themes and persists the choice across reloads.
Show / Hide Extra Bio Details: Expands or collapses additional background details with accessible `aria-expanded` state updates.
Skill Category Filter: Filters skill cards dynamically (`All`, `Frontend`, `Workflow`) using `data-category` attributes.
Interactive Milestone Slider: Navigates Week 1–3 highlights with Previous/Next buttons and clickable dot indicators.
Interactive Learning Goals Tracker: Adds new goals, toggles completion on click, and removes items dynamically with `localStorage` persistence.
Real-Time Contact Form Validation: Validates Name (`>= 2` chars), Email (`@` and `.`), and Message (`>= 10` chars) with live character count and status banners.
Setup Instructions
Install Visual Studio Code and the Live Server extension.
Clone this repository:
```bash
   git clone https://github.com/saigantala/web-development-task-3.git
   ```
Open the `web-development-task-3` folder in VS Code.
Right-click `index.html` and choose Open with Live Server (or open `index.html` directly in any modern browser).
7-Day Development Breakdown
Day	Focus Area	What Was Implemented
Day 1	Setup JavaScript	Created `script.js` and linked it at the bottom of `index.html`
Day 2	DOM Manipulation	Selected elements with `getElementById` / `querySelectorAll` and updated classes/text
Day 3	Event Handling	Added `click`, `input`, and `submit` listeners for buttons, filters, and forms
Day 4	Form Validation	Implemented `validateName()`, `validateEmail()`, `validateMessage()`, and `validateForm()`
Day 5	Interactive Features	Built Dark Mode toggle, Show/Hide bio, Milestone Slider, and Goals Tracker
Day 6	Local Storage	Persisted `darkMode` and `portfolioGoals` in `localStorage`
Day 7	Testing & Debugging	Verified all interactive controls, edge cases, and mobile responsiveness
Testing Evidence
Test ID	Feature Tested	Input / Action	Expected Result	Status
TC-01	Dark/Light Mode	Click theme toggle button & refresh page	Theme switches and persists via `localStorage`	Passed
TC-02	Show/Hide Bio	Click "Show More Details" button	Extra bio expands and button label updates	Passed
TC-03	Skill Filter	Click `Frontend` / `Workflow` / `All`	Displays matching skill cards only	Passed
TC-04	Milestone Slider	Click Next/Prev arrows and dots	Smoothly transitions between Week 1–3 slides	Passed
TC-05	Goals Tracker	Add, click to complete, and remove a goal	Updates DOM list and persists in `localStorage`	Passed
TC-06	Form Validation	Submit invalid email or short message	Shows inline field errors and blocks submission	Passed
TC-07	Valid Form Submit	Enter valid name, email, and 10+ char message	Shows green confirmation banner and resets form	Passed
