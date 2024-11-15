# Day 8: JavaScript Event Listeners + Data Handling

Welcome to Day 8 of the Job-Ready Devs 30-Day Challenge! Today, we’ll improve the interactivity of the form by using JavaScript event listeners. You’ll enhance form functionality by adding submit and reset buttons to capture and clear user input dynamically.

## Objectives
1. Learn how to use JavaScript event listeners to handle form events.
2. Capture user input with the submit button and reset the form with the reset button.
3. Improve the interactivity of the frontend by handling form actions dynamically.

---

## Steps

### Step 1: Add a Reset Button to the Form
1. Open your `index.html` file.
2. Add a reset button to the form below the submit button:
   ```html
   <button type="reset">Reset</button>
   ```

3. Save the file and refresh your browser to see the reset button appear.

### Step 2: Enhance the Submit Button Functionality
1. Open your script.js file.
2. Modify the form event listener to display a success message when a student is added:
    ```javascript
    form.addEventListener('submit', (event) => {
    event.preventDefault(); // Prevent the default form submission behavior

    const name = nameInput.value.trim();
    const email = emailInput.value.trim();

    if (!name || !email) {
        alert('Please fill out both fields!');
        return;
    }

    // Add the new student to the list
    addStudent(name, email);

    // Display a success message
    alert('Student added successfully!');

    // Clear the input fields
    nameInput.value = '';
    emailInput.value = '';
    });
    ```

3. Save the file and test:
    - Add a student using the form and verify that the success message appears.

### Step 3: Add an Event Listener for the Reset Button
1. Add an event listener for the reset button to display a confirmation message when the form is cleared:
    ```javascript
    const resetButton = document.querySelector('button[type="reset"]');

    resetButton.addEventListener('click', () => {
        const confirmation = confirm('Are you sure you want to clear the form?');
        if (!confirmation) {
            // Prevent the reset if the user cancels
            event.preventDefault();
        }
    });
    ```

2. Save the file and test:
    - Click the reset button and confirm whether the form is cleared based on the user’s choice.


## Push Your Changes to GitHub
Follow these steps to save your progress:

  1. **Stage the changes**:
     ```bash
     git add .
     ```
  2. **Commit the changes with a descriptive message**:
     ```bash
     git commit -m "Add functions for dynamic student list rendering"
     ```
  3. **Push the changes to your GitHub repository**:
     ```bash
     git push origin Day-8
     ```

---

## Fantastic work! 🎉
You’ve successfully enhanced the interactivity of your app by handling form events dynamically. This is an essential skill for creating user-friendly applications. Keep up the great work, and get ready for the backend setup tomorrow!