<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume first the [Riemann hypothesis](../../../../../../riemann-hypothesis.md). Replace any $x\geq2$ by $y=\lfloor x\rfloor+1/2$; then $\psi(x)=\psi(y)$ and $\langle y\rangle\geq1/2$. Take $T=y$ in part a. Every nontrivial zero has real part $1/2$, and the [Riemann–von Mangoldt formula](../../../../../../riemann-von-mangoldt-formula.md) implies

$$
\sum_{|\gamma|\leq y}\frac1{|\rho|}\ll(\log y)^2.
$$

Consequently

$$
\sum_{|\gamma|\leq y}\left|\frac{y^\rho}{\rho}\right|
\ll y^{1/2}(\log y)^2,
$$

while both truncation errors in part a are $O((\log y)^2)$. Thus

$$
\psi(x)=x+O\left(x^{1/2}(\log x)^2\right),
$$

which implies the stated $O_\epsilon(x^{1/2+\epsilon})$ estimate.

Conversely, suppose that estimate holds for every $\epsilon>0$. For $\Re s>1$, [partial summation](../../../../../../abel-s-summation-formula.md) gives

$$
-\frac{\zeta'(s)}{\zeta(s)}
=s\int_1^\infty\psi(x)x^{-s-1}\,dx
=\frac{s}{s-1}
+s\int_1^\infty(\psi(x)-x)x^{-s-1}\,dx.
$$

Given any $s$ with $\Re s>1/2$, choose $\epsilon<\Re s-1/2$. The error hypothesis makes the last integral locally uniformly convergent there, so it supplies a holomorphic continuation of

$$
-\frac{\zeta'(s)}{\zeta(s)}-\frac{s}{s-1}
$$

to the half-plane $\Re s>1/2$. A zero of $\zeta$ in that half-plane would create a pole of its [logarithmic derivative](../../../../../../logarithmic-derivative.md), so none exists. The [functional equation of the Riemann zeta function](../../../../../../functional-equation-of-the-riemann-zeta-function.md) reflects every nontrivial zero with real part below $1/2$ to one above $1/2$. All nontrivial zeros must therefore lie on the [critical line](../../../../../../critical-line.md), proving the [Riemann hypothesis equivalence for the second Chebyshev function](../../../../../../riemann-hypothesis-equivalence-for-the-second-chebyshev-function.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
