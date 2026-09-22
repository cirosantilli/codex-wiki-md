<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $T_\alpha=A^*A+\alpha I$. For every $f\in X$,

$$
\alpha\|f\|_X^2
\leq\langle f,T_\alpha f\rangle_X
=\|Af\|_Y^2+\alpha\|f\|_X^2
\leq(\|A\|^2+\alpha)\|f\|_X^2.
$$

Thus $T_\alpha$ is a [coercive operator](../../../../../../../coercive-operator.md). If it is invertible and $T_\alpha f=g$, the lower bound and the [Cauchy-Schwarz inequality](../../../../../../../cauchy-schwarz-inequality.md) give

$$
\alpha\|f\|^2\leq\langle f,g\rangle\leq\|f\|\|g\|,
$$

and therefore $\|T_\alpha^{-1}g\|\leq\alpha^{-1}\|g\|$. Hence

$$
\boxed{\|(A^*A+\alpha I)^{-1}\|\leq\frac1\alpha}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
