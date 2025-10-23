# Profile Card Project

A simple, elegant, and responsive **Profile Card** built using **semantic HTML5**, **CSS3**, and a bit of **vanilla JavaScript**.  
This project showcases a personal profile section with a photo, social links, hobbies, and dislikes — perfect for personal portfolios, resume sites, or introductory pages.

---

## Project Overview

This project demonstrates:
- Use of **semantic HTML elements** (`article`, `header`, `section`, `figure`, `nav`) for accessibility and structure.  
- Integration of **responsive design principles** with a linked CSS file (`profilecard.css`).  
- A touch of **JavaScript** to dynamically display the current date and timestamp.  
- **Social media links** (GitHub, LinkedIn, and X/Twitter).  
- **Personalized content sections** for hobbies and dislikes.

---

## Project Structure

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

## Getting Started

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

## Customization Guide

You can easily personalize your profile card:

| Section | How to Customize | Example |
|----------|------------------|----------|
| **Profile Image** | Replace `ME.jpg` in `/assets` with your image (keep the same filename or update the `src` path in HTML) | `/assets/your-photo.jpg` |
| **Name & Role** | Edit `<h2>` and `<h4>` inside `<header>` | `Ayeni Phillip` → `Your Name` |
| **Bio** | Update the `<p class="bio">` text | Add your short personal description |
| **Social Links** | Replace the `href` values with your social profile URLs | Update GitHub, LinkedIn, or X links |
| **Hobbies & Dislikes** | Edit the list items (`<li>`) | Add or remove items as you wish |

---

## How It Works

The dynamic date display is handled using a small inline JavaScript script:
```javascript
const timeElement = document.querySelector('[data-testid="test-user-time"]');
timeElement.textContent = `Date: ${(new Date).toLocaleDateString()} (${Date.now()} ms)`;
```
This updates the date and timestamp when the page loads.

---

## Technologies Used

| Technology | Purpose |
|-------------|----------|
| **HTML5** | Page structure & semantic layout |
| **CSS3** | Styling and responsive design |
| **JavaScript (ES6)** | Dynamic date and time display |
| **Accessibility Attributes** | Better usability for assistive technologies |

---

## Best Practices Followed

- Semantic HTML for SEO and accessibility
- Minimal inline styling
- Clear separation of structure (HTML), style (CSS), and behavior (JS)
- Descriptive `alt` attributes for all images
- Externalized CSS for maintainability

---

## Preview

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

##  Author

**Ayeni Phillip Adetunji**  
Frontend Developer | Tech Enthusiast | Research & People-focused  

