# Project 1: Basic Personal Finance Tracker

Goal: Track basic income and expenses using localStorage, with a minimal and responsive UI.

### 1. Set Up Project Structure
- index.html
- styles.css
- script.js

Basic folder layout, linked properly.

### 2. Create the HTML Layout
Elements to include:

- Form to add a transaction:
  - Input for description
  - Input for amount (positive for income, negative for expense)
  - Submit button
  - Section to display transactions
- Section for totals:
  - Total balance
  - Total income
  - Total expenses

Responsive with Flexbox and at least one media query.

### 3. Handle Form Submission with JavaScript
Capture the form input

Create a transaction object:
```js
{
  id: 1,
  description: "Groceries",
  amount: -30.00
}
```
- Store transaction in an array
- Save the array to localStorage

### 4. Render Transactions on the Page
On page load:
  - Read from localStorage
  - Loop through transactions
  - Append them to the page

Show:
  - Description
  - Amount

Optionally, a delete button (for later)

### 5. Calculate and Display Totals
Use Array.reduce or forEach to calculate:
  - Total balance
  - Sum of positive numbers = total income
  - Sum of negative numbers = total expense
  - Display these in real-time as transactions are added.

### 6. Add Styling
- Keep it clean and readable
- Use colors to distinguish income and expense
- Make it mobile-responsive:
- Vertical stack on mobile
- Horizontal layout on wider screens

Use:
  - Flexbox/Grid for layout
  - At least one media query

### 7. Add Delete Functionality
- Each transaction has a delete button
- Clicking removes it from the array + localStorage
- Re-render the list and totals

---

## Skills Reinforced

#### DOM Manipulation
- **How it's used**: JavaScript is used to dynamically add transactions to the page, update the totals, and remove transactions when deleted.

- **Why it matters**: DOM manipulation is essential for creating interactive, data-driven web applications. It’s a core frontend development skill used in nearly every web project.

#### Form Handling and Input Validation
- **How it's used**: Users input a description and amount into a form. JavaScript captures this input, validates it (e.g., amount is a number), and processes it.

- **Why it matters**: Proper form handling ensures good user experience and prevents bad or invalid data from entering the system — crucial for real-world applications.

#### LocalStorage for Persistence
- **How it's used**: Transactions are saved in localStorage as JSON so they persist between page reloads without needing a backend or database.

- **Why it matters**: Understanding localStorage is key for building apps that work offline or don’t require immediate server-side storage. It introduces concepts of data persistence and state management.

#### Array Methods (map, reduce, filter)
- **How it's used**: Transactions are stored as an array. Methods like map display them, reduce calculates totals, and filter is used for deleting specific entries.

- **Why it matters**: These methods are foundational for working with data in JavaScript. Mastery of these allows developers to transform, analyze, and manage collections of data efficiently.

#### Responsive Layout with Media Queries and Flexbox
- **How it's used**: The layout adapts to mobile and desktop views using Flexbox for layout structure and media queries to switch styles based on screen size.

- **Why it matters**: Mobile-friendly design is a standard requirement. Responsive design ensures your apps are accessible and usable on all device sizes.

#### Clean Separation of HTML, CSS, and JS
- **How it's used**: The project uses three separate files for structure (index.html), styling (styles.css), and logic (script.js).

- **Why it matters**: Keeping concerns separated improves maintainability, readability, and scalability. It’s a professional standard in modern web development.

---

## Deliverables
- [ ] Form to add new transactions
- [ ] Dynamic transaction list
- [ ] Real-time balance, income, and expense totals
- [ ] Data saved and loaded from localStorage
- [ ] Delete functionality
- [ ] Responsive UI for desktop and mobile

---

## Folder Structure 
```bash 
/project_1/
  ├── index.html
  ├── styles.css
  └── script.js
```

---

## Testing Tips
- Refresh the page — do your transactions persist?
- Try adding income and expense and see if totals update correctly.
- Try deleting a transaction — does everything update properly?

