<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [weak convergence of distributions](../../../../../weak-convergence-of-distributions.md) $u_j\to u$ means

$$
\langle u_j,\phi\rangle\longrightarrow\langle u,\phi\rangle
\quad\text{for every }\phi\in\mathcal D(\mathbb R).
$$

For $\theta\in\mathcal D(\mathbb R)$, its [convolution](../../../../../convolution.md) with a [distribution](../../../../../distribution-mathematical-analysis.md) is the [smooth function](../../../../../smooth-function.md)

$$
(\theta*u)(x)=\langle u_y,\theta(x-y)\rangle.
$$

The subscript records the variable on which the [distribution](../../../../../distribution-mathematical-analysis.md) acts. With $\check\theta(x)=\theta(-x)$, its [regular distribution](../../../../../regular-distribution.md) satisfies the useful pairing identity

$$
\langle\theta*u,\phi\rangle=\langle u,\check\theta*\phi\rangle.
$$

Indeed integrating $\theta(x-y)\phi(x)$ in $x$ gives $(\check\theta*\phi)(y)$; continuity of the [distribution](../../../../../distribution-mathematical-analysis.md) justifies moving the pairing through that integral, by approximation with sums of [test functions](../../../../../test-function.md) in one common [compact support](../../../../../compact-support.md).

Part (i), applied to the reflected [mollifier](../../../../../mollifier.md), gives $\check\rho_\varepsilon*\phi\to\phi$ in the [space of test functions](../../../../../space-of-test-functions.md). Continuity of $u$ therefore proves

$$
\boxed{\langle\rho_\varepsilon*u,\phi\rangle
=\langle u,\check\rho_\varepsilon*\phi\rangle\longrightarrow\langle u,\phi\rangle,
\qquad\rho_\varepsilon*u\to u\text{ in }\mathcal D'.}
$$

Reflection is harmless even if the chosen standard [mollifier](../../../../../mollifier.md) is not even.

For the [mollifiers](../../../../../mollifier.md) themselves, a change of variable gives

$$
\langle\rho_\varepsilon,\phi\rangle=\int\rho(y)\phi(\varepsilon y)\,dy\longrightarrow\phi(0)\int\rho(y)\,dy=\phi(0).
$$

Thus $\boxed{\rho_\varepsilon\to\delta_0\text{ in }\mathcal D'(\mathbb R)}$, with limit the [Dirac delta distribution](../../../../../dirac-delta-function.md), despite the failure of convergence in the [L1 space](../../../../../l1-space.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
