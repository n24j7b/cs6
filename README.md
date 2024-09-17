java c
Homework 1: Learning Theory and Linear Predictors 
CS 6316 Machine Learning 
Due on September 25, 2024
Submission Instruction 
•  For the writing part: please only submit pdf file with name  [ComputingID]-hw1.pdf.  We recom- mend to use LaTeX and you can find a template on the course webpage.  If you are not familiar with LaTeX, using hand writing and scanning it to pdf will also work.
•  For the coding part: by default, we will use Python. Your submission should be ajupyter notebook file with the name [ComputingID]-hw1.ipynb. You can also format your writing part in the jupyter notebook along with the coding part.  If you choose to combine them into one jupyter notebook file, please submit both the original ’.ipynb’ file and an exported ’.pdf’ file. 
Questions (20 points) 
1. The Bayes Predictor (4 points) For a binary classification problem, if we know the data distri- bution D over X × Y with Y = {+1, −1}, we can define the Bayes predictor as
Note that e[y = +1 | x] + e[y = −1 | x] = 1.  Please show that this is the optimal predictor.  In other words, for any predictor h, we haveLD (fD ) ≤ LD (h)                                                              (2)
2. Selection of Hypothesis Spaces (8 points) In  lectures, we talked about how to identify the decision boundary using a mixture of Gaussian distributions.  As an exercise, please replace the distribution with the following mixture of Gaussian distributions
Please answer the following questions with the new data distribution
(a)  (2 point) What is the decision boundary of the Bayes predictor  bBayes?  Such as the Bayes predictor can be defined as

(b)  (1 point) What is the true error of the Bayes predictor, LD (fD )?
(c)  (2 point) With the following hypothesis space H and the data distribution in equation 3, please find out the best hypothesis代 写CS 6316 Machine Learning Homework 1: Learning Theory and Linear PredictorsPython
代做程序编程语言 h*  ∈ H and report the corresponding decision boundary b*H = {400/i : i ∈ [1200]}                                (5) 
(d)  (1 point) What is the true error of h* , LD (h* )?
(e)  (1 point) Sample 100 data points from  each  component and label them correspondly.  Then, with the same hypothesis space H in equation 5 and these 200 training examples, please find out the best hypothesis hS  that minimize the empirical error and report the corresponding decision boundary bS .
(f)  (1 point) What is the true error of hS , LD (hS )?
3. Perceptron algorithm (3 points) Implementing the Perceptron algorithm with a simple example. The data you need for the implementation is in the file data.txt, which is released together with the assignment.  Comparing to the pseudocode in our lecture, T was removed from line 3.  That is because in practice we do not know the actual value of T.  But we can monitor the predictions on all data points and stop the algorithm when the classifier makes correct predictions on all examples.
1: Input: S = {(x1 , y1 ), . . . , (xm ,ym ))}
2:  Initialize w (0)  = (0, . . . , 0)
3: for t = 1, 2, ··· do 
4:       i ← t  mod m 
5: if yi (w(t) , xi〉≤0 then 
6: w (t+1) ← w (t) + yi xi
7: end if 
8: end for 
9: Output: the final w(t)
4. Logistic Regression (2 points) Given a training set S = {(x1 , y1 ), . . . , (xm ,ym )}, the loss function of logistic regression is defined as
Please show that the gradient of L(hw , S) with respect to w is5. Linear Regression (3 points) The loss function of linear regression with ℓ2  regularization is defined as
Please show that the solution of this problem, when A + λI is invertible, isw = (A + λI)−1b (9)
where I is the identify matrix, A and b is defined as
Note that {xi } are column vectors.





         
加QQ：99515681  WX：codinghelp
