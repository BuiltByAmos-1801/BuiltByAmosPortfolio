
---

# 🌐 BuiltByAmosPortfolio

[![Build Status](https://img.shields.io/badge/build-passing-brightgreen)](https://github.com/BuiltByAmos-1801/BuiltByAmosPortfolio/actions)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](./LICENSE)
[![Issues](https://img.shields.io/github/issues/BuiltByAmos-1801/BuiltByAmosPortfolio.svg)](https://github.com/BuiltByAmos-1801/BuiltByAmosPortfolio/issues)
[![Stars](https://img.shields.io/github/stars/BuiltByAmos-1801/BuiltByAmosPortfolio.svg)](https://github.com/BuiltByAmos-1801/BuiltByAmosPortfolio/stargazers)
[![Forks](https://img.shields.io/github/forks/BuiltByAmos-1801/BuiltByAmosPortfolio.svg)](https://github.com/BuiltByAmos-1801/BuiltByAmosPortfolio/network)
[![Website](https://img.shields.io/badge/website-live-blue)](https://builtbyamos.vercel.app)
[![Made by Amos Anand](https://img.shields.io/badge/made%20by-Amos%20Anand-orange)](https://github.com/BuiltByAmos-1801)

---

## 🧠 About The Project

Welcome to **BuiltByAmosPortfolio** — a personal portfolio and professional guide that documents my full development workflow using **GitHub**, **Termux**, and **Android Studio (Kotlin)**.  
This project not only showcases my portfolio but also includes a **complete guide** on how to set up, connect, and deploy your own GitHub repositories directly from **Termux**.

---

## 🚀 Features

✅ Responsive Portfolio Website  
✅ Termux + GitHub full setup commands  
✅ Step-by-step deployment guide  
✅ Kotlin Android app sample project  
✅ Professional README structure  
✅ Git error fix documentation  
✅ Badges, credits, and license setup  

---

## 🧰 Tech Stack

| Category | Tools |
|-----------|-------|
| **Frontend** | HTML5, CSS3, JavaScript |
| **Backend** | Node.js (optional setup) |
| **Mobile** | Kotlin, Android Studio |
| **Version Control** | Git, GitHub |
| **Terminal Setup** | Termux |
| **Deployment** | GitHub Pages, Vercel |
| **Design Tools** | Figma, Canva |

---

## 🧑‍💻 Developer Info

**Name:** Amos Anand  
**Brand:** BuiltByAmos  
**Location:** Bangalore, India (from Garhwa, Jharkhand)  
**Roles:** Software Developer | UI/UX Designer | Freelancer | YouTuber | Blogger  
**Email:** builtbyiamos@gmail.com  
**GitHub:** [BuiltByAmos-1801](https://github.com/BuiltByAmos-1801)

---

## ⚙️ Step 1: Setting Up Termux & GitHub Integration

Below are the complete steps to connect **Termux** to **GitHub** and push code seamlessly.

### 🧩 Install Git in Termux

```bash
pkg update && pkg upgrade
pkg install git

📂 Configure Git

git config --global user.name "BuiltByAmos-1801"
git config --global user.email "builtbyiamos@gmail.com"

🔑 Generate SSH Key

ssh-keygen -t rsa -b 4096 -C "builtbyiamos@gmail.com"
cat ~/.ssh/id_rsa.pub

Copy the generated SSH key and add it to your GitHub → Settings → SSH and GPG keys → New SSH Key.


---

🧱 Step 2: Creating a New Repository on GitHub

1. Go to GitHub


2. Enter Repository name → BuiltByAmosPortfolio


3. Description → My official portfolio and setup guide.


4. Choose Public


5. Click on Create Repository




---

🌿 Step 3: Connect Termux to GitHub Repo

git clone https://github.com/BuiltByAmos-1801/BuiltByAmosPortfolio.git
cd BuiltByAmosPortfolio

If you already have files locally:

git init
git remote add origin https://github.com/BuiltByAmos-1801/BuiltByAmosPortfolio.git
git add .
git commit -m "Initial website deployment"
git push -u origin main


---

🧩 Step 4: Handling Common Errors

❌ Error 403: Permission Denied

Fix:

git remote remove origin
git remote add origin https://BuiltByAmos-1801@github.com/BuiltByAmos-1801/BuiltByAmosPortfolio.git

❌ Error: Authentication Failed

Fix: Use a GitHub Personal Access Token (PAT) instead of a password.

Create one from:
👉 GitHub → Settings → Developer Settings → Personal Access Tokens → Fine-grained token

Then run:

git remote set-url origin https://<username>:<token>@github.com/<username>/<repo>.git


---

📱 Step 5: Kotlin Android Project (Example)

Create a simple Hello User app in Android Studio using Kotlin.

🧩 MainActivity.kt

package com.example.hellouser

import androidx.appcompat.app.AppCompatActivity
import android.os.Bundle
import android.widget.Button
import android.widget.Toast

class MainActivity : AppCompatActivity() {
    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)
        setContentView(R.layout.activity_main)

        val btn = findViewById<Button>(R.id.button)
        btn.setOnClickListener {
            Toast.makeText(this, "Hello User!", Toast.LENGTH_SHORT).show()
        }
    }
}


---

🖥️ Step 6: Portfolio Website Folder Structure

BuiltByAmosPortfolio/
│
├── index.html
├── about.html
├── services.html
├── contact.html
├── css/
│   ├── style.css
│   └── responsive.css
├── js/
│   └── main.js
├── images/
│   └── author.jpeg
└── README.md


---

🎨 CSS Snippet Example

.img-about img {
  width: 100%;
  height: auto;
  border-radius: 20px;
  object-fit: cover;
  display: block;
  margin: auto;
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}


---

💡 Pro Tips

Always commit with clear messages

Use .gitignore to skip node_modules or build files

Deploy portfolio using GitHub Pages or Vercel

Add project screenshots under /images folder

Keep README updated with your latest features



---

🧩 Example Commands Recap

git status
git add .
git commit -m "Updated portfolio design"
git push origin main


---

🧾 Example README Badges Section

[![GitHub repo size](https://img.shields.io/github/repo-size/BuiltByAmos-1801/BuiltByAmosPortfolio)]
[![Contributors](https://img.shields.io/github/contributors/BuiltByAmos-1801/BuiltByAmosPortfolio)]
[![Last Commit](https://img.shields.io/github/last-commit/BuiltByAmos-1801/BuiltByAmosPortfolio)]


---

📑 Documentation Structure

📘 Documentation/
│
├── 01-Termux-Setup.md
├── 02-GitHub-Connection.md
├── 03-Error-Fixes.md
├── 04-Portfolio-Design.md
├── 05-Kotlin-App.md
├── 06-Deployment-Guide.md
└── README.md


---

🧩 License

This project is licensed under the MIT License.
You are free to use, modify, and distribute this project for educational and personal use.


---

🤝 Contributing

Contributions are welcome!

1. Fork the repository


2. Create a new branch (feature/my-feature)


3. Commit changes


4. Push and submit a Pull Request




---

💬 Contact & Support

📧 Email: builtbyiamos@gmail.com

🌐 Website: builtbyamos.vercel.app

🐙 GitHub: BuiltByAmos-1801

💼 LinkedIn: Amos Anand



---

🌟 Acknowledgments

Termux Project

Android Studio

GitHub Docs

Canva & Figma

All open-source contributors ❤️



---

✨ Final Thoughts

> “Consistency builds expertise — and expertise builds freedom.”
— Amos Anand (BuiltByAmos)



Keep building. Keep learning. Keep sharing.
Thank you for visiting my portfolio repository 🙌


---

📜 Version History

Version	Date	Description

1.0	Oct 2025	Initial portfolio and Termux setup
1.1	Oct 2025	Added Kotlin app example
1.2	Oct 2025	Fixed push error and added docs
1.3	Oct 2025	Final release with 400-line README



---

🧠 Keywords for SEO

#AmosAnand #BuiltByAmos #TermuxSetup #GitHub #WebDevelopment
#KotlinApp #PortfolioWebsite #UIUXDesign #Freelancer #BangaloreDeveloper


---

---

