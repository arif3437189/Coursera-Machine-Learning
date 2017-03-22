# Week 02

# Linear Regression with Multiple Variables

## Question 1

Suppose m=4 students have taken some class, and the class had a midterm exam and a final exam. You have collected a dataset of their scores on the two exams, which is as follows:

| midterm exam | (midterm exam)^2 | final exam |
|--------------|------------------|------------|
| 89 | 7921 | 96 |
|72|5184|74|
|94|8836|87|
|69|4761|78|

You'd like to use polynomial regression to predict a student's final exam score from their midterm exam score. Concretely, suppose you want to fit a model of the form h?(x)=?0+?1x1+?2x2, where x<sub>1</sub> is the midterm score and x<sub>2</sub> is (midterm score)2. Further, you plan to use both feature scaling (dividing by the "max-min", or range, of a feature) and mean normalization. 
What is the normalized feature x<sub>2</sub><sup>(4)</sup>? (Hint: midterm = 69, final = 78 is training example 4.) Please round off your answer to two decimal places and enter in the text box below.

### Answer

The mean of x<sub>2</sub> is 6675.5 and the range is 8836 - 4761 = 4075 

So x<sub>2</sub><sup>(4)</sup> is 4761 - 6675.5/4075 = -0.47.

## Question 2

You run gradient descent for 15 iterations with a=0.3 and compute J(?) after each iteration. You find that the value of J(?) decreases slowly and is still decreasing after 15 iterations. Based on this, which of the following conclusions seems most plausible?

### Answer

* Rather than use the current value of a, it'd be more promising to try a smaller value of a (say a=0.1).
* a=0.3 is an effective choice of learning rate.
* **Rather than use the current value of a, it'd be more promising to try a larger value of a (say a=1.0).**