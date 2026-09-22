<h1 id="a/2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $x=1-t$. For $0<k\leq1$,

$$
(1-t)^k=1-kt+\frac{k(k-1)}2t^2+O(t^3),
$$

whereas the constrained [rational interpolant](../../../../../rational-interpolant.md) expands as

$$
\frac{a(1-t)}{1+b-bt}
=\frac a{1+b}\left[1-\frac{t}{1+b}+O(t^2)\right].
$$

Matching the constant term gives $a=1+b$, and matching the coefficient of $t$ gives $1/(1+b)=k$. Thus $a=1/k$, $b=(1-k)/k$, and

$$
\boxed{r(x)=\frac{x}{k+(1-k)x}.}
$$

This is an [endpoint-constrained rational approximation to a power](../../../../../endpoint-constrained-rational-approximation-to-a-power.md): it matches value and derivative at $x=1$ and also enforces $r(0)=0$ for $k>0$.

There is a terminology qualification. A standard degree-$(1,1)$ [Padé approximant](../../../../../pade-approximant.md) about $t=0$ matches through $t^2$, but the displayed constrained expression has quadratic coefficient $-k(1-k)$ rather than $-k(1-k)/2$. The unconstrained Padé approximant is instead

$$
R(x)=\frac{(1-k)+(1+k)x}{(1+k)+(1-k)x}.
$$

The source's requested formula is obtained by the two stated endpoint matching conditions within its restricted family, rather than by full Padé matching. At $k=1$ both reduce to $x$. At $k=0$, the requested expression is one for $x>0$ with a removable value at zero; finite $a,b$ in the original restricted form do not represent that constant function. The endpoint is understood by this limit.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
