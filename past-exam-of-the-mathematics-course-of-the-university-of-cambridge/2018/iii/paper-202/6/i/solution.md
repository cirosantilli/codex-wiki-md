<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret the [Stratonovich integral](../../../../../../stratonovich-integral.md) in its standard extension to continuous [semimartingale](../../../../../../semimartingale.md) integrands:

$$
\int_0^tY_s\circ dX_s=\int_0^tY_s\,dX_s+\frac12[Y,X]_t.
$$

This extension is needed because $f'(X)$ is generally a [semimartingale](../../../../../../semimartingale.md) rather than a [local martingale](../../../../../../local-martingale.md). Also the introductory prose in the PDF reverses integrand and integrator relative to its displayed definition; the displayed definition fixes the convention used here.

Apply the [Itô formula](../../../../../../ito-s-lemma.md) to $f'(X)$, using $f\in C^3$:

$$
df'(X_s)=f''(X_s)\,dX_s+\frac12f'''(X_s)\,d\langle X\rangle_s.
$$

The continuous [finite-variation process](../../../../../../finite-variation-process.md) in the second term has zero [quadratic covariation](../../../../../../quadratic-covariation.md) with $X$, while the [quadratic covariation](../../../../../../quadratic-covariation.md) rule for an [Itô integral](../../../../../../ito-integral.md) gives

$$
[f'(X),X]_t=\int_0^tf''(X_s)\,d\langle X\rangle_s.
$$

A second application of the [Itô formula](../../../../../../ito-s-lemma.md), now to $f(X)$, therefore yields

$$
\boxed{f(X_t)-f(X_0)=\int_0^tf'(X_s)\circ dX_s.}
$$

All unbounded coefficients are handled by stopping $X$ on compact spatial intervals, then removing the [localizing sequence](../../../../../../localizing-sequence.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
