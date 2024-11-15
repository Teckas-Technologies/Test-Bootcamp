# Day 3: CSS Basics + Styling the Interface

Welcome to Day 3 of the Job-Ready Devs 30-Day Challenge! Today, we’ll enhance the visual appeal of our Student Management App by adding styles using CSS. You’ll focus on layout, colors, and fonts, with special attention to styling the form and student list sections.

## Objectives
1. Learn the basics of CSS for styling web pages.
2. Style the navigation bar for a modern look.
3. Apply clean and consistent styles to the student list and form sections.
4. Use CSS to improve the overall layout and typography of the app.

---

## Steps

### Step 1: Create a CSS File
1. In your project folder, create a new file named `styles.css`.
2. Link the CSS file to your HTML file by adding the following line inside the `<head>` section of `index.html`:
   ```html
   <link rel="stylesheet" href="styles.css">
   ```

---

### Step 2: Style the Navigation Bar

1. Open the `styles.css` file you created in Step 1.

2. Add the following CSS code to style the navigation bar:
   ```css
   nav {
       background-color: #007BFF; /* Set a blue background color */
       color: white; /* Set the text color to white */
       padding: 1rem; /* Add padding inside the navigation bar */
       display: flex; /* Use flexbox for layout */
       justify-content: space-between; /* Space out items */
       align-items: center; /* Align items vertically */
   }

   nav h1 {
       margin: 0; /* Remove default margin for the title */
   }

   nav ul {
       list-style: none; /* Remove default bullet points */
       padding: 0; /* Remove default padding */
       display: flex; /* Arrange list items in a row */
       gap: 1rem; /* Add space between list items */
   }

   nav ul li a {
       color: white; /* Set link text color to white */
       text-decoration: none; /* Remove underline from links */
       font-weight: bold; /* Make the text bold */
   }

   nav ul li a:hover {
       text-decoration: underline; /* Add underline when hovering over links */
   }
   ```

3. Save the file.

4. Refresh your browser to see the updated navigation bar:
    - The background is now blue, with white text.
    - The navigation links are bold and underline on hover.
    - Items in the navigation bar are aligned and spaced neatly.

---

### Step 3: Style the Student List Section

1. Open the `styles.css` file.

2. Add the following CSS code to style the student list section:
   ```css
   #student-list {
       margin: 2rem 0; /* Add space above and below the section */
       padding: 1rem; /* Add padding inside the section */
       background-color: #f9f9f9; /* Set a light gray background color */
       border: 1px solid #ddd; /* Add a light border around the section */
       border-radius: 5px; /* Round the corners of the section */
   }

   #student-list h2 {
       margin-bottom: 1rem; /* Add space below the heading */
   }

   #student-list ul {
       list-style: none; /* Remove bullet points from the list */
       padding: 0; /* Remove default padding */
   }

   #student-list ul li {
       padding: 0.5rem 0; /* Add vertical padding to each list item */
       border-bottom: 1px solid #ddd; /* Add a divider between list items */
   }

   #student-list ul li:last-child {
       border-bottom: none; /* Remove the border from the last list item */
   }
   ```

3. Save the file.

4. Refresh your browser to see the updated student list section:

    - The section now has a light gray background with padding and rounded corners.
    - The student names are neatly separated by lines, with no bullet points.

---

### Step 4: Style the Add Student Form

1. Open the `styles.css` file.

2. Add the following CSS code to style the form:
   ```css
   #add-student {
       margin: 2rem 0; /* Add space above and below the section */
       padding: 1rem; /* Add padding inside the section */
       background-color: #f9f9f9; /* Set a light gray background color */
       border: 1px solid #ddd; /* Add a light border around the section */
       border-radius: 5px; /* Round the corners of the section */
   }

   #add-student h2 {
       margin-bottom: 1rem; /* Add space below the heading */
   }

   #add-student form {
       display: flex; /* Use flexbox for form layout */
       flex-direction: column; /* Stack form elements vertically */
       gap: 1rem; /* Add space between form elements */
   }

   #add-student label {
       font-weight: bold; /* Make labels bold */
   }

   #add-student input {
       padding: 0.5rem; /* Add padding inside input fields */
       border: 1px solid #ddd; /* Add a light border to input fields */
       border-radius: 5px; /* Round the corners of input fields */
   }

   #add-student button {
       padding: 0.5rem 1rem; /* Add padding to the button */
       background-color: #007BFF; /* Set a blue background color for the button */
       color: white; /* Set button text color to white */
       border: none; /* Remove the default button border */
       border-radius: 5px; /* Round the corners of the button */
       cursor: pointer; /* Change the cursor to a pointer on hover */
   }

   #add-student button:hover {
       background-color: #0056b3; /* Darken the button color on hover */
   }
   ```

3. Save the file.

4. Refresh your browser to see the updated form:

    - The form now has a light gray background with rounded corners and padding.
    - Input fields are styled for better readability.
    - The submit button stands out with a blue color that changes on hover.

---

### Step 5: Test the Layout

1. Open your `index.html` file in a web browser:
   - You can double-click the file or right-click and select "Open with Browser."
   - Alternatively, drag and drop the file into your browser window.

2. Verify the following updates:
   - **Navigation Bar**:
     - The navigation bar has a blue background with white text.
     - Links in the navigation bar are bold and underline when hovered.
   - **Student List Section**:
     - The section has a light gray background with padding and rounded corners.
     - Student names are neatly displayed in a list format with borders separating each item.
   - **Add Student Form**:
     - The form section has a light gray background with padding and rounded corners.
     - Input fields are styled for a clean and consistent look.
     - The submit button has a blue background and changes color when hovered.

3. Interact with the app:
   - Click on the navigation links to ensure they scroll to the respective sections (e.g., "Student List" and "Add Student").
   - Test the form’s fields to ensure they are functional and visually appealing.

4. Make any necessary adjustments to your `styles.css` file if something doesn’t look right.

---

## Next Steps

- Tomorrow, we’ll add interactivity to the app using JavaScript.
- Push your changes to GitHub by following the steps from Day 1:
  1. Stage the changes:
     ```bash
     git add .
     ```
  2. Commit the changes with a descriptive message:
     ```bash
     git commit -m "Style the Student Management App with CSS"
     ```
  3. Push the changes to your GitHub repository:
     ```bash
     git push origin main
     ```

---

### Amazing job! 🎉  
Your app now has a clean and professional look. Keep up the great work, and get ready for Day 4!
