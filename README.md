&nbsp;

<div align="center">
<img src="https://github.com/jaredhud/QuikDine-mobile/blob/main/src/img/quik-dine.png?raw=true" alt="QuikDine logo" style="height:80px" />
<br>
Recipe made Easy! - Server Repo
</div>
&nbsp;
<div align="center">
<img src="https://badge.fury.io/js/npm.svg"> <img src="https://img.shields.io/badge/compatible-iOS%20%26%20android-blue" > 
<a href="https://spoonacular.com/food-api"> <img src="https://img.shields.io/badge/API-Spoonacular-orange"> </a>
<a href="https://cloud.google.com/vision/"> <img src="https://img.shields.io/badge/API-Google%20Vision-orange"> </a>
</div>

&nbsp;
<div align="center">
<img src="https://github.com/jaredhud/QuikDine-mobile/blob/main/src/img/architecture.jpg?raw=true" alt="QuikDine logo" style="width:100%">
</div>

&nbsp;
<div>
<a href="https://www.youtube.com/watch?v=kbyUfBJmxLE">
  <img src="https://img.shields.io/badge/DEMO%20-YOUTUBE VID%20%E2%86%92-gray.svg?colorA=5d5d5d&colorB=b30b00&style=for-the-badge" />
<a href="https://github.com/jaredhud/QuikDine-mobile/tree/main/src/img/IU C9 P3 G3.pdf">
<img src="https://img.shields.io/badge/PDF%20-DIGITAL FLYER%20%E2%86%92-gray.svg?colorA=5d5d5d&colorB=ff7605&style=for-the-badge"/></a>
&nbsp;
</div>

# 🍽️ QuikDine — Server

**Recipe discovery made easy.**

QuikDine helps you decide what to eat using the ingredients you already have.

Scan items in your pantry, discover recipes based on those ingredients, save your favorites, and invite family or friends to vote on what's for dinner!

This repository contains the **server component** of the QuikDine application.

---

## 📑 Table of Contents

