<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $h=\sqrt{1-m^2}$ be the complementary modulus of the [complete elliptic integral of the first kind](../../../../../../../complete-elliptic-integral-of-the-first-kind.md). With $\varphi=\pi/2-\theta$, write the integrand as $(\sin^2\varphi+h^2\cos^2\varphi)^{-1/2}$. Its [logarithmic endpoint asymptotic of the complete elliptic integral](../../../../../../../logarithmic-endpoint-asymptotic-of-the-complete-elliptic-integral.md) comes from $\varphi=O(h)$; an expansion at fixed $\varphi$ alone misses the constant accompanying the logarithm.

Choose an intermediate cutoff $h\ll d\ll1$. In the endpoint region, the integral is

$$
\int_0^d\frac{d\varphi}{\sqrt{\varphi^2+h^2}}=\operatorname{arsinh}(d/h)=\log\frac{2d}{h}+o(1).
$$

Outside this region, the leading integral is

$$
\int_d^{\pi/2}\frac{d\varphi}{\sin\varphi}=-\log\tan(d/2)=\log\frac2d+o(1).
$$

The arbitrary cutoff cancels in this [matched asymptotic expansion](../../../../../../../matched-asymptotic-expansion.md), leaving

$$
\boxed{K(m)=\log\frac4{\sqrt{1-m^2}}+o(1)=-\frac12\log(1-m)+\log(2\sqrt2)+o(1).}
$$

These are the divergent logarithm and the finite constant, the requested first two terms. If terms are instead grouped by powers of the complementary modulus, the next refinement is $K(m)=\log(4/h)+(h^2/4)[\log(4/h)-1]+O(h^4\log(1/h))$; its coefficients agree with [the DLMF expansion](https://dlmf.nist.gov/19.12.E1).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 79](../../../../paper-79-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
