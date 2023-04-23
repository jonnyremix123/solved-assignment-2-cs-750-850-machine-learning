Download Link: https://assignmentchef.com/product/solved-assignment-2-cs-750-850-machine-learning
<br>
<h1>Problem 1 [30%]</h1>

This problem examines the use and assumptions of LDA and QDA. We will be using the dataset Default from ISLR.

<ol>

 <li>Split the data into a training set (70%) and a test set (30%). Then compare the classification error of LDA, QDA, and logistic regression when predicting default as a function of features of your choice. Which method appears to work best?</li>

 <li>Report the confusion table for each classification method. Make sure to label which dimension is the predicted class and which one is the true class. What do you observe?</li>

 <li>Are the LDA assumptions satisfied when predicting default as a function of balance <em>only </em>(i.e default ~ balance)? You can use qqnorm and qqline to examine whether the conditional class distributions are normally distributed. Also examine standard deviations of the class distributions. Are the QDA assumptions satisfied?</li>

 <li>Would you ever want to use LDA in place of QDA even when you suspect that some of the assumptions are violated (e.g. different conditional standard deviations) for LDA?</li>

</ol>

<em>Hint</em>: Check out <a href="https://www.tidyverse.org/">TidyVerse</a> for a collection of packages that can help with data manipulation. And see the <a href="https://www.rstudio.com/resources/cheatsheets/">Rstudio cheatsheets</a> for a convenient and concise reference to the methods. This is entirely optional!

<h1>Problem 2 [30%]</h1>

Using the <a href="http://yann.lecun.com/exdb/mnist/">MNIST</a> dataset, fit classification models in order to predict the digit <strong>1 </strong>(vs all others).

<ol>

 <li>Compare the classification error for each one of these methods:</li>

 <li>Logistic regression</li>

 <li>K-NN with 2 <em>reasonable </em>choices of k</li>

 <li>LDA</li>

 <li>Explore at least one transformation of the features (predictors), such as considering their combinations, and run the methods from part 1 on the data.</li>

 <li>Which one of the methods works the best?</li>

</ol>

Make sure to split the data into a training set and a test set. No need to run on the entire dataset; a subsample of say 10000 datapoints is OK.

<strong>Hint</strong>: There is a file in the gitlab repository: assignments/mnist_simple.Rmd which you can use as a starting point. If you are using Python, please checkout <a href="https://pypi.org/project/python-mnist/">this package.</a> If you have trouble getting started, please do not hesitate to ask the instructor or the TAs or Piazza for help.

1

<h1>Problem O2 [35%]</h1>

This problem can be substituted for Problem 2 above, for up to 5 points extra credit. The better score from problems 2 and O2 will be considered.

Solve Exercises <em>1.11 </em>and <em>1.13 </em>in [Bishop, C. M. (2006). Pattern Recognition and Machine Learning].

<h1>Problem 3 [20%]</h1>

Logistic regression uses the logistic function to predict class probabilities:

<em>e</em><em>β</em><sub>0</sub>+<em>β</em><sub>1</sub><em>X</em>

<em>p</em>(<em>X</em>) =

1 + <em>e</em><em>β</em><sub>0</sub>+<em>β</em><sub>1</sub><em>X</em>

This is equivalent to assuming a linear model for the prediction of the <em>log-odds</em>:

<sup> </sup><em>p</em>(<em>X</em>)

log               = <em>β</em><sub>0 </sub>+ <em>β</em><sub>1</sub><em>X</em>

1 <em>−p</em>(<em>X</em>)

Using algebraic manipulation, <em>prove </em>that these two expressions are identical. See Section 4.3 in ISLR and equations (4.2) &amp; (4.3) for more context.

<h1>Problem 4 [20%]</h1>

This problem examines the differences between LDA and QDA.

<ol>

 <li>For an arbitrary training set, would you expect for LDA or QDA to work better on the <em>training set</em>?</li>

 <li>If the Bayes decision boundary between the two classes is linear, would you expect LDA or QDA to work better on the <em>training set</em>? What about the <em>test set</em>?</li>

 <li>As the sample size increases, do you expect the prediction accuracy of QDA with respect to LDA increase or decrease</li>

 <li><em>True or False</em>: Even if the Bayesian decision boundary for a given problem is linear, we will probably achieve a superior test error rate using QDA rather than LDA because QDA is more flexible and can model a linear decision boundary. Justify your answer.</li>

</ol>


