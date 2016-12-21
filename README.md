# Quiz

This project contains a python module for quiz handling. A quiz can be

1. Simple quiz (the more answers is correct, the more points)
2. Speed quiz (only the first correct answer gets the points)
3. Limit quiz (everybody gets the same amount of points if they have at least some percentage of the test, e. g. 70%)

A quiz is compounded from a serie of questions. There are several kinds of questions

1. Text question (example: "How many fingers has homo sapiens")
2. Dynamic text question (example: "What is a result of 2 * 3?", the formula is dynamically generated when the question is created)
3. Image question (example: "What is on the picture?")
4. Sound question (example: "Which instrument does this sound?")
5. Input sound question (example: "Can you play the Tenor C?")

At the same time the question can be one of the types

1. ABCD - single answer is correct
2. ABCD - multiple answers are correct
3. ABCD - multiple answers are correct and they must be answered
4. Open question (with a text field)

Other specification

- The design of the module must follow that the addition of a new question kind must be as simple as possible, ideally only the question class must be implemented.
- Every question must be capable of serializing and deserializing itself so it can be saved and loaded somewhere.

## CLI Application

To demonstrate the functionality there is a CLI application with a simple quiz interacting in the user's console.

## Web Application

Finally the web application containing user accounts is developed. This allows users to use the module almost anywhere via the browser. The application must

1. Display quizes (with questions)
2. Evaluate the quizes
3. Create quizes (as a serie of questions)
4. Create new question
5. Display the leaderboard
