# Demo Quiz App User Manual
## Joseph Caradonna - CSI 3150 - Take Home Assignment 5
---

Visit https://oujoe.github.io/josephcaradonna_hw5TH_csi3150_fs2023/index.html to see an example of the Quiz App

### Problem Statement
The app consists of a 5 question quiz that contains questions relating to HTML, CSS, PHP, SQL, and XML. The app operates as a website and uses HTML, CSS, and JavaScript to function. The app is designed so users can implement additional questions using JavaScript in their own implementations of the app.

### Functional Features
+ Home (index.html) page that presents with "Start Quiz" option
+ Rules menu - lists rules of the quiz before the user starts
+ Exit Quiz option - takes user back to home page
+ Continue option - starts quiz for user
+ Quiz question menu - displays a question and multiple choice options along with a 15-second timer
+ Completion menu - displays after the user answers all questions and gives a score for how many questions the user got right
+ Replay quiz option - restarts the quiz at the first question
+ Quit quiz option - takes user back to home page

### Directory Structure
To host the app on a website (like GitHub Pages) please use the directory structure outlined below:
1. The root directory needs to be a folder that contains the other files. In this example the repository "josephcaradonna_hw5TH_csi3150_fs2023
" is the default folder.
    1. CSS folder - contains all CSS files
        - style.css file - contains CSS styling for the website
    3. JS folder - contains all JS files
        - questions.js file - contains a modifiable list of questions that get referenced in the quizApp.js file
        - quizApp.js file - contains JavaScript code that controls the quiz app
    5. index.html file - must be in the root directory to be referenced by GitHub pages

### Codebase Explanation

#### index.html
<pre lang="html">
    
    <link rel="stylesheet" href="css/style.css">
    <!-- This is my personal font awesome kit code. you will have to add your own after you register with email-->
    <script src="https://kit.fontawesome.com/4a4f4b55b0.js" crossorigin="anonymous"></script>

     <!-- Add questions list -->
    <script src="js/questions.js" defer></script>

    <!-- Main logic of the app -->
    <script src="js/quizApp.js" defer></script>
</pre>

#### styles.css

#### questions.js

#### quizApp.js

---
Note: Codebase provided from https://github.com/martysen/DemoQuizApp for use in TakeHome Assignment #5
