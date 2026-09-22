<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By part (a), every nontrivial zero $\rho=\beta+i\gamma$ with $|\gamma|\le T$ satisfies $\beta\le1-c_1/\log^9T$ for large $T$, after reducing the positive constant. The [local zero count for the Riemann zeta function](../../../../../../local-zero-count-for-the-riemann-zeta-function.md) gives

$$
\sum_{|\gamma|\le T}\frac1{|\rho|}\ll1+\sum_{1\le j\le T}\frac{\log(j+3)}j\ll\log^2T.
$$

There are finitely many zeros at bounded height, none at zero or at one, so that part of the sum is bounded. The [truncated explicit formula for the second Chebyshev function](../../../../../../truncated-explicit-formula-for-the-second-chebyshev-function.md) now yields

$$
\boxed{\psi(x)=x+O\bigl(x^{1-c_1/\log^9T}\log^2x\bigr)+O\left(\frac{x\log^2x}T\right),\qquad2\le T\le x.}
$$

Balance the exponent losses $c_1\log x/(\log T)^9$ and $\log T$ by choosing $\log T=(c_1\log x)^{1/10}$. This is the optimal order obtainable from these two errors: making either exponent larger forces the other smaller. Thus, for a positive constant $c_2$,

$$
\boxed{\psi(x)-x\ll x\log^2x\exp\bigl(-c_2(\log x)^{1/10}\bigr).}
$$

The logarithmic prefactor can be absorbed by reducing $c_2$. This is the [prime number theorem error from a logarithmic zero-free region](../../../../../../prime-number-theorem-error-from-a-logarithmic-zero-free-region.md) with ninth-power width.

Under the [Riemann hypothesis](../../../../../../riemann-hypothesis.md), $|x^\rho|=x^{1/2}$. The same reciprocal-zero sum bounds the zero contribution by $O(x^{1/2}\log^2T)$. Taking $T=x$ makes the truncation error $O(\log^2x)$, so

$$
\boxed{\psi(x)=x+O(x^{1/2}\log^2x).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
