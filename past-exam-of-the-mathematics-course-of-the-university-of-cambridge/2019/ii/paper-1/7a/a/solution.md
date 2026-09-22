<h1 id="7a/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With $u=x^4$, the [change of variables formula](../../../../../../change-of-variables-formula.md) gives

$$
\int_0^1\frac{dx}{\sqrt{1-x^4}}
=\frac14\int_0^1u^{-3/4}(1-u)^{-1/2}\,du
=\frac14B\left(\frac14,\frac12\right).
$$

The [beta--gamma identity](../../../../../../beta-gamma-identity.md), $\Gamma(1/2)=\sqrt\pi$, and the [Gamma reflection formula](../../../../../../gamma-reflection-formula.md) give

$$
\frac14B\left(\frac14,\frac12\right)
=\frac{\Gamma(1/4)\sqrt\pi}{4\Gamma(3/4)},
\qquad
\Gamma(1/4)\Gamma(3/4)=\pi\sqrt2.
$$

Therefore

$$
\boxed{\int_0^1\frac{dx}{\sqrt{1-x^4}}
=\frac{\Gamma(1/4)^2}{\sqrt{32\pi}}}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7A](../../7a.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
