# Day 3: CSS Basics + Styling the Interface
Welcome to Day 3 of the **Job-Ready Devs 30-Day Challenge!** 🎨 Today, we’ll focus on improving the visual appeal of our **Student Management App**. With CSS, you’ll transform the basic structure from Day 2 into a sleek, user-friendly interface. By the end of this session, your app will look professional and modern, setting the stage for more advanced features in the coming days.

## Overview
In this lesson, you’ll:

1. **Learn CSS basics**: Explore key properties for styling web pages.
2. **Enhance the layout**: Style the navigation bar, student list, and form sections.
3. **Focus on typography and design consistency**: Apply color schemes, spacing, and borders for a polished look.
4. **Boost your confidence**: See how a few lines of CSS can make a big difference!
Remember: Good design improves user experience. While functionality is crucial, an attractive and intuitive interface will make your app stand out.

## Objectives
1. Learn and apply CSS basics: selectors, properties, and values.
2. Style the navigation bar for a modern and functional look.
3. Design the student list and form sections with clean layouts and consistent themes.
4. Practice linking CSS to HTML for seamless integration.

## CSS Style Selectors
1. **Element Selector**
    - The element selector applies styles to all elements of a specific type.

    **Example**:
    ```css
    nav {
    background-color: #007BFF; /* Applies to all <nav> elements */
    }
    ```

    - Targets all `<nav>` elements in the `html` document.
    - Commonly used for global styles.

2. **Class Selector**
    - The class selector applies styles to elements with a specific class attribute.
    **Syntax**:
    ```css
    .class-name {
    property: value;
    }
    ```

    **Example**:
    ```css
    .nav-item {
    padding: 0.5rem; /* Adds padding to elements with the class 'nav-item' */
    }
    ```

    - Use a period (`.`) followed by the class name.
    - Multiple elements can share the same class.

3. **ID Selector**
    - The ID selector applies styles to a single element with a unique ID attribute.
    **Syntax**:
    ```css
    #id-name {
    property: value;
    }
    ```

    **Example**:
    ```css
    #student-list {
    margin: 2rem 0; /* Applies to the element with ID 'student-list' */
    }
    ```

    - Use a hash (`#`) followed by the ID name.
    - IDs must be unique on a webpage.


## CSS basic attributes

1. `background-color`
    - Sets the background color of an element. 
    **Example**:
    ```css
    background-color: #007BFF; // hexadecimal values define the different colors
    ```

2. `color`
    - Defines the text color inside an element. 
    **Example**:
    ```css
    color: white;
    ```

3. `padding`
    - Adds space inside an element, between its content and its border. 
    **Example**:
    ```css
    padding: 1rem;
    ```

4. `margin`
    - Adds space outside an element, between it and adjacent elements. 
    **Example**:
    ```css
    margin: 2rem 0;
    ```

5. `border`
    - Specifies the border style, width, and color of an element. 
    **Example**:
    ```css
    border: 1px solid #ddd;
    ```

6. `border-radius`
    - Rounds the corners of an element. 
    **Example**:
    ```css
    border-radius: 5px;
    ```

7. `display`
    - Controls the layout behavior of an element (e.g., flex, block, inline). 
    **Example**:
    ```css
    display: flex;
    ```

8. `gap`
    - Adds space between child elements in a flex or grid container. 
    **Example**:
    ```css
    gap: 1rem;
    ```

9. `text-decoration`
    - Adds or removes text decoration (e.g., underline, none). 
    **Example**:
    ```css
    text-decoration: none;
    ```

10. `cursor`
    - Changes the mouse cursor style when hovering over an element. 
    **Example**:
    ```css
    cursor: pointer;
    ```

---

## Steps
### Step 1: Create a CSS File
1. Switch to the "Day-3" Branch
    - Switch to the "Day-3" branch by running the following command in the terminal
    ```bash
     git checkout Day-3
    ```
2. In your project folder, create a new file named `styles.css`.
    **Why?**: Separating CSS from HTML keeps your code organized and easier to manage.

3. Link the CSS file to your `index.html` file by adding the following inside the `<head>` section:
    ```html
    <link rel="stylesheet" href="styles.css">
    ```
    - This line tells the browser to apply the styles defined in styles.css to your HTML file.

### Step 2: Style the Navigation Bar
1. Open the `styles.css` file.

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

3. Save the file and refresh your browser to see the updated navigation bar:
    - Notice the blue background, white text, and clean spacing between items.
    - Hover over the links to see the underline effect.

### Step 3: Style the Student List Section
1. Add the following CSS code to style the student list:
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

2. Save the file and refresh your browser:
    - The section now has a light gray background with rounded corners.
    - Student names are neatly separated by lines.

### Step 4: Style the Add Student Form
1. Add the following CSS code to style the form:
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

2. Save the file and refresh your browser:
    - The form now looks clean and professional, with visually appealing input fields and buttons.

### Step 5: Test Your Layout and Style
1. Open your app in the browser and verify:
    - The navigation bar is styled and functional.
    - The student list section is neatly organized.
    - The form has a polished design.

2. Experiment:
    - Adjust colors, padding, or fonts in `styles.css` to see the effects.
    - Share screenshots of your styled app in the community chat to inspire others!

## Push Your Changes to GitHub
Follow these steps to save your progress:

  1. **Stage the changes**:
     ```bash
     git add .
     ```
  2. **Commit the changes with a descriptive message**:
     ```bash
     git commit -m "Style the Student Management App with CSS"
     ```
  3. **Push the changes to your GitHub repository**:
     ```bash
     git push origin Day-3
     ```

---

### Amazing job! 🎉  
Your app now has a clean and professional look. Keep up the great work, and get ready for Day 4!