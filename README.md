<!-- Output copied to clipboard! -->

<!-----
NEW: Check the "Suppress top comment" option to remove this info from the output.

Conversion time: 1.602 seconds.


Using this Markdown file:

1. Paste this output into your source file.
2. See the notes and action items below regarding this conversion run.
3. Check the rendered output (headings, lists, code blocks, tables) for proper
   formatting and use a linkchecker before you publish this page.

Conversion notes:

* Docs to Markdown version 1.0β31
* Sun Sep 26 2021 22:00:00 GMT-0700 (PDT)
* Source doc: 2.1 Boolean Values & Expressions (Java) (Make a Copy)
* This is a partial selection. Check to make sure intra-doc links work.
* Tables are currently converted to HTML tables.
----->
# 2.1 Boolean Values & Expressions

* In the 1840s, the mathematician George Boole showed that the classical rules of logic could be expressed in purely mathematical form using only the two values “true” and “false.”  
* Boole’s work could be used to optimize the design of electromechanical telephone switches.  
* led directly to the use of _Boolean logic _to design computer circuits. 


### The Bool Data Type & Boolean Expressions



* `int` and `double` have many of possible values, the Java data type `boolean` only has two possible values: `true` or `false`
* `true` and `false `are values, just like 0 and 43.7 are values for int and double
* An expression that evaluates to a boolean value `true` or `false` is a boolean expression


### Comparison Operators

The most common way to produce boolean values is through comparison operators.  Just as there are arithmetic operators (+,-,*, /, %) and string operators (+) that allow us to form numerical and string operations, boolean expressions are formed using the set of comparison operators in Java.


<table>
  <tr>
   <td><strong>Comparison Operator</strong>
   </td>
   <td><strong>Description</strong>
   </td>
  </tr>
  <tr>
   <td>&lt;
   </td>
   <td>Less than
   </td>
  </tr>
  <tr>
   <td>>
   </td>
   <td>Greater than
   </td>
  </tr>
  <tr>
   <td>&lt;=
   </td>
   <td>Less than or equal to
   </td>
  </tr>
  <tr>
   <td>>=
   </td>
   <td>Greater than or equal to
   </td>
  </tr>
  <tr>
   <td>==
   </td>
   <td>Equivalent
   </td>
  </tr>
  <tr>
   <td>!=
   </td>
   <td>Not Equivalent
   </td>
  </tr>
</table>



<table>
  <tr>
   <td>boolean expression
   </td>
   <td>Result
   </td>
  </tr>
  <tr>
   <td><code>4 > 5</code>
   </td>
   <td>
     <code>false</code>
   </td>
  </tr>
  <tr>
   <td><code>4 &lt; 5</code>
   </td>
   <td>
     <code>true</code>
     
   </td>
  </tr>
  <tr>
   <td><code>5 &lt;= 5</code>
   </td>
   <td>
     <code>true</code>
   </td>
  </tr>
  <tr>
   <td><code>12 >= 11 </code>
   </td>
   <td>
     <code>true</code>
   </td>
  </tr>
  <tr>
   <td><code>12 &lt;= 11</code>
   </td>
   <td>
     <code>false</code>
   </td>
  </tr>
  <tr>
   <td><code>10 == 10</code>
   </td>
   <td>
     <code>true</code>
   </td>
  </tr>
  <tr>
   <td><code>10 !=10 </code>
   </td>
   <td>
     <code>false</code>
   </td>
  </tr>
  <tr>
   <td><code>4 != 5</code>
   </td>
     <td><code>true</code>
   </td>
  </tr>
</table>



### true/false Values

In Java, the words **true** and **false** have special meaning and CANNOT be used as variable names. They are boolean values, and as you can see in the above examples, the result of boolean expressions.  Just as 4 and 5 are numerical values, and “hello” and “good-bye” are string values — true and false are boolean values.   It is important to note that true and false have a lowercase t and f and must be expressed in that fashion.


### Combining Comparison and Numerical Operators

We can form boolean expressions by combining numerical expressions with comparison operators:


<table>
  <tr>
   <td><strong>You Try</strong>
   </td>
   <td><strong>Result</strong>
   </td>
  </tr>
  <tr>
   <td>(6*2) >= (6+5)
   </td>
   <td>
      <code>true</code>
   </td>
  </tr>
  <tr>
   <td>(6/2) != (6-3)
   </td>
   <td>
     <code>false</code>
   </td>
  </tr>
  <tr>
   <td>Math.pow(5, 2) > (5*2)
   </td>
   <td>
     <code>true</code>
   </td>
  </tr>
