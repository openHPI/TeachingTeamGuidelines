![HPI Logo](../../img/HPI_Logo.png)

# H5P 

H5P is an open source library which delivers interactive html content. It can be embedded through iframes and has also integrations in different platform like moodle. Currently it is mainly used for educational content.





## Introduction 
H5P delivers interactive content that can be embedded in various ways into the platform. It's main feature are the interactive content types. Examples are: Drag and Drop, Fill in the Blanks,  Find the Hotspot and Interactive Video. These content types can be used to either show something in an interactive way or to create a quiz. These interactive quizzes are currently an addition to the openHPI platform and make it possible to have an interactive self-check for the  participants. However this cannot be used for final exams due to the fact that the answers are in the source code of the website.
### Availability
H5P is a free open source project under the MIT license. The source code can be found in the [Github repository](https://github.com/h5p). The project is currently founded by a company called Joubel which is an open source company. H5P aims to be community driven. There a part of the development is sourced out to the community. It is unclear how long the funding is secured but it is used by some other univercities and has available plugins for different learning platforms like moodle. The website can be found under [h5p.org](https://h5p.org/).


## How to use it
**(Lti provider anlegen)**
**Add the H5P Dummy to the course (placeholder on how to do that)**. Then execute the dummy task. You should see the Course Library. This is the section where you manage the h5p content for your course. You can create new content with the button on the top. Next select the desired type on content. This is also the place where you can upload h5p content if you downloaded it. Once you selected the the content you can fill it in any way you like. For the quizzes there are two sections on the bottom where you can set specific feedback for score ranges or the behavioral setting of the quiz. This allows you to define penalties, retries and other visual behavior of the task. Once the content is created you have to save the item. Now you will see the item as it is display for the participants of the course. Additionally you can see a box at the bottom that looks similar to this one:  ![Content Setup](../img/externaltools/h5p/content_setup.png)
The last line e.g. _exercise=60074a88a0e7742300b91a6d_ is the parameter which you have to enter on the create quiz site on open.hpi. You have to set the Lti provider as well. An example looks like this:  ![Content Setup 2](../img/externaltools/h5p/content_setup_2.png)

## Content of H5P

It is possible to use H5P for a variety of use cases. As an example it can be used to display data and display interactive quizzes. The following quizzes are examples that have been used in the computeranatomie course. 

1. **Memory** You can either set the pictures to be the same or the match different pictures. In the first case the participant will have to find pairs. In the second case the participant has to find matching pictures. As long as the participant completes the memory game, full points will be rewarded. An example looks like this:  ![Memory](../img/externaltools/h5p/memory.png)
2. **Find the words** In this quiz you can define a list of words that will be hidden in a field of letters. This will be done automatically. The words will appear in any possible way and direction in the letter field. It is possible for a word to be backwards diagonal. There are no penalties so the full points will be rewarded for finding all words. An example:  ![Find the words](../img/externaltools/h5p/find_the_words.png)
3. **Drag and Drop** In this quiz the participants drop words either on marked areas over a picture or in question fields. They are not as easy to set up as the others. However it is more flexible than the other quizzes. It is possible to define which words can be dropped into which zones. Additionally the number of words per zone can be set as well. This makes the following examples possible:  ![Drag and Drop 1](../img/externaltools/h5p/drag_and_drop_1.png)  ![Drag and Drop 2](../img/externaltools/h5p/drag_and_drop_2.png)
4. **Image Sequencing** This quiz allows you to set pictures in a correcter order. In will then mix them up for the participants. This is easy to set up and use. The example from the course looks like this:  ![Image sequencing](../img/externaltools/h5p/image_sequencing.png)


## Current problems with the tool

There are three main things that you should be aware of when using the tool. 
1. The scaling and aligning of items is either automatic and not really perfect or it requires quite some work to do it right. In some cases questions are cut of automatically or answers might overlap each other. Furthermore the scaling is not perfect and the text might get very small and unreadable in standard settings on small screens. Some examples look like this:
![Problem 1](../img/externaltools/h5p/problem_1.png)  ![Problem 2](../img/externaltools/h5p/problem_2.png)
2. Creating the quizzes might either be easy or a lot of work in some cases. Some quizes like the memory are pretty easy and intuitive. Other quizzes like the drag and drop are not intuitive and have some missing translations. This makes it more like a try and error testing instead on creating a task. An example is the problem when you press on the red text. You might think that this just discard the changes or something similar. In practice it deletes the object. 
![Problem 3](../img/externaltools/h5p/problem_3.png)
A further problem is that the flexibility for the drag and drop quiz is unexpected. You can set the drop zones for each text and you have to do that in order to specify in each drop zone which text(s) should be the correct one. It is not to difficult but it takes more time to get used to compared to the other quizzes.
3. In some quizzes there are small problem with attending the quiz. In the find the words quiz it is very difficult to select a word in the top row because the mouse it not aligned with the selection on the word field. A second problem we found is that it is also difficult to place larger texts in small drop zones in the drag and drop quiz. In both cases it is not impossible to successfully complete the task but it might be very annoying for the users.


## Feedbacks from the users



----------


Details are to be discussed. 
Contact: openhpi-info@hpi.de

