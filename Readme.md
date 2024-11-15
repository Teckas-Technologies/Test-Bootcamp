# Day 2: HTML Basics + App Structure

Welcome to Day 2 of the Job-Ready Devs 30-Day Challenge! Today, we’ll focus on building the basic structure of our Student Management App using HTML. You’ll create a navigation bar, a section to display a student list, and a form to add new students. Let’s dive in!

## Objectives
1. Learn HTML basics for structuring a web page.
2. Create a navigation bar for the app.
3. Build sections for adding and viewing students.
4. Understand how to organize content using semantic HTML.

---

## Steps

### Step 1: Create a New HTML File
1. Open the `student-management-app` project folder in Visual Studio Code.
2. If not already present, create a file named `index.html`.

---

### Step 2: Add the Basic HTML Structure
1. Add the following code to define the standard structure for the HTML document:
   ```html
   <!DOCTYPE html>
   <html lang="en">
   <head>
       <meta charset="UTF-8">
       <meta name="viewport" content="width=device-width, initial-scale=1.0">
       <title>Student Management App</title>
   </head>
   <body>
   </body>
   </html>

---

### Step 3: Create a Navigation Bar

1. Inside the `<body>` tag of your `index.html` file, add a `<nav>` element to create a navigation bar.
2. Use the following code to structure the navigation bar:
   ```html
   <nav>
       <h1>Student Management App</h1>
       <ul>
           <li><a href="#">Home</a></li>
           <li><a href="#student-list">Student List</a></li>
           <li><a href="#add-student">Add Student</a></li>
       </ul>
   </nav>
   ```

    - The <h1> tag will display the app title.
    - The <ul> element contains a list of links:
        - Home: Links to the homepage.
        - Student List: Links to the section displaying the list of students.
        - Add Student: Links to the section with the form for adding students.

3. Save the file and preview it in your browser to see the navigation bar at the top of the page.
4. Verify that the links work by clicking on them (even though they will only scroll to placeholders for now).

---

### Step 4: Add a Student List Section

1. Below the `<nav>` element in your `index.html` file, add a `<section>` element for displaying the student list.
2. Use the following code to structure the section:
   ```html
   <section id="student-list">
       <h2>Student List</h2>
       <ul>
           <!-- Example placeholder for student names -->
           <li>John Doe</li>
           <li>Jane Smith</li>
       </ul>
   </section>
   ```
    - The <h2> tag provides a heading for the section.
    - The <ul> element creates an unordered list of student names.
    - Add placeholder student names (John Doe and Jane Smith) to populate the list temporarily.
3. Save the file and open it in your browser to verify the section displays properly below the navigation bar.

---

### Step 5: Create a Form for Adding Students

1. Below the `<section>` for the student list, add another `<section>` element for the form to collect student details.
2. Use the following code to structure the form:
   ```html
   <section id="add-student">
       <h2>Add Student</h2>
       <form>
           <label for="name">Name:</label>
           <input type="text" id="name" name="name" placeholder="Enter student name" required>
           <br>
           <label for="email">Email:</label>
           <input type="email" id="email" name="email" placeholder="Enter student email" required>
           <br>
           <button type="submit">Add Student</button>
       </form>
   </section>
   ```

    - The <h2> tag provides a heading for the section.
    - The <form> element contains:
        - A text input field for the student name, labeled "Name."
        - An email input field for the student email, labeled "Email."
        - A submit button to add the student.
    - The required attribute ensures users must fill out the fields before submitting the form.
3. Save the file and open it in your browser to verify that the form is displayed correctly below the student list section.

---

### Step 6: Review and Save

1. Open your `index.html` file and review the structure:
   - Ensure that the navigation bar, student list section, and form are all correctly placed within the `<body>` tag.
   - Check for any missing or unclosed tags.
2. Save your file by clicking **File > Save** or pressing `Ctrl+S` (or `Cmd+S` on Mac).

---

### Step 7: Test in a Browser

1. Open your `index.html` file in a web browser:
   - You can either double-click the file or right-click and select "Open with Browser."
   - Alternatively, drag and drop the file into your browser window.
2. Verify the following:
   - The navigation bar appears at the top of the page.
   - The "Student List" section with placeholder names is displayed below the navigation bar.
   - The "Add Student" form appears below the student list section.
3. Test the navigation bar links:
   - Clicking the links should scroll the page to their respective sections: "Student List" and "Add Student."

Congratulations! 🎉 You’ve successfully structured the Student Management App with HTML. Tomorrow, we’ll start styling it with CSS.

