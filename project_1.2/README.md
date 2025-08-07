# Project 1.2: Personal Finance Tracker with Backend (Express + SQLite)

In this version, you will build on the enhanced finance tracker (Project 1.1) by creating a backend using **Node.js**, **Express**, and **SQLite**. Instead of storing data in localStorage, you'll now persist data in a real database and interact with it through a RESTful API.

This project introduces full-stack development concepts and mirrors the structure of real-world web applications.

---

## Project Goals

- Replace localStorage with a **Node.js + Express API**
- Use **SQLite** as your database for persistent data
- Create **RESTful API routes** for CRUD operations
- Maintain a clean **frontend-backend separation**
- Retain existing UI features (filtering, charts, pagination, etc.)

---

## Features to Implement

### 1. **Set Up the Backend**
- Use `Express.js` to create a local API server
- Install and configure `sqlite3`
- Create a `transactions` table with fields:
  - `id` (INTEGER PRIMARY KEY)
  - `description` (TEXT)
  - `amount` (REAL)
  - `date` (TEXT)
  - `category` (TEXT, optional)



### 2. **Build RESTful API Endpoints**

| Method | Route               | Description                      |
|--------|---------------------|----------------------------------|
| GET    | `/api/transactions` | Get all transactions             |
| POST   | `/api/transactions` | Add a new transaction            |
| DELETE | `/api/transactions/:id` | Delete a transaction by ID |
| (Optional) PUT | `/api/transactions/:id` | Edit a transaction |

- Validate input on the server
- Use middleware like `express.json()` to parse JSON



### 3. **Connect the Frontend to the Backend**
- Replace localStorage with `fetch()` or `axios` calls to your API
- On page load, fetch and render data from the backend
- On form submit, POST to your API
- On delete, send a DELETE request
- Make sure totals and charts update after each operation



### 4. **Keep Frontend Functionality from Project 1.1**
- Sorting, filtering, and pagination
- Date range filters
- Chart.js integration
- Responsive design

---

## 🔧 Technologies Used

**Backend:**
- Node.js
- Express.js
- SQLite (`sqlite3` or `better-sqlite3`)
- (Optional) CORS middleware

**Frontend:**
- HTML, CSS, JavaScript
- Chart.js
- Fetch API or Axios

---

## Skills Reinforced

| Skill                  | How It's Used                                                | Why It Matters                                         |
|------------------------|--------------------------------------------------------------|--------------------------------------------------------|
| Express.js API design  | RESTful routes for CRUD operations                           | Foundation for building full-stack web apps            |
| SQLite                 | Store and retrieve persistent data                           | Lightweight and portable real-world database           |
| Frontend ↔ API         | Fetching and updating data via HTTP requests                 | Essential for dynamic, data-driven interfaces          |
| Input validation       | Validate data both client-side and server-side               | Protects data integrity and improves UX                |
| Full-stack architecture| Clean separation between frontend and backend layers         | Mirrors real-world software structure                  |

---

## Suggested Folder Structure

```
/project_1.2/
├── /client/
│   ├── index.html
│   ├── styles.css
│   └── script.js
├── /server/
│   ├── index.js         # Express server
│   └── db.sqlite        # SQLite database
├── package.json
└── README.md
```

---

## Checklist

### Backend
- [ ] Express server running
- [ ] SQLite database initialized
- [ ] GET/POST/DELETE routes working
- [ ] Validations in place

### Frontend
- [ ] Transactions fetched from API
- [ ] Form submits data to backend
- [ ] Deletion updates UI and backend
- [ ] Charts and totals update dynamically
- [ ] UI remains responsive

---

## Testing Tips

- Does data persist after refresh?
- Can you delete a transaction and see it removed from the database?
- Do charts reflect the correct totals?
- Are server errors handled gracefully?

---

## Stretch Goals
- Categories for charting
- CSV export
- Input validation
- Error handling
- Simple tests