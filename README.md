# Practice Exam Engine 🚀

A lightweight, modern, client-side web application designed for practicing technical examinations, certifications, and quizzes. Built with pure HTML5, CSS3, and Vanilla JavaScript with zero external framework dependencies.

![Exam Engine Preview](https://img.shields.io/badge/status-active-success) ![License](https://img.shields.io/badge/license-MIT-blue) ![Vanilla JS](https://img.shields.io/badge/javascript-vanilla-yellow)

---

## ✨ Key Features

* **Dynamic JSON Loader:** Instantly upload any custom question bank formatted as a JSON file or download the built-in template to create your own.
* **Session Persistence:** Automatically saves your progress, answers, and flagged questions to `localStorage` so you never lose your work if the page refreshes.
* **Interactive Navigation Sidebar:** Track your total, answered, remaining, and flagged questions in real-time with an intuitive question grid.
* **Timer & Privacy Controls:** Features an elapsed/countdown timer with pause functionality and a blur-screen toggle for privacy.
* **Instant Score & Review Breakdown:** Receive a comprehensive final score, time taken, detailed answer explanations, and a dedicated review panel for incorrect answers upon submission.
* **Theme Customization:** Switch seamlessly between a high-end minimalist dark mode and a clean sea-blue light mode.

---

## 🛠️ Tech Stack

* **Frontend:** HTML5, CSS3 (Glassmorphism, Custom Properties/Variables)
* **Logic:** Vanilla JavaScript (ES6+, Intersection Observer API, LocalStorage API)
* **Styling:** Fully responsive layout with custom grid systems and smooth transitions

---

## 📁 JSON Question Bank Structure

To use your own questions, structure your JSON file as follows (or use the built-in "Download Template" button directly in the app):

```json
{
    "config": {
        "topic": "Your Exam Name Here",
        "timeMinutes": 60
    },
    "questions": [
        {
            "question": "What is the capital of cloud computing?",
            "options": ["Option A", "Option B (Correct)", "Option C", "Option D"],
            "answer": [1],
            "explanation": "Explain why Option B is correct here.",
            "type": "single"
        },
        {
            "question": "Which of the following are cloud service models? (Select 2)",
            "options": ["IaaS", "CPU", "PaaS", "RAM"],
            "answer": [0, 2],
            "explanation": "IaaS and PaaS are core cloud service deployment models.",
            "type": "multiple"
        }
    ]
}
