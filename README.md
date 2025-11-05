# My Interactive Terminal Portfolio

### 🔴 **Live Demo:** [Vikas Porfolio](https://vikas-porfolio.netlify.app)
---
![Terminal Section](https://github.com/Vikas2171/my-portfolio/blob/main/screenshots/terminal.png)

---

![Cipher Machine](https://github.com/Vikas2171/my-portfolio/blob/main/screenshots/cipher-machine.png)

---

![Contact](https://github.com/Vikas2171/my-portfolio/blob/main/screenshots/contact.png)

---
## About This Project

This is a fully interactive, responsive portfolio designed to look and feel like a developer's terminal. The entire project is built from scratch using **vanilla HTML, CSS, and JavaScript**, showcasing a deep understanding of core web technologies.

The terminal is not just for show—it's a fully functional command-line interface (CLI) where users can execute commands like `about`, `projects`, `skills`, and `contact` to navigate the site.

This project was initially built as a full-stack application with a Node.js and Express backend. However, for better performance, scalability, and zero hosting costs, I **re-architected it to a modern serverless (Jamstack) model** hosted on Netlify.

## 🎨 Design Process

The design for this portfolio is **100% original**. It was not taken from any template or tutorial.

I personally imagined and designed the complete user interface and all components in **Figma** before writing a single line of code. This allowed me to iterate on the "hacker" theme and ensure a consistent, responsive layout across both desktop and mobile.

## ✨ Features

  * **Interactive Terminal:** A custom-built JavaScript CLI that parses user commands and handles output.
  * **Live Coding Stats:** The `about` command fetches and displays real-time competitive programming stats by calling a custom-built serverless function, with data cached for 1 hour to ensure speed.
  * **Client-Side Cipher Machine:** A set of encryption tools (Caesar, Affine, Vigenere) that run entirely in the browser using JavaScript.
  * **Secure Contact Form:** The "Contact" section uses **Netlify Forms** to securely handle submissions without a backend, including email notifications.
  * **Fully Responsive:** The layout, from the ASCII art to the terminal output, gracefully adapts to all screen sizes, from wide desktops to narrow mobile phones.

## 🛠 Tech Stack & Architecture

This project runs with no traditional backend server. The backend logic was intentionally unbundled into a serverless architecture:

  * **Frontend:** `HTML5`, `CSS3` (with Flexbox, Grid, and Media Queries), `Vanilla JavaScript`
  * **Backend (Serverless):**
      * **Netlify Functions:** A single serverless function (written in Node.js) is used to fetch live stats from third-party APIs (Codeforces, LeetCode). This securely bypasses CORS issues and protects API keys.
      * **Netlify Forms:** Replaced the original `nodemailer` backend. Netlify securely handles all contact form submissions and provides spam filtering and email notifications.
  * **Hosting:** `Netlify` (Provides continuous deployment from a private GitHub repo, site hosting, function execution, and form handling all for free).
