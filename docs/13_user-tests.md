# User Tests
The user test dashboard is available for administrators in the administration menu.

## New User Test
Click "New User Test" to open the form. Each user test has a unique identifier which is used in the code to change the user interface or system behavior. Available tests can be chosen from a list of active user tests. You have to give the test a title and description, and set the start and end date. For a representative sample it is advised to let the test run for one or more full weeks.

### Metrics
Then the metric(s) can be chosen. They can either be evaluated directly after the user finished the test or with a custom delay. Here again, a representative sample requires a multiple of full weeks, if applicable.

The metrics currently implemented are:

#### Pinboard Posting Activity

The pinboard posting activity counts how often a user asks, answers and comments questions and discussions in the pinboard of a course.

#### Pinboard Watch Count

The pinboard watch count denotes the number of viewed questions and discussions of a user.

#### Pinboard Activity

This pinboard activity combines pinboard posting activity and pinboard watch count. Considering the different amounts of effort, a weighting is
applied. The posting activity contributes with a ratio of 90%, while the watch count is weighted with 10%.

#### Question Response Time

The question response time denotes how long after a question was asked, a user answered the question. To compute this metric all Experience API statements with the verb ANSWERED_QUESTION are retrieved for a user,
the matching ASKED_QUESTION statement is queried and the
average difference between their timestamps is computed. Since not all users answer questions in the specified time frame, nil values may be retrieved.

#### Visit Count

The visit count denotes how many items a user visited, including videos, selftests and text parts.

#### Video Visit Count

The video visit count denotes the number of visited videos per user.

#### Course Activity

The course activity summarizes the aforementioned metrics to measure the overall activity of a user in a course. The pinboard activity is weighted with 50%, while the visit count is included without weight.

#### Course Points

After the end of a course the number of points are persisted and the quantile of the users’ points is calculated. For each enrollment a *completed* event is emitted. The course points metric returns the number of points a user received in a specified course.

### Filters

You can set filters to only accept certain users. The have the form `field operator value`. Admins and teachers are always excluded.

Fields can be every profile field and queried data, currently only enrollments denoting the number of enrollments of a user.

Operators can be `==, !=, in` for string fields and `<, >, <=, >=, <<, <=<=` for integer fields.
in checks for inclusion of the field value of the user in the supplied values, `<<` means between excluding the border values and `<=<=` including them.

Values can be either a single word like `female`, and integer, a range like `3,5` or a list of values like `1,2,3`.

#### Examples
```
enrollments == 1
gender == female
enrollments << 3,5
highest_degree in bachelor,master,phd
```

## Dashboard
When a user test is running you can see the number of participants in the test groups, the number of participants who finished the test, those who are waiting for metric evaluation in case of a delayed metric, the mean in the groups, the estimated effect (Cohen's d or Cohen's h) and the required number of participants for that effect to reach a power of 0.8.

After the test is finished and the metric retrieval is completed, the significance test results are shown.
