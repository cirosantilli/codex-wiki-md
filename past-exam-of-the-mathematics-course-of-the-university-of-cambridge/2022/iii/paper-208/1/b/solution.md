<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set

$$
Z=\frac{e^{\lambda X}}{M(\lambda)},
\qquad \mathbb EZ=1.
$$

Under the probability measure with density $Z$, the [Jensen inequality](../../../../../../jensen-s-inequality.md) for the concave logarithm gives

$$
\frac{\operatorname{Ent}(e^{\lambda X})}{M(\lambda)}
=\mathbb E[Z\log Z]
\leq\log\mathbb E[Z^2]
=\log\frac{M(2\lambda)}{M(\lambda)^2}.
$$

The sub-Gaussian assumption with variance parameter $\nu/4$ gives $M(2\lambda)\leq e^{\nu\lambda^2/2}$. A second application of [Jensen inequality](../../../../../../jensen-s-inequality.md) gives $M(\lambda)\geq e^{\lambda\mathbb EX}=1$. Consequently

$$
\operatorname{Ent}(e^{\lambda X})
\leq\frac{\nu\lambda^2}{2}M(\lambda),
$$

as required.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
