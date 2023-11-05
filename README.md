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

### index.html
+ Links to css/style.css for the main stylesheet
  ```
  <link rel="stylesheet" href="css/style.css">
  ```
+ Links to https://kit.fontawesome.com/4a4f4b55b0.js font
  ```
  <script src="https://kit.fontawesome.com/4a4f4b55b0.js" crossorigin="anonymous"></script>
  ```
+ Links to js/questions.js to retrieve user-defined questions for the quiz
  ```
  <script src="js/questions.js" defer></script>
  ```
+ Links to js/quizApp.js for the quiz to function
  ```
  <script src="js/quizApp.js" defer></script>
  ```

+ Start Quiz button
```
<div class="start_btn"><button>Start Quiz</button></div>
```

+ Info Box div which appears when the user presses the Start Quiz button
```
    <div class="info_box">
        <div class="info-title"><span>Some Rules of this Quiz</span></div>
        <div class="info-list">
            <div class="info">1. You will have only <span>15 seconds</span> per each question.</div>
            <div class="info">2. Once you select your answer, it can't be undone.</div>
            <div class="info">3. You can't select any option once time goes off.</div>
            <div class="info">4. You can't exit from the Quiz while you're playing.</div>
            <div class="info">5. You'll get points on the basis of your correct answers.</div>
        </div>
        <div class="buttons">
            <button class="quit">Exit Quiz</button>
            <button class="restart">Continue</button>
        </div>
    </div>
```

+ Quiz Box div that pulls data from JS scripts
```
    <div class="quiz_box">
        <header>
            <div class="title">Demo Quiz App in JavaScript</div>
            <div class="timer">
                <div class="time_left_txt">Time Left</div>
                <div class="timer_sec">15</div>
            </div>
            <div class="time_line"></div>
        </header>
        <section>
            <div class="que_text">
                <!-- Insert questions from ./js/questions.js -->
            </div>
            <div class="option_list">
                <!-- Insert options to questions from ./js/questions.js -->
            </div>
        </section>

        <!-- footer of Quiz Box -->
        <footer>
            <div class="total_que">
                <!-- insert Question Count Number dynamically from JavaScript App logic -->
            </div>
            <button class="next_btn">Next Que</button>
        </footer>
    </div>
```

+ Result Box div that pulls data from JS scripts
```
    <div class="result_box">
        <div class="icon">
            <i class="fas fa-crown"></i>
        </div>
        <div class="complete_text">You've completed the Quiz!</div>
        <div class="score_text">
            <!-- insert dynamic user score as Result from JavaScript -->
        </div>
        <div class="buttons">
            <button class="restart">Replay Quiz</button>
            <button class="quit">Quit Quiz</button>
        </div>
    </div>
```

### styles.css

### questions.js

### quizApp.js

---
Note: Codebase provided from https://github.com/martysen/DemoQuizApp for use in TakeHome Assignment #5
