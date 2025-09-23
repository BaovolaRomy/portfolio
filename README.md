### Baovola ANDRIANARISOA – Portfolio

This repository hosts my personal **portfolio website**, built to showcase my projects in **Power Platform** (Power Apps, Power Automate, SharePoint, CI/CD Pipelines) as well as web development projects.

The website is based on the **Massively** template from [HTML5 UP](https://html5up.net/), customized and extended with additional sections, lightbox galleries, and project details.

---

## 🚀 Live Demo
The portfolio is available here:  
👉 [https://BaovolaRomy.github.io/portfolio](https://BaovolaRomy.github.io/portfolio)

---

## 📂 Project Structure

├── index.html # Main portfolio page
├── assets/ # CSS, JS, fonts
│ ├── css/
│ ├── js/
│ └── ...
├── images/ # Project screenshots & logos
│ ├── TF/ # Talent Flow app images
│ ├── FFRT/ # Finance vendor app images
│ ├── Pipelines/ # CI/CD pipelines screenshots
│ ├── EVAS/ # EVAS web app images
└── README.md # This file


---

## ✨ Features
- **Responsive design** using the Massively template (HTML5 UP).
- **Project showcase** with dedicated sections for:
  - Power Apps & Power Automate
  - SharePoint
  - Pipelines (CI/CD)
  - Other projects (EVAS, Portfolio itself…)
- **Lightbox galleries** for project details (navigate images with arrows).
- **Contact section** with email and social links.
- Hosted on **GitHub Pages**.

---

## 🛠️ Tech Stack
- HTML5 / CSS3 / JavaScript
- Massively template (HTML5 UP)
- jQuery (from the original theme)
- GitHub Pages for deployment

---

## 🔧 Setup & Local Development
Clone the repo and open `index.html` in your browser:

```bash
git clone https://github.com/BaovolaRomy/portfolio.git
cd portfolio
open index.html   # or double-click index.html
https://BaovolaRomy.github.io/portfolio/

# Contact Form via EmailJS (GitHub Pages Friendly)

This site uses **EmailJS** to send contact form submissions directly from the browser — no backend required.  
Works on **GitHub Pages**.

---

## 1) Prerequisites

- EmailJS account → https://www.emailjs.com/
- An email service connected in EmailJS:
  - **iCloud SMTP (recommended for your setup)**  
    - Enable Apple ID **2FA**  
    - Generate an **App-Specific Password** at https://appleid.apple.com/  
    - SMTP settings:
      - Host: `smtp.mail.me.com`
      - Port: `587` + STARTTLS (or `465` + SSL if needed)
      - Username: your full iCloud address (e.g. `baoromy@icloud.com`)
      - Password: your **app-specific password** (not Apple ID password)
- Create an **EmailJS Template** (e.g., `template_xxxxxx`)
- Note your:
  - **Service ID**: `service_xxxxxx`
  - **Template ID**: `template_xxxxxx`
  - **Public Key**: `YOUR_PUBLIC_KEY`

---

## 2) HTML Form

Place this in your footer (or wherever your contact section lives):

```html
<form id="contact-form">
  <div class="fields">
    <div class="field">
      <label for="name">Name</label>
      <input type="text" name="user_name" id="name" required />
    </div>
    <div class="field">
      <label for="email">Email</label>
      <input type="email" name="user_email" id="email" required />
    </div>
    <div class="field">
      <label for="message">Message</label>
      <textarea name="message" id="message" rows="3" required></textarea>
    </div>
  </div>

  <!-- iCloud requires the "From" to be your iCloud address -->
  <input type="hidden" name="from_email" value="baoromy@icloud.com" />
  <input type="hidden" name="subject" value="New message from portfolio" />

  <!-- optional honeypot (spam protection) -->
  <input type="text" name="_gotcha" tabindex="-1" autocomplete="off" style="display:none" />

  <ul class="actions">
    <li><button type="submit" class="primary">Send Message</button></li>
  </ul>
  <p id="form-status" style="margin-top:1rem;"></p>
</form>


📬 Contact

Email: baoromy@icloud.com

LinkedIn: Baovola Andrianarisoa

GitHub: BaovolaRomy


---

👉 Do you want me to also include a **section with screenshots of each project** (Talent Flow, FFRT, Pipelines, EVAS) directly in the README, so recruiters can preview them without opening the site?

