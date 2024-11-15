# Day 4: JavaScript Basics + DOM Manipulation
Welcome to Day 4 of the **Job-Ready Devs 30-Day Challenge!** 🎉 Today, you’ll take your **Student Management App** to the next level by adding interactivity with **JavaScript**. You’ll learn to dynamically update the student list based on user input—just like real-world applications. By the end of this session, your app will respond to user actions and feel alive!

## Overview
In this lesson, you’ll:

1. **Learn JavaScript basics**: Understand variables, event listeners, and the `Document Object Model (DOM).`
2. **Capture user inputs**: Use form data in your app.
3. **Manipulate the DOM**: Dynamically add content to the page.
4. **Validate inputs**: Ensure clean and error-free user interactions.
Remember: Learning JavaScript opens the door to building dynamic and interactive web applications. Stay curious and experiment!

## Objectives
1. Understand basic JavaScript syntax and the importance of the DOM.
2. Write JavaScript to capture and validate form inputs.
3. Dynamically update the "Student List" with user-provided data.
4. Build error handling and validation for smoother user experience.

## Steps
### Step 1: Add a JavaScript File
1. Switch to the "Day-4" Branch
    - Switch to the "Day-4" branch by running the following command in the terminal
    ```bash
     git checkout Day-4
    ```
2. In your project folder, create a new file named script.js.
    Why?: Keeping JavaScript in a separate file helps keep your code organized and maintainable.
3. Link the JavaScript file to your index.html by adding the following line before the closing `</body>` tag:
    ```html
     <script src="script.js"></script>
    ```

### Step 2: Capture Form Inputs
1. Open the `script.js` file.
2. Select elements from the HTML to interact with using JavaScript:
    ```javascript
    const form = document.querySelector('#add-student form');
    const nameInput = document.querySelector('#name');
    const emailInput = document.querySelector('#email');
    const studentList = document.querySelector('#student-list ul');
    ```
    - `document.querySelector()` allows you to grab elements from your HTML for manipulation.

3. Add an event listener to the form to capture its "submit" event:
    ```javascript
    form.addEventListener('submit', (event) => {
    event.preventDefault(); // Prevent the page from refreshing

    // Capture input values
    const name = nameInput.value;
    const email = emailInput.value;

    // Log values to verify
    console.log(`Name: ${name}, Email: ${email}`);

    // Clear the input fields
    nameInput.value = '';
    emailInput.value = '';
    });
    ```
4. Save and test:
    - Open your browser console (`F12` or `Ctrl+Shift+I`).
    - Submit the form and check if the captured values are logged to the console.

### Step 3: Dynamically Add Inputs to the Student List
1. Update the form event listener to dynamically create a new student entry in the list:
    ```javascript
    form.addEventListener('submit', (event) => {
    event.preventDefault();

    // Capture and trim inputs
    const name = nameInput.value.trim();
    const email = emailInput.value.trim();

    // Validate inputs
    if (!name || !email) {
        alert('Both fields are required!');
        return;
    }

    // Create a new list item
    const listItem = document.createElement('li');
    listItem.textContent = `${name} - ${email}`;

    // Add the new student to the list
    studentList.appendChild(listItem);

    // Clear the input fields
    nameInput.value = '';
    emailInput.value = '';
    });
    ```

2. Save and refresh your browser:
    - Fill out the form and click "Add Student."
    - Check that the student name and email are displayed in the list below.

### Step 4: Enhance User Experience with Validation
1. Update the code to handle empty inputs gracefully:
    ```javascript
    form.addEventListener('submit', (event) => {
    event.preventDefault();

    const name = nameInput.value.trim();
    const email = emailInput.value.trim();

    // Validate inputs
    if (!name || !email) {
        alert('Please fill out both fields!');
        return;
    }

    // Add the student to the list
    const listItem = document.createElement('li');
    listItem.textContent = `${name} - ${email}`;
    studentList.appendChild(listItem);

    // Clear the inputs
    nameInput.value = '';
    emailInput.value = '';
    });
    ```
2. Save and test:
    - Submit the form without filling out the fields.
    - You should see an alert prompting the user to complete the form.
    - Properly filled forms should add the student to the list.

## Push Your Changes to GitHub
Follow these steps to save your progress:

  1. **Stage the changes**:
     ```bash
     git add .
     ```
  2. **Commit the changes with a descriptive message**:
     ```bash
     git commit -m "Add JavaScript functionality for form and student list"
     ```
  3. **Push the changes to your GitHub repository**:
     ```bash
     git push origin Day-4
     ```

---

## You Did It! 🎉
Congratulations on completing Day 4! Your **Student Management App** is now interactive, and you’ve taken a huge step toward building real-world applications. See you tomorrow for more exciting challenges as we enhance your app further! 🚀
