# 🌟 Profile Card Project

A simple, elegant, and responsive **Profile Card** built using **semantic HTML5**, **CSS3**, and a bit of **vanilla JavaScript**.  
This project showcases a personal profile section with a photo, social links, hobbies, and dislikes — perfect for personal portfolios, resume sites, or introductory pages.

---

## 🧠 Project Overview

This project demonstrates:
- Use of **semantic HTML elements** (`article`, `header`, `section`, `figure`, `nav`) for accessibility and structure.  
- Integration of **responsive design principles** with a linked CSS file (`profilecard.css`).  
- A touch of **JavaScript** to dynamically display the current date and timestamp.  
- **Social media links** (GitHub, LinkedIn, and X/Twitter).  
- **Personalized content sections** for hobbies and dislikes.

---

## 📂 Project Structure

```bash
project-folder/
├── assets/
│   ├── ME.jpg                    # Profile picture
│   ├── github-mark-white.png     # GitHub logo
│   ├── InBug-White.png           # LinkedIn logo
│   ├── logo-white.png            # X (Twitter) logo
│
├── profilecard.html              # Main HTML file (this project)
├── profilecard.css               # Stylesheet (custom design)
└── README.md                     # Documentation file
```

---

## 🚀 Getting Started

Follow these steps to run the project **locally** on your computer.

### 1️⃣ Prerequisites
Make sure you have:
- A **modern web browser** (Chrome, Edge, Firefox, or Safari)
- A **text editor** (VS Code, Sublime Text, etc.)
- Optionally, a local web server (like VS Code Live Server extension) for smoother experience

---

### 2️⃣ Clone or Download the Repository

**Option A: Clone via Git**
```bash
git clone https://github.com/your-username/profile-card.git
```

**Option B: Download ZIP**
- Click on the green **“Code”** button above  
- Choose **“Download ZIP”**
- Extract the ZIP file to your preferred location

---

### 3️⃣ Open the Project

After cloning or extracting:

```bash
cd profile-card
```

Then open the folder in your code editor (for example, VS Code).

---

### 4️⃣ Run the Project

#### Option 1: Open Directly in Browser
- Locate the file: `profilecard.html`
- Double-click it to open in your browser

#### Option 2: Use Live Server (Recommended)
If using **VS Code**:
1. Install the **Live Server extension**
2. Right-click on `profilecard.html`
3. Select **“Open with Live Server”**

This ensures automatic reloads and smoother development.

---

## 🧩 Customization Guide

You can easily personalize your profile card:

| Section | How to Customize | Example |
|----------|------------------|----------|
| **Profile Image** | Replace `ME.jpg` in `/assets` with your image (keep the same filename or update the `src` path in HTML) | `/assets/your-photo.jpg` |
| **Name & Role** | Edit `<h2>` and `<h4>` inside `<header>` | `Ayeni Phillip` → `Your Name` |
| **Bio** | Update the `<p class="bio">` text | Add your short personal description |
| **Social Links** | Replace the `href` values with your social profile URLs | Update GitHub, LinkedIn, or X links |
| **Hobbies & Dislikes** | Edit the list items (`<li>`) | Add or remove items as you wish |

---

## 🧠 How It Works

The dynamic date display is handled using a small inline JavaScript script:
```javascript
const timeElement = document.querySelector('[data-testid="test-user-time"]');
timeElement.textContent = `Date: ${(new Date).toLocaleDateString()} (${Date.now()} ms)`;
```
This updates the date and timestamp when the page loads.

---

## 🧱 Technologies Used

| Technology | Purpose |
|-------------|----------|
| **HTML5** | Page structure & semantic layout |
| **CSS3** | Styling and responsive design |
| **JavaScript (ES6)** | Dynamic date and time display |
| **Accessibility Attributes** | Better usability for assistive technologies |

---

## 🧰 Best Practices Followed

- Semantic HTML for SEO and accessibility
- Minimal inline styling
- Clear separation of structure (HTML), style (CSS), and behavior (JS)
- Descriptive `alt` attributes for all images
- Externalized CSS for maintainability

---

## 📸 Preview

You can preview the card by opening:

```bash
profilecard.html
```

Your browser should display something similar to this layout:

```
+-------------------------------------+
|          [ Profile Image ]          |
|      Ayeni Phillip (Frontend Dev)   |
|  "Passionate about tech, research..."|
|   [X] [LinkedIn] [GitHub] Icons     |
|          Hobbies & Dislikes         |
+-------------------------------------+
```

---

## 🧑‍💻 Author

**Ayeni Phillip Adetunji**  
Frontend Developer | Tech Enthusiast | Research & People-focused  

- 🌐 [LinkedIn](https://www.linkedin.com/in/ayeni-phillip-adetunji/)  
- 🐦 [X (Twitter)](https://x.com/ayenitunji?t=Qqilk_Ky-nZSnSFM_CtqQ&s=09)  
- 💻 [GitHub](https://github.com/ASPAT1)

---

## 🤝 Contributing

Contributions, ideas, or suggestions are welcome!  
If you'd like to improve this project:
1. Fork the repository  
2. Create a new branch  
3. Commit your changes  
4. Open a Pull Request  

---

## 🪪 License

This project is open-source and available under the **MIT License**.  
You are free to use, modify, and distribute it as long as you give appropriate credit.

---

## 🏁 Final Notes

This project serves as a great **starter template** for building:
- Personal portfolios
- Developer introduction sections
- Resume or bio pages

Feel free to customize and build upon it! ✨
