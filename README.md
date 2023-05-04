Download Link: https://assignmentchef.com/product/solved-cs436-assignment-naive-bayes-for-text-classification
<br>
<h2>1 Naive Bayes for Text Classification</h2>

In this question, you will implement and evaluate Naive Bayes for text classification.

<strong>0 Points </strong>Download the spam/ham (ham is not spam) dataset available on myCourses. The data set is divided into two sets: training set and test set. The dataset was used in the Metsis et al. paper [1]. Each set has two directories: spam and ham. All files in the spam folders are spam messages and all files in the ham folder are legitimate (non spam) messages.

<strong>40 points </strong>Implement the multinomial Naive Bayes algorithm for text classification described here: <a href="http://nlp.stanford.edu/IR-book/pdf/13bayes.pdf">http://nlp.stanford.edu/IR-book/pdf/13bayes.pdf </a>(see Figure 13.2). Note that the algorithm uses add-one laplace smoothing. Ignore punctuation and special characters and normalize words by converting them to lower case, converting plural words to singular (i.e., “Here” and “here” are the same word, “pens” and “pen” are the same word). Normalize words by stemming them using an online stemmer such as <a href="http://www.nltk.org/howto/stem.html">http://www.nltk.org/howto/stem.html</a><a href="http://www.nltk.org/howto/stem.html">.</a> Make sure that you do all the calculations in log-scale to avoid underflow. Use your algorithm to learn from the training set and report accuracy on the test set.

<strong>10 points </strong>Improve your Naive Bayes by throwing away (i.e., filtering out) stop words such as “the” “of” and “for” from all the documents. A list of stop words can be found here: <a href="http://www.ranks.nl/stopwords">http://www.ranks.nl/stopwords</a><a href="http://www.ranks.nl/stopwords">.</a> Report accuracy for Naive Bayes for this filtered set. Does the accuracy improve? Explain why the accuracy improves or why it does not?

<h2>            2       Point Estimation</h2>

<strong>20 points </strong>Derive maximum likelihood estimators for

<ol>

 <li>parameter p, Bernoulli(p) sample of size n.</li>

 <li>parameter p based on a Binomial(N, p) sample of size n. Computeyour estimators if the observed sample is (3, 6, 2, 0, 0, 3) and N =</li>

</ol>

10.

<ol start="3">

 <li>parameters a and b based on a Uniform (a, b) sample of size n.</li>

 <li>parameter <em>µ </em>based on a Normal(<em>µ</em>, <em>σ</em><sup>2</sup>) sample of size n with known variance <em>σ</em><sup>2 </sup>and unknown mean <em>µ</em>.</li>

 <li>parameter <em>σ </em>based on a Normal(<em>µ</em>, <em>σ</em><sup>2</sup>) sample of size n with known mean <em>µ </em>and unknown variance <em>σ</em><sup>2</sup>.</li>

 <li>parameters (<em>µ</em>, <em>σ</em><sup>2</sup>) based on a Normal(<em>µ</em>, <em>σ</em><sup>2</sup>) sample of size n with unknown mean <em>µ </em>and variance <em>σ</em><sup>2</sup>.</li>

</ol>

<strong>30 points </strong>You are given a coin and a thumbtack and you perform the following experiment: toss both the thumbtack and the coin 100 times. To your surprise, you get 60 heads and 40 tails for both the coin and the thumbtack. You put Beta priors Beta(1000, 1000), Beta(100, 100), and Beta(1,1) on the coin and thumbtack, respectively.

<ol>

 <li>Derive the MLE and MAP estimates for the coin and the thumbtack.</li>

 <li>With the help of figures identify how the different priors affect theestimated parameter values. Follow the point estimation example in the lectures and illustrate in a similar manner in your answer. For full credit, a curve for each scenario should be shown along with an explanation of the curve in terms of the different values in the question (number of heads and tails recorded and parameters of the Beta prior).</li>

 <li>True or False: The MLE estimate of both the coin and the thumbtackis the same but the MAP estimate is not. Briefly explain your answer. [Answers without explanation will receive no credit.]</li>

 <li>True or False: The MAP estimate of the parameter <em>θ </em>(probability of landing heads) for the coin is greater than the MAP estimate of <em>θ </em>for the thumbtack. Briefly explain your answer. [Answers without explanation will receive no credit.]</li>

</ol>