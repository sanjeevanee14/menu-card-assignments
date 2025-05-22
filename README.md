# 🧾 JavaScript Menu Card Component using Web Components

## 📌 Project Overview

This project is developed and maintained by **Maha Mission Education and Career Council (NGO)** under its innovative skill-based learning initiative at **ApnaGuru.in**. This assignment is technically supported by **Apnasite IT Services Pvt. Ltd.**, providing:

✅ **Frontend training and mentorship**\
✅ **Deployment and versioning**\
✅ **Ongoing platform maintenance**

**🌐 Live Preview:**
[https://menu-card.apnasite.in](https://menu-card.apnasite.in)\
**🧑‍🏫 Learn with Us:** [https://apnaguru.in](https://aapn.in/M7PM3JB5)\
**📢 NGO Info:** [https://mmeac.org](https://mmeac.org)\
**🏢 Company:** [https://apnasite.in](https://apnasite.in)\
**📞 Contact:** +91-8999417889 (Call/WhatsApp)

---

## 🧭 Goal

Create a **custom Web Component** called `<menu-card>` that renders a restaurant-style menu using:

* ✅ **JavaScript’s DOM API** only (no external frameworks like React or Vue)
* ✅ **Web Components** (using `class extends HTMLElement`)
* ✅ **Dynamic `config` and `data` attributes** to control styling and menu content
* ✅ **Reusable structure** for integrating menus in any restaurant or food-ordering website
* ✅ **Bootstrap** (for responsive layout and design)

---

## 🔗 Deployment Format

`https://services.apnasite.in/menu-card-assignments/[YourName_AssignmentNumber]/preview.html`

**Example:**
[https://services.apnasite.in/menu-card-assignments/Mahesh\_Bhosle\_21/preview.html](https://services.apnasite.in/menu-card-assignments/Mahesh_Bhosle_21/preview.html)

---

## 📁 Folder Structure

```
menu-card-assignments/
 ┣ 📂 SubmittedAssignments/
 ┃ ┗ 📂 [Your_Name_XX]/
 ┃    ┣ 📜 preview.html     // Menu card demo with dynamic content
 ┃    ┣ 📜 script.js        // JS Web Component for <menu-card>
 ┃    ┣ 📜 data.json        // Sample JSON for 'data' and 'config'
 ┃    ┣ 📂 IMG/             // Menu images and assets
 ┃    ┣ 📂 css/             // Custom CSS (if required)
 ┃    ┗ 📂 fonts/           // Fonts (optional)
```

---

## 🧱 Component Specifications

### 🔸 `<menu-card>` Web Component

A full-screen restaurant menu component that dynamically displays:

* 🍕 Restaurant Name and Description
* ☎️ Contact Info (Phone, Web, Email)
* 🧾 Menu Categories (e.g., Pizza, Burger)
* 🖼️ Category-wise Image
* 💵 Item List with Names and Prices

### ✅ Attributes Accepted:

#### 1. `data` (JSON structure of restaurant and menu)

Includes:

* Restaurant details (`name`, `description`, `phone`, `web`, `email`)
* Menu list (categories, image, item names, prices)

#### 2. `config` (Optional UI customization)

Includes:

* Class names for wrappers, sections, text, images, etc.
* Allows flexible theming of the layout

---

## 🎯 Functional Features

* 👨‍🍳 Fully encapsulated component using Shadow DOM concept
* ⚙️ Customization via `data` and `config` JSON
* 🔄 Live rendering on attribute change (`observedAttributes`)
* 📦 Bootstrap utility classes used for responsiveness

---

## 🧪 Example `data` Structure

```json
{
  "restaurant": {
    "name": "FAUGET",
    "description": "BAKERY",
    "phone": "+91 0987654321",
    "web": "www.reallygratsite.com",
    "email": "reallygratsite@gmail.com"
  },
  "menu": [
    {
      "heading": "PIZZA",
      "image": "./IMG/img11.jpg",
      "imageClass": "img1 img-hover",
      "items": [
        { "name": "Pan Pizza", "price": 100 },
        { "name": "Butter Pizza", "price": 120 }
      ]
    }
  ]
}
```

---

## 🧾 `form.json` Structure

Use `form.json` to define a **Formly-compatible** input form that includes:

* Data fields (for component content)
* Config fields (for assigning Bootstrap classes)

---

## 🧪 Example DOM Structure (Card Component)

```javascript
const card = document.createElement("div");
card.className = config.cardClass || "card";

const title = document.createElement("h5");
title.className = config.titleClass || "card-title";
title.innerText = data.title;

card.appendChild(title);
this.appendChild(card);
```

---

## 🚀 Submission Process

### 1. 📦 Fork the Repository

👉 [https://github.com/Apnasite/menu-card-assignments](https://github.com/Apnasite/menu-card-assignments)

### 2. 💻 Clone Your Forked Repo

```bash
git clone https://github.com/YOUR_USERNAME/menu-card-assignments.git
```

### 3. 🧩 Create Your Assignment Folder

```bash
mkdir SubmittedAssignments/Your_Name_01
```

### 4. 🛠️ Copy and Build

Copy the sample folder structure and implement your solution inside `script.js`, `preview.html`, and `form.json`.

### 5. ✅ Commit and Push

```bash
git add .
git commit -m "Added Menu Card Assignment - Your_Name_01"
git push origin main
```

### 6. 🔃 Create Pull Request

After pushing your changes to your forked repository:

1. Go to your forked repository on GitHub.
2. Click the **"Compare & pull request"** button, or go to the "Pull requests" tab and click **"New pull request"**.
3. Set the base repository to `Apnasite/menu-card-assignments` and the base branch to `main`.
4. Compare with your fork and branch containing your assignment.
5. Add a clear title and description for your PR (e.g., "Added Menu Card Assignment - Your_Name_01").
6. Review your changes, then click **"Create pull request"**.

Your submission will be reviewed and feedback will be provided if needed.
