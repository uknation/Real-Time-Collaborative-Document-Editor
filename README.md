# Real-Time Collaborative Document Editor 📝⚡

> **Developed as part of an internship at CodTech IT Solutions

This is a real-time Google Docs-style collaborative text editor built using **React**, **Socket.IO**, **Quill**, **Node.js**, and **MongoDB**. It allows multiple users to collaborate on documents simultaneously with live editing capabilities and persistent cloud storage.

---

## 🌟 Project Overview

This project was developed during a full-stack web development internship at **CodTech IT Solutions**. The objective was to build an industrial-level real-time application that demonstrates mastery of frontend-backend integration, WebSocket communication, and database interaction.

---

## 🔧 Technologies Used

### 🚀 Frontend
- React
- Quill.js (Rich text editor)
- Axios
- Socket.IO Client

### 🛠️ Backend
- Node.js
- Express.js
- Socket.IO
- Mongoose
- MongoDB

---

## 📁 Folder Structure
Real-Time-Collaborative-Document-Editor/
│
├── client/ # React frontend
│ └── ... # Components, styles, socket config
│
├── server/ # Node.js backend
│ ├── Document.js # Mongoose schema
│ └── server.js # Express + Socket.IO server
│
├── .gitignore
├── README.md

---

## 🔄 How It Works

- When a user opens a document link, the server checks if the document exists in MongoDB.
- If not, it creates a new document with a unique ID.
- Edits are synced live across all connected users via **Socket.IO**.
- Changes are automatically saved in MongoDB.

---

## 🖥️ How to Run Locally

### 📌 Prerequisites
- Node.js
- npm
- MongoDB (Local or Atlas)

### 🛠 Setup Instructions

#### 1. Clone the Repository

```bash
git clone https://github.com/uknation/Real-Time-Collaborative-Document-Editor.git
cd Real-Time-Collaborative-Document-Editor

Install Dependencies
# Backend
cd server
npm install

# Frontend
cd ../client
npm install
