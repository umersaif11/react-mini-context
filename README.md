# 📦 React Mini Context Project

A foundational React application that demonstrates how to manage **Global State** using the **Context API**. This project was built to understand how to solve "Prop Drilling" by sharing data directly between unconnected components.

## 🚀 Concept
In a standard React app, data flows from Parent → Child via props. This becomes a problem when deep components need data from the top (Prop Drilling).

**This project solves that by:**
1. Creating a central "Data Warehouse" (Context).
2. Creating a "Provider" to wrap the application.
3. Allowing components (`Login` and `Profile`) to access data directly, bypassing their parents.

## 🛠️ Tech Stack
* **React** (Vite)
* **Context API** (State Management)
* **CSS** (Basic Styling)

## 📂 Project Structure
The core logic resides in the `context` folder:

```text
src/
├── context/
│   ├── UserContext.js          # 1. Creates the Context (The "Plan")
│   └── UserContextProvider.jsx # 2. Provides the Data (The "Tank")
├── components/
│   ├── Login.jsx               # 3. Sends data (Writes to Context)
│   └── Profile.jsx             # 4. Receives data (Reads from Context)
├── App.jsx
└── main.jsx