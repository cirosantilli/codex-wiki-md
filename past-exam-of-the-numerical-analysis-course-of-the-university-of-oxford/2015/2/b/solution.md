<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume $f\in C^{n+1}[a,b]$ and set $\omega(t)=\prod_{i=0}^n(t-x_i)$, a [monic polynomial](../../../../monic-polynomial.md) of [polynomial degree](../../../../degree-of-a-polynomial.md) $n+1$. Fix $x\in[a,b]$ distinct from all the [interpolation nodes](../../../../interpolation-node.md), and choose

$$
C=\frac{f(x)-p_n(x)}{\omega(x)}.
$$

The auxiliary [function](../../../../function-split.md)

$$
F(t)=f(t)-p_n(t)-C\omega(t)
$$

vanishes at the $n+2$ distinct points $x_0,\ldots,x_n,x$. Order those points and repeatedly apply [Rolle's theorem](../../../../rolle-theorem.md). After $n+1$ applications, there is some $\xi$ strictly between their smallest and largest values, hence in $(a,b)$, such that $F^{(n+1)}(\xi)=0$.

Because $p_n$ has [polynomial degree](../../../../degree-of-a-polynomial.md) at most $n$ and $\omega$ is monic of [polynomial degree](../../../../degree-of-a-polynomial.md) $n+1$,

$$
0=f^{(n+1)}(\xi)-C(n+1)!.
$$

Substituting the resulting value of $C$ proves the [polynomial interpolation error](../../../../polynomial-interpolation-error.md) formula

$$
\boxed{f(x)-p_n(x)=\frac{f^{(n+1)}(\xi)}{(n+1)!}\prod_{i=0}^n(x-x_i).}
$$

At an [interpolation node](../../../../interpolation-node.md), both sides are zero, so any $\xi\in(a,b)$ works. Such an interior point exists because $n\geq1$ and the [interpolation nodes](../../../../interpolation-node.md) are distinct. The selected $\xi$ generally depends on $x$; the theorem makes an existence assertion, not a regularity assertion about that dependence.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
