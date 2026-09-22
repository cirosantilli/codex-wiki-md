<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the second form of the functional equation as

$$
\zeta(s)=\chi(s)\zeta(1-s),
\qquad
\chi(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s).
$$

For $-2\leq\sigma\leq2$, the elementary exponential formula for the [sine](../../../../../../sine.md) gives, uniformly for $t\geq4$,

$$
|\sin(\pi s/2)|\asymp e^{\pi t/2}.
$$

The stated [Stirling formula](../../../../../../stirling-formula.md) gives

$$
|\Gamma(1-s)|\asymp t^{1/2-\sigma}e^{-\pi t/2}
$$

uniformly on the same strip. The bounded factors $2^\sigma\pi^{\sigma-1}$ and the cancelling exponentials therefore show that

$$
|\chi(s)|\asymp t^{1/2-\sigma}.
$$

Taking absolute values in the functional equation proves the [Vertical-strip factor in the Riemann zeta functional equation](../../../../../../vertical-strip-factor-in-the-riemann-zeta-functional-equation.md):

$$
\boxed{|\zeta(s)|\asymp t^{1/2-\sigma}|\zeta(1-s)|}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
