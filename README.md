# Ajay Soni Portfolio

**Personal Portfolio Website with AI Chat Assistant**

A responsive portfolio website built to present projects, skills, certifications, and contact information in a clean web interface, with an integrated AI chatbot that can answer questions about the portfolio content.

![Status](https://img.shields.io/badge/status-active%20prototype-blue)
![HTML](https://img.shields.io/badge/html-5-orange)
![CSS](https://img.shields.io/badge/css-3-blue)
![JavaScript](https://img.shields.io/badge/javascript-ES6%2B-yellow)
![AI](https://img.shields.io/badge/feature-AI%20chatbot-purple)
![License](https://img.shields.io/badge/license-MIT-green)

---

## Overview

Ajay Soni Portfolio is a personal developer portfolio website for showcasing technical skills, machine learning projects, certifications, and contact details.

The project includes a browser-based AI chatbot assistant that can respond to questions about the portfolio owner, projects, skills, and contact information.

The portfolio is built using:

- HTML5
- CSS3
- Vanilla JavaScript
- OpenRouter API integration
- Gemini model through OpenRouter
- Local Storage for theme and session behavior

The goal of this project is to make a portfolio that is not only visually presentable, but also interactive enough for visitors to ask direct questions instead of manually searching through every section.

---

## Current Project Scope

This project is currently a **frontend portfolio prototype with AI chatbot integration**.

It is not:

- a full-stack production SaaS platform
- a private backend chatbot system
- a secure enterprise AI assistant
- a replacement for a resume or formal interview
- a guaranteed always-online AI service

The website is intended for personal branding, project presentation, GitHub showcasing, and recruiter-facing portfolio use.

---

## Why This Project Exists

Most portfolio websites are static.

They usually show:

```text
Name
Skills
Projects
Certificates
Contact links
```

That is useful, but visitors still need to manually search for information.

This project adds an AI chatbot layer so that visitors can ask questions such as:

- What projects has Ajay built?
- What are Ajay's main technical skills?
- How can I contact Ajay?
- What machine learning work is shown in this portfolio?
- Which certifications are listed?
- Is the portfolio owner suitable for ML or data science roles?

The main idea is simple:

```text
Portfolio Content
        ↓
Structured JavaScript Data
        ↓
AI Chatbot Context
        ↓
Visitor Questions
        ↓
Portfolio-Specific Answers
```

---

## Core Idea

The website combines a standard portfolio layout with an AI assistant.

The chatbot is not meant to be a general-purpose AI application. Its main purpose is to explain the portfolio content in a conversational way.

```text
Visitor opens portfolio
        ↓
Visitor explores sections
        ↓
Visitor opens chatbot
        ↓
Chatbot uses portfolio context
        ↓
Visitor receives direct answers
```

The chatbot responses are based on portfolio data and prompt instructions defined in the JavaScript logic.

---

## Main Features

| Feature | Purpose |
|---|---|
| Responsive Portfolio Layout | Works across desktop, tablet, and mobile screens |
| Hero Section | Introduces the portfolio owner clearly |
| About Section | Explains background, interests, and technical direction |
| Project Showcase | Displays selected projects with descriptions and links |
| Skills Section | Shows technical skills in a structured format |
| Certifications Section | Lists learning achievements and credentials |
| Contact Section | Provides direct ways to reach the portfolio owner |
| AI Chatbot Assistant | Answers questions about portfolio content |
| Dark/Light Theme | Allows visitors to switch visual mode |
| Theme Persistence | Stores selected theme locally |
| Chat Session Behavior | Maintains short-term interaction state in browser |
| Smooth UI Effects | Adds transitions and better user experience |

---

## AI Chatbot Assistant

The AI chatbot is the main interactive feature of the portfolio.

It is designed to answer portfolio-related questions such as:

```text
"What projects has Ajay built?"
"What skills are listed?"
"How can I contact Ajay?"
"What is Ajay's background?"
"Does Ajay work with machine learning?"
```

The chatbot flow:

```text
User Message
    ↓
Chat UI
    ↓
Portfolio Context
    ↓
OpenRouter API Request
    ↓
Gemini Model Response
    ↓
Formatted Chat Reply
```

If the API is unavailable, the chatbot should fall back to predefined responses instead of completely breaking the user experience.

---

## Portfolio Sections

| Section | Description |
|---|---|
| Home / Hero | First impression, headline, and call-to-action buttons |
| About | Short personal and technical background |
| Projects | Machine learning, AI, web, and development projects |
| Skills | Programming languages, tools, and technical areas |
| Certifications | Courses, certificates, and learning records |
| Contact | Email, GitHub, LinkedIn, and other contact options |
| AI Chatbot | Floating assistant for portfolio-specific queries |

---

## Design and User Experience

The portfolio focuses on a clean modern layout rather than heavy visual clutter.

Current design goals:

- readable text
- clear section spacing
- responsive layout
- accessible color contrast
- smooth animations
- professional project cards
- simple navigation
- usable mobile experience
- chatbot access without disturbing the page layout

The design should support the content instead of hiding it behind unnecessary effects.

---

## Current Workflow

The current project workflow is frontend-based.

```text
Edit portfolio content
        ↓
Update HTML / CSS / JavaScript
        ↓
Configure chatbot data
        ↓
Run locally in browser
        ↓
Test responsiveness
        ↓
Deploy to hosting platform
```

The project can run without a build step because it uses plain HTML, CSS, and JavaScript.

---

## Repository Structure

```text
AjaySoni-Portfolio/
│
├── README.md
├── LICENSE
│
├── index.html
│
├── style.css
│
├── script.js
│
│
├── assets/
│   ├── images/
│   │   ├── profile/
│   │   ├── projects/
│   │   └── certificates/
│   │
│   ├── icons/
│   └── documents/
│
└── docs/
    ├── chatbot_setup.md
    ├── deployment_notes.md
    └── future_improvements.md
```

The exact structure may change depending on how the project is organized.

If the project uses separate CSS and JavaScript folders, the structure can also be arranged like this:

```text
AjaySoni-Portfolio/
│
├── index.html
├── assets/
│   ├── css/
│   │   └── style.css
│   ├── js/
│   │   └── script.js
│   └── images/
└── README.md
```

---

## Tech Stack

| Tool / Technology | Purpose |
|---|---|
| HTML5 | Page structure |
| CSS3 | Styling, layout, responsiveness |
| JavaScript ES6+ | Interactivity and chatbot logic |
| OpenRouter API | AI model access |
| Gemini Model | Chatbot response generation |
| Local Storage | Theme and session persistence |
| Font Awesome | Icons |
| Google Fonts | Typography |
| WhatsApp Link API | Direct contact option |

---

## Installation

Clone the repository:

```bash
git clone https://github.com/AjaySoni-Dev/AjaySoni-Portfolio.git
cd AjaySoni-Portfolio
```

Open directly in browser:

```bash
start index.html
```

Or run using a local server.

Using Python:

```bash
python -m http.server 8000
```

Using Node.js:

```bash
npx http-server
```

Using PHP:

```bash
php -S localhost:8000
```

Then open:

```text
http://localhost:8000
```

---

## Configuration

### Portfolio Data

Update the portfolio content inside the HTML or JavaScript file depending on the current implementation.

Typical editable content includes:

```text
name
title
about
skills
projects
certifications
social links
contact links
chatbot knowledge base
```

If the project uses a JavaScript object for data, update values like:

```javascript
const portfolioData = {
  name: "Ajay Soni",
  title: "Machine Learning Engineer",
  skills: [],
  projects: [],
  certifications: []
};
```

---

## AI Chatbot Setup

The chatbot uses OpenRouter API.

### Step 1: Get an API Key

Create an API key from OpenRouter.

### Step 2: Add the API Key

In development, the key may be placed in the JavaScript file:

```javascript
const API_KEY = "YOUR_API_KEY_HERE";
```

However, this is not recommended for public deployment.

### Important Security Warning

Do not expose a real API key directly in public frontend code.

For public deployment, use a backend proxy or serverless function.

Recommended safer flow:

```text
Browser
   ↓
Your Backend / Serverless Function
   ↓
OpenRouter API
   ↓
AI Response
   ↓
Browser
```

This prevents users from directly viewing or copying the API key from the browser source code.

---

## How the Chatbot Works

The chatbot follows this basic logic:

```text
User opens chat widget
        ↓
User sends question
        ↓
Question is combined with portfolio context
        ↓
Request is sent to AI API
        ↓
AI response is returned
        ↓
Message is displayed in chat window
```

Example supported questions:

```text
Tell me about Ajay.
What projects are shown here?
What skills does Ajay have?
How can I contact Ajay?
Does Ajay have machine learning experience?
```

The chatbot should stay focused on the portfolio and avoid giving unrelated or misleading answers.

---

## Deployment Options

The project can be deployed on static hosting platforms.

| Platform | Notes |
|---|---|
| GitHub Pages | Free and simple for static websites |
| Netlify | Easy deployment with custom domain support |
| Vercel | Good GitHub integration |
| InfinityFree | Free hosting option |
| Firebase Hosting | Good for future expansion |
| Cloudflare Pages | Fast static hosting |

If the chatbot uses a real API key, use a backend or serverless function instead of placing the key directly in frontend code.

---

## Implementation Status

| Component | Status | Current Form |
|---|---|---|
| Responsive layout | Implemented | HTML/CSS |
| Hero section | Implemented | Static section |
| About section | Implemented | Static content |
| Project cards | Implemented | HTML/CSS/JS |
| Skills section | Implemented | Static/animated UI |
| Certifications section | Implemented | Static content |
| Contact section | Implemented | Links and contact options |
| Dark/light theme | Implemented | JavaScript + Local Storage |
| AI chatbot UI | Implemented | Floating chat widget |
| OpenRouter API connection | Implemented | JavaScript fetch request |
| Portfolio context injection | Implemented | JavaScript object/prompt |
| Offline fallback responses | Partial | Basic fallback logic |
| API key protection | Needs improvement | Backend/serverless recommended |
| Accessibility testing | Partial | Needs manual testing |
| SEO optimization | Partial | Needs metadata refinement |
| Performance optimization | Partial | Needs image and script audit |
| Backend proxy | Planned | Not implemented |
| Admin content editor | Future work | Not implemented |

---

## Current Limitations

- The project is mainly frontend-based.
- A public API key in JavaScript is not secure.
- Chatbot quality depends on the model and prompt design.
- The chatbot can still produce imperfect answers.
- Portfolio content must be updated manually.
- There is no admin dashboard for editing content.
- There is no backend database.
- SEO may need improvement before serious public promotion.
- Image optimization may be required for faster loading.
- Accessibility should be tested on keyboard and screen readers.
- The chatbot should not be treated as an official hiring or verification system.

---

## Future Work

Planned improvements:

- add backend or serverless proxy for API protection
- improve chatbot prompt safety and accuracy
- add better fallback responses
- improve SEO metadata
- optimize images and loading speed
- add project filters by category
- add downloadable resume button
- add better mobile chatbot layout
- add contact form with validation
- add analytics for visitor behavior
- add testing for accessibility and responsiveness
- convert repeated content into structured JSON
- add deployment documentation
- add screenshots and live demo preview in README

---

## Recommended README Additions Later

The following items can make the repository stronger after the project is stable:

```text
screenshots/
demo GIF
live website preview image
Lighthouse performance score
known issues
version history
contribution rules
```

These are not required immediately, but they improve the professional appearance of the repository.

---

## Important Notes

This portfolio is a personal web project with AI-assisted interaction.

The AI chatbot should be used only as a helpful guide for visitors. Important professional details such as education, certifications, project links, and contact information should still be verified through the visible portfolio sections or official profiles.

Do not store sensitive personal data or private credentials directly in the frontend files.

---

## Author

**Ajay Soni**

Aspiring Machine Learning Engineer

Focus areas:

- Machine Learning
- Data Science
- Web Development
- AI-Integrated Interfaces
- Portfolio Automation
- Frontend User Experience

---

## License

This project is licensed under the MIT License.

---

## Contact

| Platform | Link |
|---|---|
| Portfolio | https://learnerportfolio.rf.gd |
| GitHub | https://github.com/AjaySoni-Dev |
| LinkedIn | https://www.linkedin.com/in/AjaySoni-Dev/ |
| Email | programmingwithcode@gmail.com |

