<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathbf e_i$ be the $i$th coordinate vector and take $p$ to be zero whenever any argument is negative. Right jumps $i\to i+1$, left jumps $i\to i-1$, and absorption from compartment $1$ give the [chemical master equation](../../../../../../chemical-master-equation.md)

$$
\begin{aligned}
\partial_t p(\mathbf a,t)
={}&\sum_{i=1}^{m-1}k_i^+
\left[(a_i+1)p(\mathbf a+\mathbf e_i-\mathbf e_{i+1},t)
-a_ip(\mathbf a,t)\right]\\
&+\sum_{i=2}^{m}k_i^-
\left[(a_i+1)p(\mathbf a-\mathbf e_{i-1}+\mathbf e_i,t)
-a_ip(\mathbf a,t)\right]\\
&+k_1^-\left[(a_1+1)p(\mathbf a+\mathbf e_1,t)
-a_1p(\mathbf a,t)\right].
\end{aligned}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 356](../../../paper-356-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
