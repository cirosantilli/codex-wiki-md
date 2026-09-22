<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Laplace-transform formula for a semigroup resolvent](../../../../../../laplace-transform-formula-for-a-semigroup-resolvent.md) is locally uniformly convergent in the half-plane $\operatorname{Re}z>\omega$, so it may be differentiated under the [Bochner integral](../../../../../../bochner-integral.md):

$$
\frac{d^n}{dz^n}R(z)u
=(-1)^n\int_0^\infty t^ne^{-tz}U(t)u\,dt.
$$

The [resolvent identity](../../../../../../resolvent-identity.md) gives $R'(z)=-R(z)^2$ and, by [mathematical induction](../../../../../../mathematical-induction.md),

$$
\frac{d^n}{dz^n}R(z)=(-1)^nn!R(z)^{n+1}.
$$

Therefore

$$
\boxed{n!(zI-A)^{-(n+1)}u
=\int_0^\infty t^ne^{-tz}U(t)u\,dt}.
$$

For real $\lambda>\omega$, the [integral triangle inequality](../../../../../../integral-triangle-inequality.md) and the [Gamma integral](../../../../../../gamma-integral.md) give

$$
\begin{aligned}
n!\|(\lambda I-A)^{-(n+1)}u\|
&\leq M\|u\|\int_0^\infty t^ne^{-(\lambda-\omega)t}\,dt\\
&=\frac{Mn!}{(\lambda-\omega)^{n+1}}\|u\|.
\end{aligned}
$$

Consequently

$$
\boxed{\|(\lambda I-A)^{-(n+1)}u\|
\leq\frac{M}{(\lambda-\omega)^{n+1}}\|u\|}.
$$

The exponent $-n+1$ printed in the question is a typographical error: already at $n=0$ it contradicts the first-resolvent bound.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 319](../../../paper-319-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