</table>



### Order of Operations

In Java, there is an order of precedence amongst its' operators.  Below is the list of operators and the order in which they are evaluated in an expression, listed from highest to lowest precedence. (There are many operators in this list we haven’t used yet, I’ve bolded the ones we’ve used so far)


<table>
  <tr>
   <td><strong>Level</strong>
   </td>
   <td><strong>Operator</strong>
   </td>
   <td><strong>Description</strong>
   </td>
   <td><strong>Associativity</strong>
   </td>
  </tr>
  <tr>
   <td><strong>16</strong>
   </td>
   <td><code>[]</code>
<p>
<code>.</code>
<p>
<code>()</code>
   </td>
   <td>access array element
<p>
access object member
<p>
parentheses
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>15</strong>
   </td>
   <td><code>++</code>
<p>
<code>--</code>
   </td>
   <td>unary post-increment
<p>
unary post-decrement
   </td>
   <td>not associative
   </td>
  </tr>
  <tr>
   <td><strong>14</strong>
   </td>
   <td><code>++</code>
<p>
<code>--</code>
<p>
<code>+</code>
<p>
<code>-</code>
<p>
<code>!</code>
<p>
<code>~</code>
   </td>
   <td>unary pre-increment
<p>
unary pre-decrement
<p>
unary plus
<p>
unary minus
<p>
unary logical NOT
<p>
unary bitwise NOT
   </td>
   <td>right to left
   </td>
  </tr>
  <tr>
   <td><strong>13</strong>
   </td>
   <td><code>()</code>
<p>
<code>new</code>
   </td>
   <td>cast
<p>
object creation
   </td>
   <td>right to left
   </td>
  </tr>
  <tr>
   <td><strong>12</strong>
   </td>
   <td><code>* / %</code>
   </td>
   <td>multiplicative
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>11</strong>
   </td>
   <td><code>+ -</code>
<p>
<code>+</code>
   </td>
   <td>additive
<p>
string concatenation
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>10</strong>
   </td>
   <td><code><&lt; >></code>
<p>
<code>>>></code>
   </td>
   <td>shift
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>9</strong>
   </td>
   <td><code>&lt; &lt;=</code>
<p>
<code>> >=</code>
<p>
<code>instanceof</code>
   </td>
   <td>relational
   </td>
   <td>not associative
   </td>
  </tr>
  <tr>
   <td><strong>8</strong>
   </td>
   <td><code>==</code>
<p>
<code>!=</code>
   </td>
   <td>equality
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>7</strong>
   </td>
   <td><code>&</code>
   </td>
   <td>bitwise AND
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>6</strong>
   </td>
   <td><code>^</code>
   </td>
   <td>bitwise XOR
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>5</strong>
   </td>
   <td><code>|</code>
   </td>
   <td>bitwise OR
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>4</strong>
   </td>
   <td><code>&&</code>
   </td>
   <td>logical AND
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>3</strong>
   </td>
   <td><code>||</code>
   </td>
   <td>logical OR
   </td>
   <td>left to right
   </td>
  </tr>
  <tr>
   <td><strong>2</strong>
   </td>
   <td><code>?:</code>
   </td>
   <td>ternary
   </td>
   <td>right to left
   </td>
  </tr>
  <tr>
   <td><strong>1</strong>
   </td>
   <td><code> =   +=   -=</code>
<p>
<code>*=   /=   %=</code>
<p>
<code>&=   ^=   |=</code>
<p>
<code><&lt;=  >>= >>>=</code>
   </td>
   <td>assignment
   </td>
   <td>right to left
   </td>
  </tr>
</table>



### Storing Boolean Values

We can store the result of boolean expressions in a variable:


### You Try
```
    boolean z = 4 < 5;
    System.out.println("The result of 4 < 5 is " + z);

    int x = 4;
    int y = 5;
    boolean t = x > y;
    System.out.println("The result of " + x + " > " + y + " is " + t);

```



In the example above, we store the result of our boolean expression x > y in the variable z. The output of this program would be the value of z, which is `false.`

It is import to reiterate that true or false are boolean values, hence, can be assigned directly to a variable.


```
int age = readInt("What is your age? ");
boolean blnCanWatchMovie = age >= 18;

int grade = readInt("What is your grade? ");
boolean blnHasA = 90 <= grade;
