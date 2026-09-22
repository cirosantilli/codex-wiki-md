<h1 id="a/1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $n\geq1$, set $p=2^{1-n}T_n$. It is monic by part (a), and its supremum [norm](../../../../../norm.md) on $[-1,1]$ is $E=2^{1-n}$. At the $n+1$ successive extreme points $x_j=\cos(j\pi/n)$ it alternates between $E$ and $-E$.

Suppose a monic degree-$n$ [polynomial](../../../../../polynomial-split.md) $q$ had $\|q\|_\infty<E$. At each $x_j$, the difference $p-q$ would have the sign of $p$. These signs alternate, so the [intermediate value theorem](../../../../../intermediate-value-theorem.md) forces a root in each of the $n$ successive gaps. But the leading monic terms cancel, making $\deg(p-q)\leq n-1$, a contradiction. Therefore

$$
\boxed{\|2^{1-n}T_n\|_\infty\leq\|q\|_\infty.}
$$

This is the monic [monic Chebyshev extremal polynomial](../../../../../monic-chebyshev-extremal-polynomial.md). The positive-degree restriction matters: at $n=0$ the printed scaling gives the constant two, while the only monic constant is one, so that version is false. The customary theorem uses $n\geq1$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [1](../../1.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
