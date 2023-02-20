

# Course Iteration

### Clone course
Course Administration menu > Course structure & content.
At the top of the page there is a button "Clone course" (if not, ask your platform administrator to create a clone for you).
On click, it reveals a text input that allows to enter the **new** course code.
Click on the "Clone course" button again and the course will be cloned.

You can access the cloned course right away under:  
https://yourinstance.of.theplatform/new_course_code
It might take a few seconds until all elements of the course are available.

#### Elements which are not cloned
- Enrollments
- Collab Spaces
- Peer Assessments
- Announcements
- Discussion Forum
- Certificate Templates
- Enrollments
- Permissions
- Properties: Course Status, Course Dates, Release Records
- Learning Objectives

### General
- All deadlines need to be reset (course, sections, items, ...)
- Unlock Forum (if previously locked)
- Check all course items for links to other course specific elements (discussion forum posts, surveys, collab spaces, quizzes, cheat-sheet etc.)
- Re-adjust research queries if necessary
- Re-create "pinned" forum threads if necessary
- Check if office hour videos still make sense or need to be recorded again
  - Create a new video with office hour questions if time is given
- Adjust course overview if necessary
- Check for deadlines in texts
- Check if introductory videos and course teaser are still correct (dates/deadlines)
- Communication in the name of the "original" teaching team (if team members change, design a consistent strategy how to deal with that. This strategy should include informing the original teaching team about your plans).
- Remove / hide sample solutions if previously included (also in the original course!)
- Hide the feedback section /( I Like I wish) till its time to get feedback
- Check the existence of [the rating question "How do you rate this course overall?"](../img/courseadministration/createcourseiteration/rating_question.png) within the feedback section to feature five answers with one to five stars

### Peer Assessment
- Re-create the complete peer assessment if still requested
- In case it is a team peer assessment:
  1. Rename the existing TeamBuilder LTI provider
  2. Create a new TeamBuilder LTI provider (ask your platform admin how to do that/contact the openHPI team)
  3. Edit the cloned TeamBuilder item and replace the old TeamBuilder LTI provider with the new one
  4. Delete the old TeamBuilder LTI provider or mark it as deprecated


### CodeOcean Exercises
- Adjust links in exercise texts
- If an exercise has been used in a previous course (just in case questions might pop-up in the forum):
  1. Old RFCs (Request for comments) might still appear
  2. If a participant has solved an exercise in the previous course, his/her solutions are still visible to him/her.
  3. Do not clone exercises without consulting your contact at openHPI.

### H5P Exercises
- H5P exercises always are part of the context of a course
- Each course has its own H5P library
- H5P exercises can be "borrowed" from one course to another.
- Borrowing means that the exercise is referenced in the new course but not copied.
- When a course is cloned, the cloned exercise items link to such borrowed H5P exercises.
- The H5P exercises themselves are not cloned, the new exercise items still link to the H5P exercises, which have been created in the context of the original course.
- The H5P exercise library of the clone is empty.
- For the participants the H5P exercises are fully functionable.

**But:**

- The H5P exercises cannot be edited from within the new course, only from the original.
- If H5P exercises are used from within two different courses, the (internal H5P) learning analytics data will probably be messed up.
- If H5P exercises are to be copied from one course to another, this has to be done manually by exporting them from one H5P course library and importing them to the other H5P course library.

### Cross-Platform Copying of a Course

The following actions should be tackled in addition to above list:

- Copying videos from one Vimeo account to another
  - Check Vimeo first frame / thumbnail (could be a test-frame --> wrong)
  - Subtitles?
  - Upload slides for each video
- Check url-endpoints (e.g., https://platform1.example.org vs. https://platform2.example.org)
- Check main page for similar, but self-paced courses (e.g. *A new Java-Course got cloned, but on the main page the self-paced (archived) course gets highlighted*)
- Check exercise type (graded, self-paced, bonus, ...)
- Check optional flag
- Check syntax highlighting for programming courses (in quizzes)
- Adjust roles and teaching team, moderation and course handler (e.g., new people involved)
- Check LTI provider settings (and use another consumer or style if applicable)
- Adjust start times for unlocking new content (e.g. use 6:00 UTC for student courses)

*Remember: Courses are copied manually between platforms. Hence, we recommend to check every single item!*

![HPI Logo](../img/HPI_Logo.png)
