<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [integer](../../../../../integer-split.md) cell coordinate, occupancy is an existential [predicate](../../../../../predicate.md):

$$
\boxed{\operatorname{contains}(W,x,y)\iff
\exists i:\quad y=y_i\ \land\ x_i\le x<x_i+w_i.}
$$

The first occupied unit cell of brick $i$ is at $x_i$, and its last is at $x_i+w_i-1$. Thus the required support [predicate](../../../../../predicate.md), with the baseplate explicitly included, is

$$
\boxed{\operatorname{supportive}(W)\iff
\forall i:\quad y_i=0\ \lor\
\left(y_i>0\ \land\
\operatorname{contains}(W,x_i,y_i-1)\ \land\
\operatorname{contains}(W,x_i+w_i-1,y_i-1)\right).}
$$

For width one, the two support cells coincide. For a wider brick, its middle may bridge an empty gap; the question only requires support beneath its two ends. Checking $x_i+w_i$ would incorrectly examine a cell beyond the brick's right end. The potentially infinite baseplate supplies every required support at height zero.[p. 6, Question 3(c), and p. 7, Figure 3](../../../../../object-oriented-programming-examination-paper-of-the-university-of-oxford-2015.md)

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Object oriented programming](../../../object-oriented-programming-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
