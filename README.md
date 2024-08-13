# Recruitment Task: Windows Service for NBP Exchange Rates

---

## **Objective**
Develop a Windows Service application that retrieves and maintains the National Bank of Poland (NBP) exchange rates using .NET 8 (or higher) and stores the data in a SQLite database.

---

## **Technical Requirements**

1. **Platform & Framework:**
   - **Operating System:** Windows
   - **Framework:** .NET 8 or higher
   - **Database:** SQLite

2. **Development Guidelines:**
   - Implement the application as a Windows Service.
   - Ensure the service starts automatically with the system.
   - Utilize asynchronous programming where appropriate to prevent blocking operations.

---

## **Functional Requirements**

1. **Initial Data Retrieval:**
   - Upon the first startup, the service should download all NBP exchange rates from the past **two years**.
   - The retrieved data should be stored efficiently in the SQLite database.

2. **Scheduled Synchronization:**
   - **Daily Update:** Every day at **1:00 PM**, the service should fetch and update the database with the latest exchange rates from NBP.

3. **(Optional for Extra Points) RESTful API:**
   - Develop a RESTful API endpoint that:
     - Accepts a currency code (e.g., "USD", "EUR") as a parameter.
     - Returns the **most recent exchange rate** for the specified currency in a JSON format.
   - Ensure the API is secure and handles exceptions gracefully.

---

## **Assessment Criteria**

1. **Code Quality & Best Practices:**
   - Clear and maintainable code structure.
   - Proper error handling and logging mechanisms.
   - Adherence to SOLID principles.

2. **Design Patterns:**
   - Effective use of design patterns where applicable.

3. **Reliability & Robustness:**
   - The service should handle unexpected scenarios gracefully.
   - Ensure data integrity during synchronization processes.

4. **Documentation:**
   - Provide clear instructions on how to build, deploy, and run the service.
   - Include comments and documentation within the code where necessary.

---

## **Submission Guidelines**

- **Source Code:** Submit all source code files to repo, ensuring they are well-organized.
- **Documentation:** Include a README file with:
  - Instructions for installation and setup.
  - Description of the application's architecture and design decisions.
  - Any assumptions made during development.
- **Database:** Include any necessary scripts or instructions for setting up the SQLite database.
- **Optional Features:** Clearly indicate if the optional RESTful API has been implemented.

---

We look forward to evaluating your solution. Good luck!
