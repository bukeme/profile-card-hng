# 🚀 Profile Card — Testable Frontend Component

This project is a **responsive, accessible Profile Card** built using **HTML, CSS, and Vanilla JavaScript only**, as part of the *Frontend Wizards Stage 1B Task*.

It follows strict requirements such as:

* Semantic HTML structure
* Accessibility best practices
* Responsive design
* Testability using `data-testid` attributes

---

## 📌 Features

* ✅ Semantic HTML (`article`, `header`, `section`, `nav`, `figure`)
* ✅ Fully responsive layout (mobile → desktop)
* ✅ Accessible (ARIA attributes, keyboard navigation, focus states)
* ✅ Live updating **epoch time (milliseconds)**
* ✅ Avatar support:

  * Image URL input
  * File upload
* ✅ Social links (open in new tab securely)
* ✅ Clearly separated:

  * Hobbies list
  * Dislikes list
* ✅ All required `data-testid` attributes included

---

## 📁 Project Structure

```
profile-card/
│
├── index.html     # Main application (HTML + CSS + JS)
└── README.md      # Project documentation
```

---

## 🛠️ How to Run Locally

### Option 1 — Simple (Recommended)

1. Download or clone the project
2. Open the folder
3. Double-click `index.html`

OR

```bash
open index.html
```

---

### Option 2 — Using Live Server (Better for development)

If you use VS Code:

1. Install **Live Server extension**
2. Right-click `index.html`
3. Click **"Open with Live Server"**

---

### Option 3 — Using Python server

```bash
python -m http.server 8000
```

Then open:

```
http://localhost:8000
```

---

## 🧪 Testing Notes

This project is designed to be tested using **automated UI tests** via `data-testid` attributes.

### Required Test IDs Implemented

| Element          | data-testid              |
| ---------------- | ------------------------ |
| Root card        | `test-profile-card`      |
| Name             | `test-user-name`         |
| Bio              | `test-user-bio`          |
| Time             | `test-user-time`         |
| Avatar           | `test-user-avatar`       |
| Social container | `test-user-social-links` |
| Hobbies list     | `test-user-hobbies`      |
| Dislikes list    | `test-user-dislikes`     |

### Time Validation

* Uses `Date.now()`
* Updates every **1000ms**
* Tests should allow small delay tolerance (~1s)

---

## ♿ Accessibility Notes

* All images include meaningful `alt` text
* `aria-live="polite"` used for time updates
* Keyboard navigation:

  * All links are tabbable
  * Buttons and inputs are accessible
* Focus states are clearly visible
* Color contrast meets WCAG AA standards

---

## 📱 Responsiveness

| Screen Size | Layout                     |
| ----------- | -------------------------- |
| Mobile      | Stacked (vertical)         |
| Tablet      | Semi-grid                  |
| Desktop     | Avatar left, content right |

---

## 🔗 Social Links Behavior

* Open in new tab using:

  ```html
  target="_blank" rel="noopener noreferrer"
  ```

---

## ⚠️ Notes for Reviewers

* No frameworks or libraries were used
* Everything is implemented using:

  * HTML
  * CSS (Flexbox + Grid)
  * Vanilla JavaScript
* All required elements are present and testable

---

## 🧠 Possible Improvements (Not required)

* Add dark mode
* Persist avatar using localStorage
* Add edit profile functionality
* Add animations/transitions

---

## 👨‍💻 Author

Ukeme Bassey
Frontend Developer
