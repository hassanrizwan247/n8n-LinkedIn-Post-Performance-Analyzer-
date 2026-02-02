# LinkedIn Post Performance Analyzer (n8n)

This project is a fully automated LinkedIn post analytics workflow built using **n8n** and **100% free tools**.

It allows creators, students, and professionals to analyze the performance of their LinkedIn posts by collecting post data, categorizing post length, evaluating engagement-based success, storing analytics, and sending automated performance summary emails.

> ⚠️ Important: This project was built completely independently without using AI-generated logic or external automation templates.

---

## 🚀 Features

- Custom form to manually submit LinkedIn post data
- Automatic post length calculation (Short / Medium / Long)
- Rule-based post performance classification (Successful / Unsuccessful)
- Google Sheets integration for analytics storage
- Automated email notification with post performance summary
- Clean, structured, and scalable n8n workflow design

---

## 🛠️ Tech Stack (Free Only)

- **n8n** (Self-hosted)
- **Google Sheets**
- **Gmail**
- **n8n Form Trigger**

No paid APIs or external services are used.

---

## 🧠 Workflow Logic Overview

### 1️⃣ Data Collection
A form trigger collects:
- Post title
- Post time
- Post type (Text / Image / Carousel)
- Impressions after 24 hours
- Likes, comments, reposts, saves
- Full post text

---

### 2️⃣ Post Length Classification
- The workflow calculates the character length of the post text.
- Posts are categorized into:
  - **Short**
  - **Medium**
  - **Long**

This helps analyze how content length affects engagement.

---

### 3️⃣ Performance Evaluation
Posts are classified as **Successful** if **any** of the following conditions are met:
- Impressions ≥ 5000
- Likes ≥ 50
- Comments ≥ 20

Otherwise, the post is marked as **Unsuccessful**.

---

### 4️⃣ Data Storage
All post data and calculated insights are automatically:
- Appended or updated in Google Sheets
- Matched using the post title
- Stored with post length and performance criteria

---

### 5️⃣ Email Notification
An automated email is sent containing:
- Post title
- Impressions after 24 hours
- Likes, comments, reposts, saves
- Final performance status (Successful / Unsuccessful)

---

## 📊 Use Cases

- LinkedIn creators tracking content performance
- Students learning analytics-driven content strategy
- Freelancers demonstrating automation & data logic skills
- Portfolio project for automation roles

---

## 📂 Repository Structure

