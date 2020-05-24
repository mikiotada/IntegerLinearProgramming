# Integer Linear Programming in Python

Demonstrate how to convert a matching optimization problem into an integer linear programming problem and solve it using Python. The following is an example that this project is going to solve: hundreds of students will take a survery to rank their top 5 choices among 25 courses before the semester starts. Based on these lists of preferences, we will assign all students into courses and maximize student satisfaction under some constraints including

1. A student is placed into one course
2. A size of all courses is between 14 and 16
3. There are various major students within a course to include different perspectives

The goal is to maximize the number of students who are assigned to their first and second choices and minimize the number of students placed in their third, fourth, and fifth choices.

## Data Set up

There are four csv files.  
* StudentSurveyData.csv. 7 columns and the number of students rows. Each row represents a student where his/her major and five preferences are listed.
* CourseList.csv. It lists all the courses.
* MajorList.csv. It lists all the majors.
* MajorMax.csv. It defines the maximum number of the same major students in one course.

## Installing


```
$ pip3 install pulp
```

```
$ brew install glpk
```

## Results
ILP was able to assign 99% of total 361 students into their first or second choices out of 25 chourses without violating any constraints.

## Acknowledgments

* [The Sorting Hat Goes to College](https://www.tandfonline.com/doi/abs/10.4169/math.mag.87.4.243)
* [Daniel Newman](https://www.dtnewman.com/index.html)
