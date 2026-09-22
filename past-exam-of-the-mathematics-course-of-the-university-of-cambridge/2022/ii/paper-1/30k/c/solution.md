<h1 id="30k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At time $n$, the minimizing feedback from part (b) is

$$
u_n^*=-\frac{X_{n-1}}{N-n+2}.
$$

Starting with $u_1^*=-X_0/(N+1)$ and repeatedly substituting  
$X_j=X_{j-1}+u_j^*+\xi_j$ gives by induction

$$
X_{n-1}=\frac{N-n+2}{N+1}X_0
+\sum_{j=1}^{n-1}\frac{N-n+2}{N-j+1}\xi_j.
$$

Therefore

$$
\boxed{u_n^*=-\frac{X_0}{N+1}-\frac{\xi_1}{N}
-\frac{\xi_2}{N-1}-\cdots-\frac{\xi_{n-1}}{N-n+2}},
$$

as required.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [30K](../../30k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
