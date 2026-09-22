<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [Itô formula](../../../../../../ito-s-lemma.md) to $Z_t^{(A)}=\exp(A X_t-A^2t/2)$. Its [semimartingale decomposition](../../../../../../semimartingale-decomposition.md) is

$$
dZ_t^{(A)}=A Z_t^{(A)}\,dX_t
+\frac{A^2}{2}Z_t^{(A)}\bigl(d[X]_t-dt\bigr).
$$

The second term is a continuous [finite-variation process](../../../../../../finite-variation-process.md). Since $Z^{(A)}$ is assumed to be a [local martingale](../../../../../../local-martingale.md), uniqueness of the semimartingale decomposition makes this term identically zero. Both $A$ and $Z^{(A)}$ are nonzero, so the [quadratic variation](../../../../../../quadratic-variation.md) of $X$ is $[X]_t=t$.

The [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md) now says that $X_t-X_0$ is a [Brownian motion](../../../../../../brownian-motion-split.md). Consequently

$$
Z_t^{(a)}=e^{aX_0}
\exp\!\left(a(X_t-X_0)-\frac{a^2t}{2}\right)
$$

is a constant multiple of an [exponential Brownian martingale](../../../../../../exponential-brownian-martingale.md). It is therefore a true martingale for every $a\in\mathbb R$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
