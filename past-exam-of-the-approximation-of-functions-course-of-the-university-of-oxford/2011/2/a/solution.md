<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Take $n\geq1$, as intended by the stated normalization. The [Chebyshev polynomial](../../../../chebyshev-polynomial.md) recurrence $T_{r+1}=2xT_r-T_{r-1}$, with $T_0=1$ and $T_1=x$, shows by [mathematical induction](../../../../mathematical-induction.md) that $T_n$ has [polynomial degree](../../../../degree-of-a-polynomial.md) $n$ and leading coefficient $2^{n-1}$. Consequently $f_n=2^{1-n}T_n$ is a [monic polynomial](../../../../monic-polynomial.md). At the ordered [Chebyshev extreme points](../../../../chebyshev-lobatto-node.md) $t_j=-\cos(j\pi/n)$,

$$
f_n(t_j)=2^{1-n}(-1)^{n+j},\qquad0\leq j\leq n,
$$

and $\|f_n\|_\infty=2^{1-n}$.

Suppose a [monic polynomial](../../../../monic-polynomial.md) $q$ of the same [polynomial degree](../../../../degree-of-a-polynomial.md) had $\|q\|_\infty<2^{1-n}$. The difference $f_n-q$ has degree at most $n-1$ because its leading coefficients cancel. Its signs at the $n+1$ ordered extreme points strictly alternate. The [intermediate value theorem](../../../../intermediate-value-theorem.md) supplies a distinct [root of a polynomial](../../../../root-of-a-polynomial.md) between each consecutive pair, giving at least $n$ roots. This contradicts its degree bound. Hence the [monic Chebyshev extremal polynomial](../../../../monic-chebyshev-extremal-polynomial.md) satisfies

$$
\boxed{\|f_n\|_\infty=2^{1-n}\leq\|q\|_\infty.}
$$

At $n=0$ the printed formula instead gives $f_0=2$, which is not monic; the degree-zero minimizer is the constant one. This endpoint case requires the separate normalization $f_0=1$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the approximation of functions course of the University of Oxford](../../../split.md)
5. [Approximation of functions course of the University of Oxford](../../../../approximation-of-functions-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
