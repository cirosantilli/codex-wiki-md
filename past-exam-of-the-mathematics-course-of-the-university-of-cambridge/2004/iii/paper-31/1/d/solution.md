<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let epsilon decrease to zero in the upper estimate. In the lower estimate first take the [supremum](../../../../../../supremum.md) over all chosen points and then decrease epsilon to zero. The bounds coincide, proving [Varadhan lemma](../../../../../../varadhan-s-lemma.md):

$$
\boxed{\lim_{n\to\infty}\frac1n\log\mathbb E e^{nf(X_n)}=\sup_{x\in\mathcal X}\{f(x)-I(x)\}.}
$$

The value is finite: f is bounded, $I\geq0$, and the large-deviation bounds on the whole space force $\inf I=0$. This proof actually uses bounded [continuity](../../../../../../continuous-function.md) and the [large deviation principle](../../../../../../large-deviation-principle.md); compact sublevels are not additionally needed for this bounded version.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 31](../../../paper-31-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
