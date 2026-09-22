<h1 id="15/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $p=y'$ and differentiate the general form of [Clairaut's equation](../../../../../clairaut-s-equation.md):

$$
p=p+xp'+f'(p)p'.
$$

Cancellation gives

$$
\boxed{[x+f'(p)]\frac{dp}{dx}=0}.
$$

For $f(p)=1/(p-1)$ the equation is defined only when $p\ne1$. There are two types of smooth branch.

First, constant $p=C\ne1$ gives the straight-line family

$$
\boxed{y=Cx+\frac1{C-1},\qquad C\in\mathbb R\setminus\{1\}}.
$$

Second, $x+f'(p)=0$ gives $x=1/(p-1)^2$, so $x>0$ and $p=1\pm x^{-1/2}$. Substituting in the original equation gives its two singular [envelope](../../../../../envelope-mathematics.md) branches,

$$
\boxed{y=x\pm2\sqrt x\qquad(x>0)}.
$$

Their [derivatives](../../../../../derivative.md) are indeed $1\pm1/\sqrt x$, verifying the required value of $p$. There is no finite-slope continuation of either [envelope](../../../../../envelope-mathematics.md) through $x=0$, and no real [envelope](../../../../../envelope-mathematics.md) branch for $x<0$.

For completeness, if “solution” requires only a [continuous](../../../../../continuous-function.md) first [derivative](../../../../../derivative.md), one can join a line from the family to the corresponding [envelope](../../../../../envelope-mathematics.md) at their tangency point $x=(C-1)^{-2}$. The [function](../../../../../function-split.md) and its first [derivative](../../../../../derivative.md) match there, so such piecewise branches also solve the original first-order equation. They are not twice continuously [differentiable](../../../../../differentiable-function.md) at a nontrivial join. The lines and [envelope](../../../../../envelope-mathematics.md) branches above exhaust the smooth branches; allowing these tangent joins supplies the additional $C^1$ solutions.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [15](../../15.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
