Download Link: https://assignmentchef.com/product/solved-coptimzation-problem-set-4
<br>



<strong>Convex Optimization</strong>




<h1>Problems from textbook</h1>

<table width="274">

 <tbody>

  <tr>

   <td width="43">Ref.</td>

   <td width="230">Exercises</td>

  </tr>

  <tr>

   <td width="43">[1]</td>

   <td width="230">9.6, 9.10, 11.1, 11.4, 11.6, 11.10</td>

  </tr>

 </tbody>

</table>

<h1>Matlab Assignment</h1>

As discussed in class, a large number of primal-dual interior point methods (IPM) are available whose practical efficiency strongly depends on the techniques used to solve their Newton equation system. In this assignment, you will implement a very simple version of interior point method for QP,

Minimize                                                                                (1)

Subject to <em>.</em>

<ul>

 <li>Derive the KKT conditions of (1) with lagrange multipliers <em>s </em>(for inequality constraint) and <em>y </em>(for equality constraint).</li>

 <li>Use logarithmic barrier to eliminate inequality constraints, and rewrite the KKT conditions for the new problem. Hint: Your answer should be in the form given below, where <em>X </em>and <em>S </em>are diagonal matrices with elements of vectors <em>x </em>and <em>s </em>spread across the diagonal, respectively and <em>e </em>∈R<em><sup>n </sup></em>is the vector of ones. You see that the only difference with part (a) is a perturbation of the complementarity slackness.</li>

 <li>Use the procedure presented in class to show that if (<em>x,y,s</em>) is primal and dual feasible then the duality gap in the barrier subproblem is equal to <em>x<sup>T</sup>s </em>= <em>nµ</em>, i.e., the term <em>µ </em>controls the distance to optimality.</li>

 <li>Primal-dual IPM applies the Newton method to solve the KKT conditions in part (b). To be more precise, it compute the Newton direction and make one step in this direction before reducing the barrier parameter <em>µ</em>. The Newton direction (∆<em>x,</em>∆<em>y,</em>∆<em>s</em>) is computed by solving the following system of linear equations:</li>

</ul>

Accordingly, the following simple primal-dual IPM for convex quadratic programming is presented. Implement the given algorithm and test your code for a number of random quadratic programs.

<ul>

 <li>The algorithm must guarantee that the error in equation <em>XSe </em>= <em>µe </em>is small. Plot k<em>XSe</em>−<em>µe</em>k versus iteration number.</li>

</ul>


