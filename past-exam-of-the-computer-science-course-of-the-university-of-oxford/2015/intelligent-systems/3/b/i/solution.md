<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose the distinct values of $(X_1,X_2,X_4)$ and call them $(a,b,c)$. There are $3!=6$ choices. Constraint (5), on $(X_1,X_4,X_9)$, immediately forces $X_9=b$.

Constraints (2) and (3) require $X_5\ne X_2=b$ and $X_5\ne X_4=c$, respectively. Since the [constraint domain](../../../../../../constraint-domain.md) has exactly three values, $X_5=a$. Constraint (2) now forces $X_3=c$, and constraint (3) forces $X_6=b$. Finally, constraint (4) permits $(X_7,X_8)=(a,c)$ or $(c,a)$.

Every choice just described satisfies all five [all-different constraints](../../../../../../all-different-constraint.md), and the forced-value argument shows there are no other possibilities. Hence

$$
\boxed{\#\operatorname{Sol}(P)=3!\cdot2=12.}
$$

In the order $(X_1,\ldots,X_9)$, the two forms are

$$
(a,b,c,c,a,b,a,c,b),\qquad
(a,b,c,c,a,b,c,a,b),
$$

where $(a,b,c)$ ranges over the six [permutations](../../../../../../permutation.md) of $(0,1,2)$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Intelligent systems](../../../../intelligent-systems-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