- [About QuikDine](#-about-quikdine)
- [How It Works](#-how-it-works)
- [Key Features](#-key-features)
- [Project Architecture](#️-project-architecture)
- [Server Responsibilities](#️-server-responsibilities)
- [Technologies Used](#️-technologies-used)
- [Installation](#-installation)
- [Project Repositories](#-project-repositories)
- [Team](#-team)
- [Development Notes](#-development-notes)
- [Credits](#-credits)

---

## 📖 About QuikDine

Choosing what to cook can be difficult — especially when you don't know what meals you can make with the ingredients already sitting in your kitchen.

QuikDine makes that decision easier.

The application allows users to scan or enter ingredients from their pantry and receive recipe suggestions based on what they have available.

Found several good options?

Invite family or friends and let everyone vote on what to make for dinner.

---

## 🔄 How It Works

```text
SCAN OR ENTER
PANTRY ITEMS
      │
      ▼
 IDENTIFY INGREDIENTS
      │
      ▼
  QUIKDINE SERVER
      │
      ▼
 SPOONACULAR API
      │
      ▼
 RECIPE SUGGESTIONS
      │
      ▼
 SAVE FAVORITES
      │
      ▼
 SHARE & VOTE
      │
      ▼
WHAT'S FOR DINNER?
```

QuikDine connects ingredient recognition, recipe discovery, saved recipes, and group voting into one workflow.

---

## ✨ Key Features

### 📸 Item QuikShot

Add pantry items using your camera or by entering them manually.

### 🔎 Recipe Finder

Find recipe suggestions based on ingredients available in your pantry.

### 🗳️ Recipe Selector

Share recipe choices with family or friends and vote on which meal to make.

Additional participants can be added to the voting process.

### ❤️ Recipe Storage

Create an account and save favorite recipes for later.

### 📱 Cross-Platform Mobile App

The QuikDine mobile application is designed to work across both Android and iOS.

---

## 🏗️ Project Architecture

QuikDine is divided into three main applications:

```text
                 QUIKDINE
                     │
       ┌─────────────┼─────────────┐
       │             │             │
       ▼             ▼             ▼
  MOBILE APP       SERVER        WEBSITE
React Native     Node.js /       React
    Expo          Express
       │             │             │
       │             ▼             │
       │      SPOONACULAR API      │
       │             │             │
       │          FIREBASE         │
       │             │             │
       └─────────────┼─────────────┘
                     │
                     ▼
              QUIKDINE DATA
```

### 📱 Mobile

The mobile application provides the primary QuikDine experience, including pantry management, recipe discovery, and mobile navigation.

### ⚙️ Server

The server handles application logic and communication with external services such as the Spoonacular API.

### 🌐 Website

The web application supports recipe voting so multiple people can participate in choosing a meal.

---

## ⚙️ Server Responsibilities

This repository contains the **QuikDine server application**.

The server acts as the bridge between QuikDine and external services required by the application.

Its responsibilities include:

- communicating with the Spoonacular API
- retrieving recipe information
- supporting recipe searches
- processing application requests
- supporting stored recipe data
- connecting application functionality with backend services

---

## 🛠️ Technologies Used

### Mobile & Frontend

- React Native
- React
- JavaScript
- HTML
- CSS
- Expo
- Expo Go

### Backend

- Node.js
- Express.js
- JavaScript

### Data & Services

- Firebase
- Spoonacular API
- Google Vision API
- SendGrid

### Design & Collaboration

- Git
- GitHub
- Figma
- Trello
- Basecamp
- Discord
- Zoom

---

## 🚀 Installation

QuikDine consists of multiple repositories that work together.

### Requirements

Make sure you have installed:

- Node.js
- npm
- Git
- Expo CLI

### 1. Clone the mobile application

```bash
git clone https://github.com/jaredhud/QuikDine-mobile.git
```

### 2. Clone the server

```bash
git clone https://github.com/jaredhud/Quikdine-server.git
```

### 3. Clone the website

```bash
git clone https://github.com/Kshitija118/QuikDineWebPage.git
```

### 4. Install dependencies

Run the following inside each project directory:

```bash
npm install
```

### 5. Start the applications

Run the appropriate start command inside each repository:

```bash
npm run start
```

Additional configuration may be required for Firebase and external API services.

---

## 📦 Project Repositories

QuikDine is separated into three repositories:

### 📱 Mobile Application

```text
QuikDine-mobile
```

The React Native mobile application used for the primary user experience.

### ⚙️ Server

```text
Quikdine-server
```

The backend application responsible for server functionality and external API communication.

### 🌐 Website

```text
QuikDineWebPage
```

The web application used to support recipe voting and shared meal selection.

---

## 👥 Team

QuikDine is developed by the **Eggroll Team**:

- **Kshitija Shirsathe**
- **Romell Bermundo**
- **Jared Huddleston**
- **Chris Desmarais** — Scrum Master

The team collaborates across application development, UI/UX, backend services, API integration, testing, and project coordination.

---

## 📝 Development Notes

### Data

Firebase is used to store application data.

### Email

SendGrid handles email functionality.

### Navigation

The mobile application uses both screen navigation and tab navigation.

Folders such as `_RecipeNav` handle tab-navigation functionality.

### Modals

Modals are used to create pop-ups and contextual information such as help notes.

### Layout

Percentage-based sizing can be used when dividing page sections to support responsive layouts.

### State & Data Transfer

React Context is used to transfer application data between different parts of the application.

---

## 🎯 Project Goal

Our goal with QuikDine is simple:

> **Make deciding what's for dinner easier.**

By combining pantry scanning, recipe discovery, saved recipes, and group voting, QuikDine turns ingredients already available at home into practical meal ideas.

At the same time, the project brings together mobile development, backend development, APIs, cloud data storage, computer vision, and collaborative software development into one integrated application.

---

## 🙏 Credits

QuikDine uses several open-source technologies and third-party services, including:

- Node.js
- React
- React Native
- Express
- Firebase
- Expo
- Spoonacular
- Google Vision API
- SendGrid

Base logo vector created by **Freepik** from **Flaticon**.
