# 🌙 Lammet Ramadan (The Islamic Facebook)

A comprehensive Islamic social media platform specially developed for the holy month of Ramadan.

**Lammet Ramadan** aims to bring loved ones together, encourage acts of worship, and create a spiritually uplifting social experience where users can share meaningful posts, messages, and moments throughout Ramadan.

The application features a modern interface, elegant visual effects, and complete support for **Light & Dark themes** to deliver a beautiful and immersive user experience.

---

## 🔥 Key Features

### 🔐 Authentication System

* Smooth and secure user sign-up and login flow
* Fast **Google Sign-In** integration
* Secure Firebase-powered account management

### 📝 Social Interaction (Posts)

* Publish text and image posts
* Like posts in real time
* Add and view comments instantly
* Save posts using bookmarks for later access

### 💬 Real-Time Chat

* Private direct messaging system between friends
* Instant messaging experience
* Unread messages counter for better engagement

### 👥 Pages & Groups

* Create public pages and community groups
* Join and follow communities
* Stay updated with posts and activities

### 🔔 Instant Notifications

Receive real-time alerts for:

* Friend requests
* New messages
* Likes
* Comments
* Social activity updates

---

## 🌙 Spiritual & Ramadan Features

### ⏳ Ramadan Countdown

A smart countdown timer to track the remaining time until the arrival of Ramadan.

### 🤲 Daily Duas

Fresh, daily renewed Islamic supplications to inspire spiritual consistency.

### 📿 Azkar & Dhikr Counter

Interactive counters for:

* Daily Azkar
* Dhikr
* Prayers upon the Prophet ﷺ

### 🏆 Reward & Streak System

Motivational reward mechanics designed to encourage:

* Daily worship consistency
* Habit building
* Ramadan spiritual goals

---

## 🛠️ Tech Stack

### Frontend

* **HTML5**
* **CSS3**

  * Glassmorphism UI effects
  * Smooth transitions and animations

### Styling Framework

* **Tailwind CSS**

  * Fully responsive layout
  * Modern utility-first styling system
  * Mobile-first design philosophy

### Backend & Database

Powered by **Firebase Suite**:

#### Firebase Authentication

Secure authentication and account management.

#### Cloud Firestore

Real-time NoSQL database for managing:

* Users
* Posts
* Chats
* Notifications
* Groups & Pages

#### Firebase Storage

Media hosting for:

* Profile images
* Cover photos
* Post uploads

---

## 📂 Firestore Architecture

Cloud Firestore is organized to ensure scalability, clean architecture, and fast querying.

```txt
fb_users
├── User Profile Data
│   ├── Name
│   ├── Email
│   ├── Bio
│   └── Friends List

fb_posts
├── Posts Data
└── comments (Subcollection)

fb_chats
├── Private Chats
└── messages (Subcollection)

fb_notifications
└── Real-time User Notifications

fb_pages
└── Public Pages Data

fb_groups
└── Community Groups Data
```

### Collections Overview

| Collection         | Purpose                                                     |
| ------------------ | ----------------------------------------------------------- |
| `fb_users`         | Stores user profile information (Name, Email, Friends, Bio) |
| `fb_posts`         | Handles posts, likes, and comments                          |
| `fb_chats`         | Manages private messaging                                   |
| `fb_notifications` | Tracks user notifications in real time                      |
| `fb_pages`         | Handles public pages                                        |
| `fb_groups`        | Handles community groups                                    |

---

## 🚀 Setup & Installation

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/lammet-ramadan.git
```

### 2. Configure Firebase

Open your Firebase initialization file (`app.js` or equivalent) and replace the placeholder configuration with your Firebase project credentials:

```javascript
const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "YOUR_AUTH_DOMAIN",
  projectId: "YOUR_PROJECT_ID",
  storageBucket: "YOUR_STORAGE_BUCKET",
  messagingSenderId: "YOUR_MESSAGING_SENDER_ID",
  appId: "YOUR_APP_ID"
};
```

### 3. Run the Application

You can:

#### Option 1: Open Directly

Open:

```txt
index.html
```

directly in your browser.

#### Option 2: Run with Local Server (Recommended)

Use a local development server such as:

* VS Code Live Server
* Localhost server extensions

---

## 📝 Developer Notes

* The application's **Data Layer** is fully abstracted into a dedicated `FirebaseDB` object for clean, maintainable, and scalable architecture.
* User-generated content is sanitized using an `escapeHtml()` utility to reduce potential XSS vulnerabilities.
* Includes a smart `getTimeAgo()` helper for converting timestamps into human-readable text such as:

```txt
Just now
2 minutes ago
1 hour ago
Yesterday
```

---

## 🎨 UI & Experience

* Elegant **Glassmorphism** effects
* Smooth UI animations and transitions
* Responsive across desktop, tablet, and mobile
* Full **Light/Dark Mode** support

---

## 👨‍💻 Developer

### Ahmed Taher (Taher Dev)

**Role:** Full-Stack Developer & Technical Consultant

**Portfolio:**
https://ahmedth.netlify.app

---

## 🌟 Support & Contributions

If this project inspires or helps others build meaningful Islamic and community-focused platforms, consider giving the repository a **Star ⭐** to support future improvements.

Contributions, ideas, and feature suggestions are always welcome.

---

> **Note:** Lammet Ramadan is designed to blend the spiritual atmosphere of Ramadan with modern social networking technologies to create a meaningful, inspiring, and high-performance experience.
