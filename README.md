Download Link: https://assignmentchef.com/product/solved-cs577-homework2
<br>
<h1></h1>

<ol>

 <li>

  <ul>

   <li>Design an algorithm to compute the binary representation of 10<em><sup>n </sup></em>in <em>O</em>(<em>n</em><sup>log</sup><sup>2 3</sup>) time.</li>

   <li>Design an algorithm that converts a given <em>n</em>-digit decimal number to binary in <em>O</em>(<em>n</em><sup>log</sup><sup>2 3</sup>) time.</li>

  </ul></li>

</ol>

Hint: Use the integer multiplication algorithm from class as a blackbox.

<ol start="2">

 <li>Given an array <em>A</em>[1<em>,…,n</em>] of integers and a positive integer <em>k</em>, we want to find a rearrangement</li>

</ol>

<em>.                                      .</em>

<em>B </em>of <em>A </em>such that the subarrays <em>B</em><sub>1 </sub>= <em>B</em>[1<em>,…,k</em>]<em>,B</em><sub>2 </sub>= <em>B</em>[<em>k </em>+ 1<em>,…,</em>2<em>k</em>]<em>,…</em>, satisfy the following property: For every <em>i &lt; j</em>, every element of <em>B<sub>i </sub></em>is less than or equal to every element of <em>B<sub>j</sub></em>.

Design an <em>O</em>(<em>n</em>log(<em>n/k</em>)) algorithm for this problem. You can assume that all elements in the array are distinct.

Hint: First solve the case where <em>n </em>= 2<em>k</em>.

<h1>Regular Problems</h1>

<ol start="3">

 <li>[Graded, 3 points] In the knapsack problem, you are given a weight limit <em>W </em>and arrays <em>w</em>[1<em>,…,n</em>] and <em>v</em>[1<em>,…,n</em>] of nonnegative integers for some <em>n </em>≥ 1, where <em>w</em>[<em>i</em>] represents the weight of the <em>i</em>-th item and <em>v</em>[<em>i</em>] its value. You want to know the maximum total value that you can achieve by a subset of the items such that the total weight does not exceed <em>W</em>.</li>

</ol>

Consider the knapsack problem with the following additional restriction: if you include an item with value <em>v </em>then you need to also include every item with value greater than <em>v</em>.

For example, for <em>W </em>= 10 and (<em>w</em>[1]<em>,v</em>[1]) = (1<em>,</em>7), (<em>w</em>[2]<em>,v</em>[2]) = (4<em>,</em>11), (<em>w</em>[3]<em>,v</em>[3]) = (6<em>,</em>9), and (<em>w</em>[4]<em>,v</em>[4]) = (3<em>,</em>10), the answer is 21, which is realized by the subset of items {2<em>,</em>4}. Note that the subset {1<em>,</em>2<em>,</em>4} is not a valid solution because of the additional restriction, even though its total weight does not exceed <em>W</em>.

The simple solution to this problem is to sort the items by value and then place items in the knapsack until you can’t fit more. As we saw in class, sorting the items would take Θ(<em>n</em>log<em>n</em>) time. Your goal is to design an algorithm that solves this problem in <em>O</em>(<em>n</em>) time irrespective of the order in which the items are given. You can assume that all values in the array <em>v</em>[1<em>,…,n</em>] are distinct.

1

<ol start="4">

 <li>You are given an <em>n </em>× <em>n </em>grid, and a procedure <em>V </em>(<em>i,j</em>) that assigns an integer value to each position (<em>i,j</em>) in the grid, where <em>i </em>and <em>j </em>are integers such that 1 ≤ <em>i,j </em>≤ <em>n</em>. Your goal is to find a local minimum (or sink) in the grid (i.e., integers <em>i</em><sup>∗</sup><em>,j</em><sup>∗ </sup>with 1 ≤ <em>i</em><sup>∗</sup><em>,j</em><sup>∗ </sup>≤ <em>n </em>such that for all neighbors (<em>i,j</em>) of (<em>i</em><sup>∗</sup><em>,j</em><sup>∗</sup>) in the grid, <em>V </em>(<em>i</em><sup>∗</sup><em>,j</em><sup>∗</sup>) ≤ <em>V </em>(<em>i,j</em>)). The neighbors of (<em>i,j</em>) are (<em>i </em>− 1<em>,j</em>)<em>, </em>(<em>i </em>+ 1<em>,j</em>)<em>, </em>(<em>i,j </em>+ 1)<em>, </em>(<em>i,j </em>− 1); the elements along the diagonals do not count as neighbors.</li>

</ol>

Design an algorithm that makes <em>O</em>(<em>n</em>) calls to <em>V </em>. Note that the grid has <em>n</em><sup>2 </sup>nodes.

<ol start="5">

 <li>You are given a topographical map that provides the maximum altitude along the direct road between any two neighboring cities, and two cities <em>s </em>and <em>t</em>. Design a linear-time algorithm that finds a route from <em>s </em>to <em>t </em>that minimizes the maximum altitude. All roads can be traversed in both directions.</li>

</ol>

<h1>Challenge problem</h1>

The following is one of the nicest introductory algorithm problems I know. Give it a try!

<ol start="6">

 <li>You are given <em>n </em>coins, at least one of which is bad. All the good coins weigh the same, and all the bad coins weigh the same. The bad coins are lighter than the good coins.</li>

</ol>

Design an algorithm that makes <em>O</em>((log<em>n</em>)<sup>2</sup>) weighings on a balance to find the exact number of bad coins. Each weighing tells you whether the total weight of the coins on the left side of the balance is smaller than, equal to, or larger than the total weight of the coins on the right side.

<h1>Programming problem</h1>

<ol start="7">

 <li>SPOJ problem <a href="https://www.spoj.com/problems/AGGRCOW">Aggressive Cows</a> (problem code AGGRCOW).</li>

</ol>