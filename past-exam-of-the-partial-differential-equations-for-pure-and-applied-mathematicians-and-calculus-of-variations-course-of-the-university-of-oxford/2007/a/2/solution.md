<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The first [weak derivative](../../../../weak-derivative.md) $D_ju=v$ is characterized by $\int_\Omega u\,\partial_j\phi=-\int_\Omega v\phi$ for every $\phi\in C_c^\infty(\Omega)$. The [fundamental lemma of the calculus of variations](../../../../fundamental-lemma-of-the-calculus-of-variations.md) in the locally integrable form says that a [function](../../../../function-split.md) pairing to zero with every such test is zero almost everywhere. Applied to the difference of two candidate derivatives, it proves uniqueness. The [Sobolev space](../../../../sobolev-space-split.md) consists of $u\in L^p$ with all first [weak derivatives](../../../../weak-derivative.md) in $L^p$, with [norm](../../../../norm.md)

$$
\boxed{\|u\|_{W^{1,p}}=\left(\|u\|_p^p+\sum_{j=1}^n\|D_ju\|_p^p\right)^{1/p}.}
$$

For the one-dimensional tent, [integration by parts](../../../../integration-by-parts.md) on each side of one has cancelling junction terms because the [function](../../../../function-split.md) is continuous. Thus **$u'=1$ on $(0,1)$ and $u'=-1$ on $(1,2)$**, almost everywhere. Both it and its derivative are bounded, so it belongs to every stated [Sobolev space](../../../../sobolev-space-split.md); its displayed [norm](../../../../norm.md) to the power $p$ is $2/(p+1)+2$.

For $u=x_1/r$ in the punctured ball, ordinary differentiation gives

$$
\boxed{D_ju=\delta_{1j}/r-x_1x_j/r^3.}
$$

The [function](../../../../function-split.md) is bounded and $|D_ju|\leq2/r$, so polar integration gives finite derivative $L^p$ [norms](../../../../norm.md) when $\int_0^1r^{n-1-p}dr<\infty$, namely $p<n$. To verify these are [weak derivatives](../../../../weak-derivative.md) across the origin, integrate by parts outside a ball of radius $\varepsilon$ against a compactly supported smooth test. The inner boundary term is at most a fixed constant times $\varepsilon^{n-1}$, since $u$ is bounded. It tends to zero for $n>1$. The volume terms converge by local integrability of the displayed derivative. Thus **$u\in W^{1,p}(B)$ for $1\leq p<n$ with exactly these derivatives**. Its value at the origin can be chosen arbitrarily.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../split.md)
5. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
