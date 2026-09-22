<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Regard the alphabet as the cyclic group $\mathbb Z/m\mathbb Z$ and put $E=X-Y$. For each $y$, subtraction by $y$ is a bijection, so

$$
H(X\mid Y=y)=H(E\mid Y=y)\leq\phi(d_y),
\qquad
d_y=\mathbb P(X\ne Y\mid Y=y).
$$

By concavity of $\phi$, its monotonicity in the distortion allowance, and $\mathbb E d_Y=\mathbb P(X\ne Y)\leq d$,

$$
H(X\mid Y)
\leq\mathbb E\phi(d_Y)
\leq\phi(\mathbb E d_Y)
\leq\phi(d).
$$

Therefore

$$
\boxed{I(X;Y)=H(X)-H(X\mid Y)\geq H(X)-\phi(d).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
