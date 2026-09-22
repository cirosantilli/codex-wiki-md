<h1 id="15/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Put $w=e^x-1=x+x^2/2+x^3/6+O(x^4)$. The local [logarithmic series](../../../../../mercator-series.md) $\ln(1-w)=-w-w^2/2-w^3/3+O(w^4)$ gives

$$
\boxed{\ln(2-e^x)=-x-x^2-x^3+O(x^4).}
$$

For the infinite [Taylor series](../../../../../taylor-series.md), it is necessary to distinguish the real domain of the logarithm, $x<\ln2$, from its convergence interval about zero. Write $a=\ln2$. The complex zeros of $2-e^z$ are $a+2\pi i k$ for integers $k$, so the nearest [logarithmic singularity](../../../../../logarithmic-singularity.md) to zero is at $a$. The [radius of convergence](../../../../../radius-of-convergence.md) is therefore $a$, giving convergence for $|x|<a$ and divergence for $|x|>a$.

The two endpoints need separate checking. Factor off the nearest singularity:

$$
h(z)=\ln(1-z/a)+H(z),\qquad H(z)=\ln\left(\frac{2-e^z}{1-z/a}\right),\qquad H(0)=0.
$$

The quotient has a nonzero removable value $2a$ at $z=a$; its other zeros are at $a+2\pi i k$ with $k\ne0$. Consequently it has a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) on a zero-free disk larger than $|z|\le a$, which is a [simply connected domain](../../../../../simply-connected-domain.md), and the [Taylor series](../../../../../taylor-series.md) of $H$ converges absolutely at both real endpoints. At $x=-a$, the remaining series $-\sum_{n\ge1}(-1)^n/n$ converges by the [alternating series test](../../../../../alternating-series-test.md). At $x=a$, it is $-\sum_{n\ge1}1/n$ and diverges. Thus the full real convergence set is

$$
\boxed{-\ln2\le x<\ln2.}
$$

Convergence is absolute in the open interval and conditional at the left endpoint, where the sum equals $\ln(3/2)$. This endpoint distinction is an instance of [isolating a logarithmic singularity to test a power-series endpoint](../../../../../isolating-a-logarithmic-singularity-to-test-a-power-series-endpoint.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [15](../../15.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
