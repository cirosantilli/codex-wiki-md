<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The functions are nonnegative and normalized to have integral one. On the disk $|x|\leq(2n)^{-1/4}$, [Bernoulli inequality](../../../../../../bernoulli-s-inequality.md) gives $(1-|x|^4)^n\geq1-n|x|^4\geq1/2$. Consequently

$$
c_n^{-1}\geq\frac12\pi(2n)^{-1/2},
\qquad \boxed{c_n\leq\frac{2\sqrt{2n}}{\pi}.}
$$

For any fixed $0<a<1$, the mass outside radius $a$ is at most

$$
\int_{|x|\geq a}g_n(x)\,dx
\leq\pi c_n(1-a^4)^n
\leq2\sqrt{2n}(1-a^4)^n\longrightarrow0.
$$

This is an [approximate identity](../../../../../../approximate-identity.md). For any test function,

$$
\left|\int g_n\varphi-\varphi(0)\right|
\leq\sup_{|x|\leq a}|\varphi(x)-\varphi(0)|
+2\|\varphi\|_\infty\int_{|x|\geq a}g_n.
$$

Let $n\to\infty$ and then $a\downarrow0$ to conclude $\boxed{g_n\to\delta_0\text{ in }\mathcal D'(\mathbb R^2)}$.

Polar coordinates also give the exact normalization through the [beta function](../../../../../../beta-function.md):

$$
c_n^{-1}=\frac\pi2B(1/2,n+1),\qquad
c_n=\frac{2\Gamma(n+3/2)}{\pi^{3/2}\Gamma(n+1)}.
$$

<a id="4/c/image-normalized-radial-densities-and-cumulative-mass-concentrating-at-the-origin"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-9-radial-approximate-identity.png)

**[Figure 1](#4/c/image-normalized-radial-densities-and-cumulative-mass-concentrating-at-the-origin). Normalized radial densities and cumulative mass concentrating at the origin**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
