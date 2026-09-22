<h1 id="9g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every $x$,

$$
\|\alpha x\|^2=\langle x,\alpha^*\alpha x\rangle,
\qquad
\|\alpha^*x\|^2=\langle x,\alpha\alpha^*x\rangle.
$$

If $\alpha$ is normal, these quantities are equal. Conversely, equality of the norms for all $x$ gives

$$
\langle x,(\alpha^*\alpha-\alpha\alpha^*)x\rangle=0.
$$

The operator in parentheses is self-adjoint, so polarization makes it zero. Therefore

$$
\boxed{\alpha\alpha^*=\alpha^*\alpha
\iff \|\alpha x\|=\|\alpha^*x\|\quad\hbox{for all }x}.
$$

The same equivalence holds over a real [inner product](../../../../../../inner-product.md) space: for a self-adjoint operator $T$, the real polarization identity

$$
4\langle Tx,y\rangle
=\langle T(x+y),x+y\rangle
-\langle T(x-y),x-y\rangle
$$

shows that a vanishing quadratic form forces $T=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9G](../../9g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
