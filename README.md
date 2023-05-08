Download Link: https://assignmentchef.com/product/solved-stats507-homework-1-data-types-functions-and-conditionals
<br>
<h1>1         Warm up: Defining Simple Functions</h1>

In this problem, you will get practice defining simple functions in Python.

<ol>

 <li>Define a function called say_hi, which takes no arguments and prints the string Hello, world! when called.</li>

 <li>Define a function called goat_pad, which takes a string as its only argument, and prints that string, prepended and appended with the string goat. So, goat_pad(’bird’) should produce the output goatbirdgoat</li>

</ol>

goat_pad(’_’) should produce the output

goat_goat

and so on. You may assume that the input is a string, so there is no need to perform any error checking in your function.

<ol start="3">

 <li>Define a function called print_n, which takes two arguments, a string s and an integer n (in that order), and prints the string n times, each on a separate line. You may assume that s is a string and that the integer n is non-negative.</li>

</ol>

<h1>2         Euclid’s algorithm</h1>

Euclid’s algorithm (<a href="https://en.wikipedia.org/wiki/Euclidean_algorithm">https://en.wikipedia.org/wiki/Euclidean_algorithm</a><a href="https://en.wikipedia.org/wiki/Euclidean_algorithm">)</a> is a method for finding the greatest common divisor (GCD) of two numbers. Recall that the GCD of two numbers <em>m </em>and <em>n </em>is the largest number that divides both <em>m </em>and <em>n</em>.

<ol>

 <li>The Wikipedia page above includes several pseudocode implementations of Euclid’salgorithm. Choose one of these, and use it to implement a function gcd, which takes two integers as its arguments and returns their GCD. You may assume that both inputs are integers, so there is no need to include any error checking in your function. <strong>Note: </strong>this is one of the rare occasions where you have my explicit permission to look up your answer. Unless otherwise stated (e.g., as in this problem), looking up solutions on Wikipedia or in any other non-class resource will be considered cheating!</li>

 <li>Use your function to evaluate the GCDs of the following pairs of numbers:

  <ul>

   <li>2018, 2019</li>

   <li>1200, 300</li>

   <li>5040, 60</li>

  </ul></li>

 <li>What does your function do if one or both of its arguments are negative? Does thisbehavior make sense?</li>

</ol>

<h1>3         Approximating Euler’s number</h1>

The base of the natural logarithm, <em>e</em>, is typically defined as the infinite sum

(1)

where <em>k</em>! denotes the factorial of <em>k</em>,

<em>k</em>! = <em>k </em>· (<em>k </em>− 1) · (<em>k </em>− 2) · ··· · 3 · 2 · 1<em>,</em>

where we define 0! = 1 by convention. For more on Euler’s number, see <a href="https://en.wikipedia.org/wiki/E_(mathematical_constant)">https://en. </a><a href="https://en.wikipedia.org/wiki/E_(mathematical_constant)">wikipedia.org/wiki/E_(mathematical_constant)</a><a href="https://en.wikipedia.org/wiki/E_(mathematical_constant)">.</a> In this problem, we will explore different approaches to approximating this number.

<ol>

 <li>An early characterization of Euler’s number, due to Jacob Bernoulli, was as the limit</li>

</ol>

<em>.                                                  </em>(2)

Define a function called euler_limit that takes as an argument an integer <em>n</em>, and returns a float that approximates <em>e </em>by taking <em>x </em>= <em>n </em>in Equation (2). You may assume that the input to your function will be a positive integer.

<ol start="2">

 <li>Define a function called euler_infinite_sum that takes a single non-negative integer argument <em>n</em>, and returns an approximation to <em>e </em>based on the first <em>n </em>terms of the sum in Equation (1). Your function should return a float. You may assume that the input will be a non-negative integer, so you do not need to include error checking in your function. As an example, euler_infinite_sum(4) should return the sum of the first four terms in Equation 1, so that euler_infinite_sum(4) returns 1+1+1<em>/</em>2+1<em>/</em>6 ≈ 2<em>.</em> <strong>Note: </strong>the sum in Equation 1 starts counting with <em>k </em>= 0 (i.e., it is “0-indexed”), while our function starts counting with <em>n </em>= 1 (i.e., it is “1-indexed”). euler_infinite_sum(1) should use <em>one </em>term from Equation (1), so that euler_infinite_sum(1) returns 1. Similarly, euler_infinite_sum(0) should return 0, since by convention an empty sum is equal to zero.</li>

 <li>Define a function called euler_approx that takes a single argument, a float epsilon, and uses the sum in (1) to obtain an approximation of <em>e </em>that is within epsilon of the true value of <em>e</em>. <strong>Hint: </strong>use a while-loop. <strong>Note: </strong>you can use the Python math module to get the true value of <em>e </em>(up to floating point accuracy): exp(1).</li>

 <li>Define a function called print_euler_sum_table that takes a single positive integer n as an argument and prints the successive values obtained from euler_infinite_sum(k) as k ranges from 1 to n, one per line.</li>

 <li>Which of these two approximations is better?</li>

</ol>

<h1>4         Testing Properties of an Integer</h1>

In this problem, you’ll get a bit more practice working with conditionals, and a first exposure to the kind of thinking that is required in a typical “coding interview” question. A positive integer <em>n </em>is a <em>power of </em>2 if <em>n </em>= 2<em><sup>p </sup></em>for some integer <em>p </em>≥ 0.

<ol>

 <li>Write a function is_power_of_2 that takes a positive integer as its only argument and returns a Boolean indicating whether or not the input is a power of 2. You may assume that the input is a positive integer. You <strong>may not </strong>use the built-in sqrt function in your solution. You should need only the division and modulus (%) operations. <strong>Hint: </strong>the simplest solution to this problem makes use of recursion, though recursion is not necessary.</li>

 <li>Generalize your previous solution to a function is_power that takes two positive integers as its arguments, <em>b </em>and <em>n</em>, in that order, and returns a Boolean. is_power(b,n) should return True if <em>n </em>is a power of <em>b </em>and False</li>

</ol>