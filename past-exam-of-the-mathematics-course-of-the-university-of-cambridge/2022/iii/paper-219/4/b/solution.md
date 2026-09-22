<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Under $M_1$, [Bayes' theorem](../../../../../../bayes-theorem.md) at the nested value $\psi=0$ gives

$$
p(\psi=0\mid D,M_1)
=\frac{p(D\mid\psi=0,M_1)p(\psi=0\mid M_1)}{p(D\mid M_1)}.
$$

Separability of the prior and equality of the $\phi$ priors imply

$$
p(D\mid\psi=0,M_1)
=\int p(D\mid\phi,\psi=0,M_1)p(\phi\mid M_1)\,d\phi
=p(D\mid M_0).
$$

Rearranging proves the [Savage-Dickey density ratio](../../../../../../savage-dickey-density-ratio.md)

$$
B_{01}
=\frac{p(D\mid M_0)}{p(D\mid M_1)}
=\left.
\frac{p(\psi\mid D,M_1)}{p(\psi\mid M_1)}
\right|_{\psi=0},
$$

which is the [Bayes factor](../../../../../../bayes-factor.md) in favor of the nested model.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 219](../../../paper-219-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
