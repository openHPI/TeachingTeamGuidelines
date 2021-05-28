![HPI Logo](../../img/HPI_Logo.png)

# Quiz Import from Google Spreadsheets

You can import the quiz structure from Google Spreadsheets.
All you have to do is the following:

### 1. Make a copy of this template
We can provide you with a quiz template that you can copy
:::image type="content" source="../../img/courseadministration/quizmanagement/quiz_template.png" alt-text="How our quiz template looks like":::
Find the non-to-be-edited quiz structure template [here](https://docs.google.com/spreadsheets/d/1_b8wO9_HlrrHQxagYan1iM6BBK0XtnD6vESxmhnML5s/edit#gid=0)

Remember: *Please, do not edit directly the template, but make a copy of it* - see below how to do it.

:::image type="content" source="../../img/courseadministration/quizmanagement/copy_quiz_template.png" alt-text="How to make a copy of a Google spreadsheet template":::

Now that you have created a copy, you can edit yours with the quiz questions for all the weeks and homeworks in your course.
Please note that every row after the _Quizname_ rows is a question.

#### Cheat sheet of quiz questions and answers

##### The infos about the quiz and its type:

- *Name* : the name of the quiz
- *CourseSection*: the section of the course where the quiz is
- *Quiz Type*: choose the most appropriate type for the quiz
- *Instructions*: This is a standard instructions

##### Question type, its points and explanation (green cells)

- *Question*: actual text of the question
- *QuestionType*: choose between multiple answer or multiple choice
- *Points*: points of the question
- *Explanation*: eventual explanation of the question

##### The answers to the question (blue and violet cells)

- *Answer1*, *Answer2*,* Answer3*, *Answer4* : the text of the answer
- *Correctness* :choose 'True' for correct answer or  ('False') for the wrong answer
- *Explanation*: text of the eventual explanation of the answer


### 2. Share your quiz spreadsheet to our quiz service

Once you have finished filling out the quiz, question and answer infos for each week and homework worksheet, click on *Share* and paste address:
_hpi-openhpi@quizquestions-1191.iam.gserviceaccount.com_

Click *Done* to submit.


### 3. Import your quiz spreadsheet into your course

Now, go to the course section page, click on import.
Fill out the Spreadsheet name with the name of your quiz spreadsheet
Fill out the Worksheet name with the name of the worksheet you want to import (e.g. "Week1")
Click on "Submit".
It may take a little while before the values from your quiz spreadsheet get displayed.


### Troubleshooting
If the import returns the error "Pop from empty list", it is most likely that the worksheet you were trying to import from your spreadsheet was not the correct one or contained empty values.
You will have to check manually again on your spreadsheet for empty or wrong values.
Once you have manually corrected the issues, please redo step 2 and 3.
