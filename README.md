# 🐙 Association 404 - Official Website

![Vercel Deployment](https://therealsujitk-vercel-badge.vercel.app/?app=asso-404-miashs)
![License](https://img.shields.io/badge/license-MIT-blue.svg)
![React](https://img.shields.io/badge/react-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB)
![Firebase](https://img.shields.io/badge/firebase-%23039BE5.svg?style=flat&logo=firebase)

Welcome to the official repository for the **Association 404** website. This project aims to centralize information, events, and student projects for the MIASHS department at the University Toulouse - Jean Jaurès[cite: 17, 20].

## 👥 The Team

This project is developed as part of the Requirements Engineering module in **M2 MIASHS ICE-LD**.

| Member | Role | GitHub |
| :--- | :--- | :--- |
| **Mathis DUGUE** | **Product Owner & Fullstack Dev**<br>*(Representative of the Association 404 Bureau)* [cite: 7] | [@MathisDugue](https://github.com/MathisDugue) |
| **Matthias LABIT** | **Scrum Master & Lead Dev**<br>*(QA & PEGS Implementation)* | [@MatthiasLabit](https://github.com/MatthiasLabit) |

## 📚 PEGS Approach & Requirements

We followed the **PEGS** (Project, Environment, Goals, System) methodology to define and structure the requirements of this application.

👉 **[Click here to view the Full Requirements Document (REQUIREMENTS.md)](./REQUIREMENTS.md)**

The development process is driven by these requirements:
* **Issues** are linked to specific requirements (e.g., `REQ-F-01`).
* **Prioritization** follows the **MoSCoW** method (Must, Should, Could, Won't).

## 🚀 Project Overview

### Context
The Association 404 lacked a centralized digital presence. Students and partners had difficulty finding information about events or contacting the team[cite: 20].

### Goals
1.  **Centralize Information:** A single point of entry for all association news and missions[cite: 22].
2.  **Showcase Projects:** A "Showcase" section to highlight student work to recruiters[cite: 23, 62].
3.  **Event Management:** Allow the board to manage events dynamically without coding[cite: 27].

## 🛠️ Tech Stack

This project is built with modern web technologies focusing on performance and maintainability[cite: 81, 82, 83]:

* **Front-end:** React, TypeScript, Tailwind CSS
* **Back-end (BaaS):** Google Firebase (Auth, Firestore, Storage)
* **Hosting / CI-CD:** Vercel

## 💻 Getting Started

### Prerequisites
* Node.js (v16+)
* npm or yarn

### Installation

1.  **Clone the repository**
    ```bash
    git clone [https://github.com/votre-username/asso-404-website.git](https://github.com/votre-username/asso-404-website.git)
    cd asso-404-website
    ```

2.  **Install dependencies**
    ```bash
    npm install
    ```

3.  **Configure Environment Variables**
    Create a `.env.local` file in the root directory and add your Firebase credentials:
    ```env
    VITE_FIREBASE_API_KEY=your_api_key
    VITE_FIREBASE_AUTH_DOMAIN=your_project.firebaseapp.com
    VITE_FIREBASE_PROJECT_ID=your_project_id
    # ... other firebase config
    ```

4.  **Run the development server**
    ```bash
    npm run dev
    ```

## 📸 Screenshots

| Landing Page | Events Section |
|:---:|:---:|
| <img src="./public/screenshots/landing.png" width="400" alt="Landing Page"> | <img src="./public/screenshots/events.png" width="400" alt="Events"> |

> *Note: Dark mode is supported natively.* [cite: 37]

## 📄 License

This project is open-source and available under the MIT License.