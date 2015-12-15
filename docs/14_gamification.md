![HPI Logo](img/HPI_Logo.png)

# Gamification

The platform supports some basic gamification features. Users can achieve experience points (XP) and gain badges.

## Badges 

Currently supported are the following:

- Communication: Users that are active in the forum
 - 	Gold (3), silver (8), and bronze (13) posts (questions/answers/comments) in the forum.
- Knowledge: Users that receive good feedback (votes, accepted answers) in the forum.
 - 	Gold (3), silver (8), and bronze (13) accepted answers in the forum.
- Self-test: Users that have solved all self-tests with a score better than 0

Badges are displayed on the user's dashboard and the user's private profile page.
All available badges are displayed here. 
As long as they are not greyed out, the user has not received the badge, it's just a placeholder.

Communication badges are available in three states. Gold, silver and bronze.


## Experience Points

Users receive experience points (XP) for the following actions:

### Continuity

- Voluntary self-test taken: 10 XP
- Continuous attendance: X = (Continous_Week + 2) * 10 XP
 - First week: 0 XP
 - First continous week: 20 XP
 - Second continous week: 30 XP
 - Third continous week: 40 XP

### Communication

- User answers a forum question: 1 XP
- User receives an upvote on a question: 5 XP
- User receives an upvote on an answer: 10 XP
- User’s answer is accepted by question author: 30 XP

### Speed

- User submits assignment before due date: n^2 × 5 XP (n = deadline - submission date in days - max: 6 days) 



XPs are displayed in the top navigation (when a user is logged in) and more detailed on the user's private profile page.

Further features in this area will follow.