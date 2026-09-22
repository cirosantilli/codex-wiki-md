<h1 id="17/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take $\sigma>0$ and substitute $u=(x-\mu)/\sigma$. The density becomes the standard [Gaussian distribution](../../../../../normal-distribution.md) density $\varphi(u)=e^{-u^2/2}/\sqrt{2\pi}$. Its normalization follows from the supplied [Gaussian integral](../../../../../gaussian-integral.md) after scaling by $\sqrt2$. Since $u\varphi(u)$ is an integrable [odd function](../../../../../odd-function.md), its integral is zero, and therefore $\mathbb EX=\mu$.

For the second moment, $\varphi'=-u\varphi$. [Integration by parts](../../../../../integration-by-parts.md) gives

$$
\int_{-\infty}^{\infty}u^2\varphi(u)du=-[u\varphi(u)]_{-\infty}^{\infty}+\int_{-\infty}^{\infty}\varphi(u)du=1.
$$

The endpoint term vanishes by Gaussian decay. Consequently

$$
\boxed{\mathbb EX=\mu,\qquad\operatorname{Var}X=\sigma^2.}
$$

## ↑ Ancestors (13)

1. [B](../b.md)
2. [17](../../17.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
