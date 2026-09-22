<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By [locality of weak differentiability](../../../../../../locality-of-weak-differentiability.md), it is enough to work near the exceptional point; translate it to zero. Let $g_i$ denote the classical derivative off zero, assigning any value at zero. For $\phi\in C_c^\infty(\Omega)$ choose a smooth cutoff $\chi_\varepsilon$ which is zero on $B_\varepsilon$, one outside $B_{2\varepsilon}$, satisfies $|D\chi_\varepsilon|\leq C/\varepsilon$, and has its transition region contained in $\Omega$. The product $\phi\chi_\varepsilon$ avoids the singular point, so classical integration by parts gives

$$
\int u\chi_\varepsilon D_i\phi+\int u\phi D_i\chi_\varepsilon
=-\int g_i\phi\chi_\varepsilon.
$$

The middle term has absolute value at most

$$
\|u\|_\infty\|\phi\|_\infty\frac C\varepsilon |B_{2\varepsilon}|\leq C'\varepsilon^{n-1}\longrightarrow0
$$

when $n\geq2$. The other terms tend to $\int uD_i\phi$ and $-\int g_i\phi$, since $u$ is [locally integrable](../../../../../../locally-integrable-function.md) and $g_i\in L^1_{\mathrm{loc}}$. Therefore $\boxed{D_i u=g_i\text{ weakly on all of }\Omega}$. Its value at the single point is irrelevant. This is [bounded isolated-point removability for weak first derivatives](../../../../../../bounded-isolated-point-removability-for-weak-first-derivatives.md).

For $n=1$, take $u(x)=0$ for $x<0$ and $u(x)=1$ for $x>0$ on $(-1,1)$, with any value at zero. It is bounded and $C^1$ off zero, with classical derivative zero there. But

$$
\int_{-1}^1u\phi'=-\phi(0),
$$

so its [distributional derivative](../../../../../../distributional-derivative.md) is a [Dirac delta](../../../../../../dirac-delta-function.md). If a [locally integrable](../../../../../../locally-integrable-function.md) [weak derivative](../../../../../../weak-derivative.md) existed, it would be zero off zero and hence zero [almost everywhere](../../../../../../almost-everywhere.md), contradicting this identity. The step function is the required counterexample; the cutoff error in dimension one need not vanish.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
