<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The indicated [integration by substitution](../../../../../integration-by-substitution.md) gives

$$
u(x,t)=\frac1{\sqrt\pi}\int_{\mathbb R}
\varphi(x+2\sqrt t\,\eta)e^{-\eta^2}\,d\eta.
$$

Pointwise, the argument of $\varphi$ tends to $x$. Since the [Gaussian integral](../../../../../gaussian-integral.md) is $\int e^{-\eta^2}d\eta=\sqrt\pi$, the expected limit is $\varphi(x)$. To justify it for unbounded data, use the [approximate identity](../../../../../approximate-identity.md) property rather than assuming a uniform bound on $\varphi$.

In the original variable, normalization gives

$$
u(x,t)-\varphi(x)=\int_{\mathbb R}K(x-\xi,t)\bigl(\varphi(\xi)-\varphi(x)\bigr)\,d\xi.
$$

For $|\xi-x|<\delta$, [continuity](../../../../../continuous-function.md) makes the difference smaller than any prescribed $\varepsilon$ if $\delta$ is small enough, and the kernel mass is at most one. On the complement the Gaussian mass tends to zero; the data-weighted tail tends to zero by [heat-kernel convergence for Gaussian-integrable initial data](../../../../../heat-kernel-convergence-for-gaussian-integrable-initial-data.md). This proves

$$
\boxed{\lim_{t\downarrow0}u(x,t)=\varphi(x)}.
$$

For [heat-kernel convergence from a conditionally convergent Gaussian integral](../../../../../heat-kernel-convergence-from-a-conditionally-convergent-gaussian-integral.md), the same tail conclusion follows using the bounded primitive of $(\varphi(\xi)-\varphi(x))e^{-\xi^2/(4T)}$. The factor $q=K(x-\xi,t)e^{\xi^2/(4T)}$ has its maximum at $\xi=xT/(T-t)$, approaching $x$. For sufficiently small $t$, it is monotone on each of the two tails outside $|\xi-x|<\delta$, and its values at the tail endpoints tend to zero exponentially. [Integration by parts](../../../../../integration-by-parts.md) bounds each tail by a constant times its endpoint value, proving the same limit without an absolute-convergence assumption. The approach $t\downarrow0$ is from positive time.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
