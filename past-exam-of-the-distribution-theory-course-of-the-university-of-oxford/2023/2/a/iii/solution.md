<h1 id="2/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [L1-normalized dilation of a distribution](../../../../../l1-normalized-dilation-of-a-distribution.md) is

$$
\boxed{\langle u_\varepsilon,\phi\rangle=\langle u,\phi(\varepsilon\,\cdot)\rangle.}
$$

For a [regular distribution](../../../../../regular-distribution.md) this is the [function](../../../../../function-split.md) $u_\varepsilon(x)=\varepsilon^{-1}u(x/\varepsilon)$. In terms of the wiki's [dilation of a distribution](../../../../../dilation-of-a-distribution.md) convention, $u_\varepsilon=\varepsilon^{-1}\delta_{1/\varepsilon}u$; the normalization preserves the [L1 space](../../../../../l1-space.md) norm.

If $u\in L^1(\mathbb R)$, the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md), with dominating [integrable function](../../../../../lebesgue-integrable-function.md) $|u(y)|\|\phi\|_\infty$, gives

$$
\langle u_\varepsilon,\phi\rangle=\int u(y)\phi(\varepsilon y)\,dy
\longrightarrow\phi(0)\int u(y)\,dy.
$$

Consequently

$$
\boxed{u_\varepsilon\longrightarrow\left(\int_{\mathbb R}u\right)\delta_0
\quad\text{in }\mathcal D'(\mathbb R).}
$$

An arbitrary [distribution](../../../../../distribution-mathematical-analysis.md) need not have this behavior. Take the constant [regular distribution](../../../../../regular-distribution.md) $u=1$. Then $u_\varepsilon=\varepsilon^{-1}$, so for a [test function](../../../../../test-function.md) with integral one,

$$
\langle u_\varepsilon,\phi\rangle=\varepsilon^{-1}\longrightarrow+\infty.
$$

Hence $\boxed{u=1\text{ gives no distributional limit}}$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
