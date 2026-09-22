<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The number $K$ is fixed. By [Big O notation](../../../../../big-o-notation.md), for each $i$ there are constants $C_i>0$ and $N_i$ such that $f_i(n)\leq C_i g(n)$ when $n\geq N_i$. Take $N=\max_iN_i$. For $n\geq N$, positivity gives

$$
h(n)\leq\left(\sum_{i=1}^K C_i\right)g(n),
\qquad
l(n)\leq\left(\sum_{i=1}^{K-1}C_iC_{i+1}\right)g(n)^2.
$$

The constants in parentheses are independent of $n$, proving $\boxed{h=O(g),\quad l=O(g^2)}$. If $K=1$, the second sum is empty and $l=0$, which satisfies the same upper bound.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2014](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
