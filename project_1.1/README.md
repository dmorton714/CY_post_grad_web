# Project 1.1: Enhanced Personal Finance Tracker

Expand on your Project 1 finance tracker by adding new features for data visualization, filtering, sorting, and improved usability — all while continuing to use browser `localStorage`.

This project reinforces intermediate front-end development skills and introduces working with third-party libraries like Chart.js.

---

## Project Goals

- Enhance your basic finance tracker from Project 1
- Work with **external libraries** (Chart.js)
- Practice advanced **array operations** (sorting, filtering, pagination)
- Build a more **interactive and professional UI**
- Reinforce **modular, scalable code practices**

## Features to Implement

### 1. **Add Date to Each Transaction**
- Update the form to include a date input.
- Save the date along with the transaction.
- If left blank, default to today's date.

```js
{
  id: 1,
  description: "Groceries",
  amount: -30.00,
  date: "2025-08-07"
}
```


### 2. **Display Transactions with Sorting and Pagination**
- Show transactions in a table or list.
- Allow users to:
  - Sort by amount, date, or description
  - Choose ascending/descending order
- Add pagination:
  - Display only 5–10 transactions at a time
  - Add Previous/Next buttons to move through pages


### 3. **Filter Transactions by Date Range**
- Allow users to input a **start date** and **end date**
- Filter the displayed transactions accordingly
- Update totals to reflect filtered transactions only


### 4. **Visualize Data with Chart.js**
Use the Chart.js library (via CDN) to create:

- A **pie or doughnut chart** showing income vs. expenses
- A **bar chart** showing total expense per category (if added)

Resources:
- [Chart.js Docs](https://www.chartjs.org/docs/latest/)
- Use static chart options first, then update dynamically with user data


### 5. **Responsive & Polished UI**
- Use Flexbox and/or CSS Grid
- At least one media query for responsive layout
- Add subtle animations or UI transitions (optional)
- Different colors or styles for income/expense entries


### 6. **(Optional) Simulated Login**
- Prompt user to enter a username on load
- Store and retrieve data in localStorage per user (e.g. `financeData_john`)
- Show a welcome message or allow switching users

--- 

## Technologies Used

- HTML, CSS, JavaScript 
- [Chart.js](https://www.chartjs.org/)
- Browser localStorage

## 🧠 Skills Reinforced

| Skill                              | How It's Used                                                     | Why It Matters                                                                 |
|-----------------------------------|-------------------------------------------------------------------|--------------------------------------------------------------------------------|
| **Advanced DOM manipulation**     | Rendering table data, sorting, pagination                         | Creates scalable, interactive interfaces                                       |
| **Form handling**                 | Capturing and validating date input                               | Enhances user experience and data accuracy                                    |
| **Array methods**                 | `filter`, `sort`, `slice`, `reduce` for logic                     | These methods are critical for data processing                                |
| **Chart.js integration**          | Turning transaction data into visual charts                       | Builds familiarity with 3rd-party libraries                                   |
| **Responsive layout**             | Adapts to mobile and desktop views                                | Ensures accessibility and modern UI design                                    |
| **localStorage per user (optional)** | Simulating multi-user environment                               | Prepares for real-world user-based data handling                              |

---

## Suggested Folder Structure

```
/project_1.1/
├── index.html
├── styles.css
├── script.js
└── assets/
    └── (optional: chart.min.js if not using CDN)
```

---

## Checklist

- [ ] Date added to all transactions
- [ ] Transactions display with sorting options
- [ ] Pagination (5–10 per page)
- [ ] Date filter (start/end)
- [ ] Chart.js pie/bar chart
- [ ] Responsive design (mobile + desktop)
- [ ] Simulated login (optional)
- [ ] Modular, readable code with comments
- [ ] Working localStorage persistence

---

## Testing Tips

- Try adding and deleting multiple transactions
- Check that filters and charts update accordingly
- Test page refresh — does data persist?
- Confirm layout works on mobile and desktop
