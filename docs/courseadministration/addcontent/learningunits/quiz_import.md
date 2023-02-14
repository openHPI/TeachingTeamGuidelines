#  Importing a quiz from a spreadsheet
In order to add a new quiz on the platform you also have the option to insert all the questions and answers into a Google Sheet document and then import it to the platform. This is the preferred way for many, as it saves time and provides the opportunity to adapt and reuse the same quiz template for several courses.

### 1. Get a copy of the Google Sheet template
Request your platform administrator to provide you with a copy of our quiz template spreadsheet.

To get yourself familiar with the way the template is structured, you can see an *only view* [example of the spreadsheet here](https://docs.google.com/spreadsheets/d/1oVpcdnl1vr-9hr8zuyyTtZXF7ZIb-wGVgOtSKleebJ8/edit?usp=sharing).

### 2. Fill in the quiz questions and answers

Withing the Google Sheet template you can click on any of the field titles (first row) to see an explanation about how to fill them. However, let's have an overview of the required fields:

##### The basic information about the quiz:

- *Quizname*: the name of the quiz
- *CourseSection*: the section of the course where the quiz will be uploaded. It must be a numeric value.
- *Quiz Type*: choose the most appropriate type for the quiz: self-test (ungraded), weekly assignment (graded), survey, bonus or final exam. The template provides the standard configuration for each one of the types of quizzes that you choose.
- *Instructions*: The instruction text for the students taking the quiz. Please note that self-tests do not have instructions.

##### Questions (green cells)

- *Question*: actual text of the question.
- *Question Type*: you can choose between 'MultiSelect' and 'SingleSelect' and 'FreeText'.
- *Points*: number of points for each question
- *Explanation*: optional explanation of the question
- *Exclude from recap*: recap is a platform feature that takes all questions from the self tests, shuffles the them and provides an "index card" style to recap the course content before the final exam. If e.g. a question relates to a previous question, it should be excluded from the recap.

##### Answers (blue and violet cells)

- *Answer 1*, *Answer 2*,* Answer 3*, *Answer 4* : the text of the answer
- *Correctness*: choose 'TRUE' for a correct answer or  'FALSE' for an incorrect answer
- *Explanation*: optional explanation about the answer. This is shown to learners together with the results of the quiz.

### 3. Share your quiz spreadsheet to our quiz service

_Before proceeding with this step, rename your quiz spreadsheet in a unique way, e.g._: `coursecode_quizname`

Once you have finished filling out the quiz questions and answers, click on *Share* and paste the address:
_hpi-openhpi@quizquestions-1191.iam.gserviceaccount.com_

Click *Done* to submit.


### 4. Import the quiz spreadsheet into your course

Go to the course section within 'Course Structure & Content' and click on the 'Import quizzes from spreadsheet' button. A pop up dialog window opens.

Fill out the Spreadsheet name with the **file name** of your quiz spreadsheet (not the URL).
Fill out the Worksheet name with the name of the worksheet you want to import (e.g. "Week1").
Click on *Submit*.
It may take a little while before the values from your quiz spreadsheet get displayed.
Check the status banner on the top of the page for the status of your import.


#### Troubleshooting
If the import shows an error, you will have to check manually again on your spreadsheet for empty or wrong values. Once you have manually corrected the issues, please redo steps 3 and 4.

![HPI Logo](../../../img/HPI_Logo.png)
