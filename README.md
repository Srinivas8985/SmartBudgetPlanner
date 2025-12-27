# Student Budget Planner & Limit Monitor

> **Academic Project Submission**
> *MERN Stack Application focusing on Financial Discipline & Planning*

## 1. Problem Statement
Students and young professionals often fail to manage their monthly finances effectively because most applications focus solely on *post-spending logging* (Expense Tracking). There is a lack of tools that emphasize **proactive budget planning** and **limit monitoring** before spending occurs. This leads to frequent overspending and financial stress.

## 2. Proposed Solution
**Student Budget Planner** is a MERN stack application designed to shift the focus from reactive tracking to **proactive planning**.

Unlike generic expense trackers, this application requires users to:
1.  **Plan First**: Set a total monthly budget and allocate limits to specific categories (e.g., Food: ₹3000, Transport: ₹2000).
2.  **Monitor Health**: Real-time visual indicators show the "health" of the budget (Safe, Warning, Critical) based on algorithmic checks.
3.  **Prevent Overspending**: Alerts and warnings are displayed *before* or *during* the spending logging process if a limit is about to be breached.

## 3. Key Features
*   **Algorithmic Budget Planning**: Dynamic allocation of funds across categories with validation to ensure total allocation matches the monthly goal.
*   **Real-Time Limit Monitoring**: Visual progress bars for each category that change color (Teal -> Yellow -> Red) based on consumption percentage.
*   **Budget Health Dashboard**: A reimagined dashboard that prioritizes "Remaining Balance" and "Budget Utilization" over simple transaction history.
*   **Proactive Alerts**: Dynamic warnings in the logging interface if a transaction exceeds the remaining category limit.

## 4. Tech Stack
*   **Frontend**: React.js (Vite), Tailwind CSS, Recharts, Framer Motion
*   **Backend**: Node.js, Express.js
*   **Database**: MongoDB (with Mongoose Schemas for `User`, `Budget`, `Expense`)
*   **Authentication**: JWT (JSON Web Tokens) with secure HTTP-only cookies/local storage.

## 5. Development Workflow & Git Strategy
This project follows a feature-branch workflow to ensure code integrity:
*   `main`: Stable, production-ready code.
*   `feature/budget-logic`: Implementation of the strict budget model and backend routes.
*   `feature/ui-overhaul`: Transformation of the Dashboard to Focus on Planning.

## 6. How to Run Locally

### Prerequisites
*   Node.js (v18+)
*   MongoDB (Local or Atlas URL)

### Steps
1.  **Clone the Repository**
    ```bash
    git clone https://github.com/your-username/student-budget-planner.git
    cd student-budget-planner
    ```

2.  **Backend Setup**
    ```bash
    cd backend
    npm install
    # Create .env file with:
    # PORT=5000
    # MONGO_URI=your_mongodb_connection_string
    # JWT_SECRET=your_secret_key
    npm run dev
    ```

3.  **Frontend Setup**
    ```bash
    # Open a new terminal
    cd src
    # Go back to root if needed, or run from root
    npm install
    npm run dev
    ```

4.  **Access App**
    *   Frontend: `http://localhost:5173`
    *   Backend API: `http://localhost:5000`

## 7. Academic Integrity & Uniqueness
This project differentiates itself from standard tutorials by:
*   Implementing a complex `Budget` model with `Map` based category limits.
*   Moving away from standard "CRUD" operations to "Logical" operations (e.g., calculating health, enforcing limits).
*   Prioritizing UI/UX that reinforces financial discipline (Planning Page) rather than just data entry.

---
*Developed for [University Course Code/Name] - [Semester Year]*