- 🌐 [LinkedIn](https://www.linkedin.com/in/ayeni-phillip-adetunji/)  
- 🐦 [X (Twitter)](https://x.com/ayenitunji?t=Qqilk_Ky-nZSnSFM_CtqQ&s=09)  
- 💻 [GitHub](https://github.com/ASPAT1)

---

## Contributing

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

## Final Notes

This project serves as a great **starter template** for building:
- Personal portfolios
- Developer introduction sections
- Resume or bio pages

Feel free to customize and build upon it!

---
# 📩 Contact Us Page

A simple, accessible, and responsive **Contact Us form** built using **HTML, CSS, and Vanilla JavaScript**.  
This project demonstrates form validation, accessibility best practices, and user feedback messages for successful or invalid submissions.

---

## 🧠 Project Overview

This project provides a **contact form interface** that allows users to send messages or inquiries.  
It includes client-side validation to ensure all inputs are filled correctly before submission, improving both usability and data quality.

The form includes the following fields:
- Full Name  
- Email Address  
- Subject  
- Message  

All fields are required, and users receive **real-time validation feedback** for incorrect or incomplete entries.

---

## 🖼️ Demo (Optional)
If you have a live demo hosted (for example, on GitHub Pages), you can add it here:

👉 [Live Demo Link](https://yourusername.github.io/contact-form)

---

## ✨ Features

✅ Semantic and accessible HTML structure  
✅ Custom error messages for invalid input  
✅ Client-side form validation using JavaScript  
✅ Success message shown after valid submission  
✅ Responsive layout using CSS  
✅ Proper use of `data-testid` attributes for testing  

---

## 🛠️ Technologies Used

| Technology | Purpose |
|-------------|----------|
| **HTML5** | Page structure and form markup |
| **CSS3** | Styling and responsive design |
| **JavaScript (Vanilla JS)** | Form validation and user feedback |

---

## ⚙️ How It Works

1. **User fills out the form** with their details (name, email, subject, and message).  
2. When the user clicks **“Send Message”**, JavaScript intercepts the submission using `event.preventDefault()`.  
3. Validation runs for each field:
   - **Name:** Must not be empty  
   - **Email:** Must match the pattern `name@example.com`  
   - **Subject:** Must not be empty  
   - **Message:** Must be at least 10 characters long  
4. If any validation fails, an error message is displayed below that field.  
5. If all validations pass, a success message appears:  
   > ✅ “Regards! Your message has been sent successfully.”  
   and the form resets automatically.

---

## 💻 File Structure

contact-us/
│
├── index.html # Main HTML file (Contact form)
├── contactme.css # Stylesheet for layout and design
└── README.md # Documentation (this file)
---

---

## 🧩 HTML Breakdown

### Main Sections:
- `<form>` element: wraps all form fields and handles the submit event.  
- `<label>` elements: provide accessible text for screen readers.  
- `<input>` and `<textarea>`: collect user information.  
- `<div class="error">`: display field-specific error messages.  
- `<div id="success">`: shows success feedback when the form is valid.

Each input uses:
```html
data-testid="test-contact-..." 
---
🧮 JavaScript Logic

The validation script:

Listens for the submit event on the form.

Uses regular expressions to validate email addresses.

Updates the DOM dynamically with feedback messages.

Uses form.reset() to clear all inputs after success.

Example of the email validation:

const emailPattern = /^[^ ]+@[^ ]+\.[a-z]{2,3}$/;
if (!email.value.match(emailPattern)) {
  document.getElementById('error-email').textContent = 'Enter a valid email (name@example.com).';
}

🎨 Styling Notes (from contactme.css)

While not shown here, the stylesheet (contactme.css) typically defines:

Form layout (.container)

Button styling

Error message color (e.g., red text)

Success message color (e.g., green text)

Responsive behavior for smaller screens

Example (typical CSS):

.error {
  color: red;
  font-size: 0.9rem;
}

.success {
  color: green;
  font-weight: bold;
}

🧭 Accessibility Considerations

Each input field uses a corresponding <label> for screen readers.

Error messages are linked via aria-describedby attributes.

Semantic HTML (label, input, textarea, button) ensures proper navigation for assistive technologies.

🚀 How to Run This Project Locally

Clone the repository:

git clone https://github.com/yourusername/contact-us-page.git


Open the folder:

cd contact-us-page


Open index.html in your browser.
(No additional setup required — it’s a plain HTML/CSS/JS project.)

🧑‍💻 Author

Your Name
📧 your.email@example.com

🌐 GitHub Profile

🪪 License

This project is open source and available under the MIT License
.

💬 Summary

This “Contact Us” form project is a great example of clean, accessible, and user-friendly front-end development using only HTML, CSS, and JavaScript.
It can be integrated into larger websites or used as a standalone page to collect user messages effectively.


---

Would you like me to **add your name and GitHub link** inside this README before you upload it?  
If yes — please send:
- Your **name**
- Your **GitHub username or profile link**

---
# 🌟 About Me Page (HTML + CSS)

This project is a simple **“About Me” web page** designed to help **students learn how to build semantic, accessible, and well-structured HTML pages**.  
It focuses on using proper HTML elements (`header`, `main`, `section`, `ul`, `p`, `h2`) and applying CSS for basic styling.

---

## 🎯 Learning Objectives

By studying this project, you will learn:

✅ How to structure a webpage using **semantic HTML elements**  
✅ How to use **headings**, **paragraphs**, and **lists** correctly  
✅ How to organize content inside meaningful **sections**  
✅ The purpose of **data-testid** attributes for testing or validation  
✅ How to link an external CSS file (`Aboutme.css`)  
✅ How to write clean, readable, and accessible HTML code  

---

## 🧩 Project Overview

The **About Me** page introduces a student or developer in a simple, clean format.  
It includes information such as:
- Personal bio  
- Goals in the program  
- Areas of low confidence  
- Notes to their future self  
- Extra thoughts or reflections  

This layout is useful for personal websites, portfolios, or training projects.

---

## 📁 File Structure

about-me/
│
├── index.html # The main HTML file (About Me page)
├── Aboutme.css # The external CSS stylesheet (linked in the HTML)
└── README.md # This documentation file

php-template
Copy code

---

## 🧠 Code Explanation

Let’s go through the important parts of the HTML step-by-step 👇

### 1. Document Setup

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>About Me</title>
  <link rel="stylesheet" href="Aboutme.css">
</head>
What this does:

<!DOCTYPE html>: Tells the browser this is an HTML5 document.

<html lang="en">: Declares the page language (important for accessibility).

<meta charset="UTF-8">: Ensures special characters display correctly.

<meta name="viewport">: Makes the page responsive on mobile devices.

<link rel="stylesheet" href="Aboutme.css">: Links the external CSS file.

2. Header Section
html
Copy code
<header>
  <h1>About Me</h1>
</header>
Purpose:
Displays the page title using a top-level heading (<h1>).
The <header> tag makes it semantically clear that this part is the introduction.

3. Main Content Area
html
Copy code
<main data-testid="test-about-page">
The <main> tag holds the core content of the page — what the page is truly about.
It’s used for accessibility and screen readers to identify the main information.

4. Bio Section
html
Copy code
<section data-testid="test-about-bio">
  <h2>My Bio</h2>
  <p> ... </p>
</section>
Explanation:

<section> groups related information together.

<h2> is used for subheadings (since <h1> is already used in the header).

<p> defines paragraphs of text that describe you.

5. Goals Section
html
Copy code
<section data-testid="test-about-goals">
  <h2>Goals in This Program</h2>
  <ul>
    <li>Master front-end frameworks like React.</li>
    <li>Improve my understanding of accessibility and responsive design.</li>
    <li>Collaborate with peers to build real-world projects.</li>
  </ul>
</section>
Learning Points:

<ul> defines an unordered list.

<li> defines individual list items.
Lists are useful when presenting goals, steps, or key points.

6. Confidence & Future Note Sections
Each section follows the same pattern — a heading and a paragraph describing your thoughts or learning progress.
This helps break down the content logically, making it easier for both readers and screen readers.

7. Extra Thoughts Section
html
Copy code
<section data-testid="test-about-extra">
  <h2>Extra Thoughts</h2>
  <p>I believe teamwork and continuous feedback are key...</p>
</section>
This is an example of a custom or flexible section that students can adapt — maybe to add hobbies, reflections, or personal values.

🧪 About data-testid Attributes
Throughout the code, you’ll notice attributes like:

html
Copy code
data-testid="test-about-bio"
These are not for users — they are mainly used by automated testing tools (like Jest, Cypress, or Playwright) to check whether specific parts of the page exist and work as expected.
For example, a test could confirm that:

The Bio section is present

The Goals list exists

Each heading has proper structure

This helps ensure your code meets the acceptance criteria for assignments or automated grading systems.

🎨 Styling (Aboutme.css)
Although not shown here, the Aboutme.css file controls how the page looks — including:

Colors

Fonts

Layout (padding, margins)

Responsive design for small screens

Example snippet (you can add this to your CSS):

css
Copy code
body {
  font-family: 'Poppins', sans-serif;
  background-color: #f9f9f9;
  color: #333;
  line-height: 1.6;
  margin: 20px;
}

h1, h2 {
  color: #2b59c3;
}

section {
  margin-bottom: 1.5rem;
}
💻 How to View This Project
Download or clone the project:

bash
Copy code
git clone https://github.com/yourusername/about-me-page.git
Open the folder:

bash
Copy code
cd about-me-page
Double-click index.html to open it in your browser.
(No server required — this runs locally.)

🧠 Key Takeaways for Students
Always use semantic tags (main, section, header) instead of just <div>.

Keep content organized and accessible for everyone.

Use CSS for styling — never inline styles in HTML.

Write clean, readable, and consistent code with indentation.

Use meaningful headings (h1, h2, etc.) in the correct order.

Keep learning by improving small projects like this.

👨‍💻 Author / Student Info
Your Name Here
📧 your.email@example.com
🌐 GitHub Profile

🪪 License
This project is open-source and free to use for educational purposes.

💬 Final Thoughts
This About Me page is an excellent foundation for beginners learning HTML and CSS.
It encourages semantic coding, accessibility awareness, and proper structure — the building blocks of every great web developer.

yaml
Copy code

---

Would you like me to include **example CSS styling** (Aboutme.css) that would make this page look visually appealing and student-friendly too?  
I can add that next so your README has a complete guide.







