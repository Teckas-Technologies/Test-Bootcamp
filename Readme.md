# Day 1: Environment Setup and "Hello, World!"

Welcome to Day 1 of the Job-Ready Devs 30-Day Challenge! Today, we’ll set up our development environment and create a simple "Hello, World!" webpage to kick things off. This setup will help you get comfortable with the tools we'll be using throughout the challenge.

## Objectives
1. Set up essential development tools: GitHub, Visual Studio Code, Git, and Node.js.
2. Create a basic "Hello, World!" project using HTML and JavaScript.
3. Push your project to GitHub.

## Steps

### Step 1: Install the Necessary Tools
1. **Git**: [Download and install Git](https://git-scm.com/downloads).
2. **Node.js**: [Download and install Node.js](https://nodejs.org/).
3. **Visual Studio Code**: [Download and install VS Code](https://code.visualstudio.com/).

### Step 2: Set Up Your GitHub Repository
1. Create a GitHub account if you don’t have one: [Sign up for GitHub](https://github.com/).
2. Create a new repository named `student-management-app`.
3. Clone the repository to your local machine using:
   ```bash
   git clone https://github.com/your-username/student-management-app.git

### Step 3: Create the "Hello, World!" Project

1. **Open Visual Studio Code**: Open the `student-management-app` folder in Visual Studio Code.
   
2. **Create an HTML file**:
   - Inside the `student-management-app` folder, create a new file named `index.html`.
   - Add the following starter code to create a simple HTML structure and a "Hello, World!" message:

     ```html
     <!DOCTYPE html>
     <html lang="en">
     <head>
         <meta charset="UTF-8">
         <meta name="viewport" content="width=device-width, initial-scale=1.0">
         <title>Student Management App - Day 1</title>
     </head>
     <body>
         <h1>Hello, World!</h1>
         <p>Welcome to the Student Management App Project!</p>
     </body>
     </html>
     ```

3. **Create a JavaScript file**:
   - In the same folder, create another file named `main.js`.
   - Add a simple console log message to test your JavaScript setup:

     ```javascript
     console.log("Hello, World! Welcome to the Student Management App.");
     ```

4. **Link JavaScript to HTML**:
   - To connect your `main.js` file to the HTML, add a `<script>` tag at the bottom of the `<body>` section in `index.html`:

     ```html
     <script src="main.js"></script>
     ```

5. **Open in Browser**:
   - Open `index.html` in a web browser. You should see "Hello, World!" displayed on the page, and if you open the browser's developer console (usually accessible by pressing `F12` or `Ctrl+Shift+I`), you should see the JavaScript message: `"Hello, World! Welcome to the Student Management App."`

### Step 4: Link JavaScript to HTML

1. Open the `index.html` file in your project folder.
2. Add the following `<script>` tag at the bottom of the `<body>` section to link your `main.js` file:

   ```html
   <script src="main.js"></script>
   ```
3. Save the file.
4. Test the connection by opening `index.html` in a web browser:
    - Right-click the file and select "Open with Browser" (or drag and drop it into your browser).
    - Open the browser's developer console (press `F12` or `Ctrl+Shift+I`) to verify that the message from `main.js` appears: - - "Hello, World! Welcome to the Student Management App."

### Step 5: Push the Project to GitHub

1. Open a terminal in your project folder or use the terminal in Visual Studio Code.

2. **Stage the files**:
   - Run the following command to stage all your project files:
     ```bash
     git add .
     ```

3. **Commit the changes**:
   - Save your progress with a descriptive commit message:
     ```bash
     git commit -m "Add Day 1 Hello, World! project"
     ```

4. **Push the changes to GitHub**:
   - Upload your code to your GitHub repository:
     ```bash
     git push origin main
     ```

5. **Verify the upload**:
   - Open your GitHub repository in a browser and confirm that your `index.html` and `main.js` files have been uploaded.

Congratulations! 🎉 Your first project is now live on GitHub, and you're all set for Day 2!
