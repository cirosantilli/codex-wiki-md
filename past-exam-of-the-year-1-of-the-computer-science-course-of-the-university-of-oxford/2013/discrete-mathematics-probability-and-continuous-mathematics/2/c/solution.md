<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By [Big O notation](../../../../../big-o-notation.md), there are $C_1,C_2>0$ and thresholds after which $f_1(n)\leq C_1g_1(n)$ and $f_2(n)\leq C_2g_2(n)$. Choose a common threshold and set $C=\max(C_1,C_2)$. The positivity assumption gives

$$
0\leq f_1(n)+f_2(n)\leq C(g_1(n)+g_2(n)).
$$

Squaring preserves this inequality, so

$$
\boxed{(f_1+f_2)^2\leq C^2(g_1+g_2)^2\text{ eventually},\qquad(f_1+f_2)^2=O((g_1+g_2)^2).}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [Discrete mathematics, probability and continuous mathematics](../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
