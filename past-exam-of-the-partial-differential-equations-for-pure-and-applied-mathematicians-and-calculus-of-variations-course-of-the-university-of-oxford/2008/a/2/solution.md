<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose a smooth compactly supported [mollifier](../../../../mollifier.md) of integral one. On every compact subset of $\Omega$, and for sufficiently small $\varepsilon$, each translated [mollifier](../../../../mollifier.md) is an allowed test, so the assumption gives $w*\rho_\varepsilon=0$. The standard [mollifier](../../../../mollifier.md) approximation theorem gives $w*\rho_\varepsilon\to w$ in local $L^1$. Thus **$w=0$ [almost everywhere](../../../../almost-everywhere.md)**.

For a multi-index $\alpha$, the [weak derivative](../../../../weak-derivative.md) $v=D^\alpha u$ is the locally integrable function satisfying

$$
\boxed{\int_\Omega uD^\alpha\phi=(-1)^{|\alpha|}\int_\Omega v\phi\quad(\phi\in C_0^\infty(\Omega)).}
$$

Two such functions have zero pairing difference against every test, so the first result proves uniqueness. A compactly supported smooth test on an open subset $E$ extends by zero to one on $\Omega$, proving restriction of the derivative to $E$.

Put $w=D^\beta u$. For every test $\phi$ the defining identity applied to $D^\alpha\phi$ gives

$$
(-1)^{|\alpha|}\int wD^\alpha\phi=(-1)^{|\alpha|+|\beta|}\int uD^{\alpha+\beta}\phi.
$$

Thus these two [distributions](../../../../distribution-mathematical-analysis.md) are identical; one is represented by a locally integrable function if and only if the other is. Their [weak derivatives](../../../../weak-derivative.md) then agree, proving **$D^\alpha(D^\beta u)=D^{\alpha+\beta}u$** with exactly the asserted existence equivalence.

On $(0,2)$ the displayed piecewise affine function is continuous at one. [Integration by parts](../../../../integration-by-parts.md) separately on the two intervals shows its first [weak derivative](../../../../weak-derivative.md) is one on $(0,1)$ and minus one on $(1,2)$; the first boundary terms cancel by continuity. The derivative of that step function is $-2\delta_1$. This [distribution](../../../../distribution-mathematical-analysis.md) is not represented by a locally integrable function: tests of height one supported in shrinking neighborhoods of one have pairing $-2$ with it, whereas their integrals against any fixed local $L^1$ function tend to zero. Hence **there is a first [weak derivative](../../../../weak-derivative.md) but no locally integrable second [weak derivative](../../../../weak-derivative.md)**.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../split.md)
5. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
