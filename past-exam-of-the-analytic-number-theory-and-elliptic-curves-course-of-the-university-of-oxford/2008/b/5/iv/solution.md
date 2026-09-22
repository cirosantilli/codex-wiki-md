<h1 id="b/5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Let $\alpha,\beta,\gamma$ be the nonzero reductions of $a,b,c$. The square set in $\mathbb F_p$ has $(p+1)/2$ members, including zero. Multiplication by $\alpha$, and separately the transformation $z\mapsto\gamma-\beta z$, preserve this cardinality. Hence the two sets in the hint have total cardinality $p+1>p$ and must intersect. This gives a solution $(x_0,y_0)$ modulo $p$.

The solution cannot have both coordinates zero since $\gamma\ne0$. If $x_0\ne0$, choose any integral lift of $y_0$ and apply [Hensel's lemma](../../../../../hensel-s-lemma.md) to the [polynomial](../../../../../polynomial-split.md) $aX^2+by_0^2-c$ in $X$: its [derivative](../../../../../derivative.md) at the reduced [root](../../../../../root-of-a-polynomial.md) is $2\alpha x_0\ne0$. If $y_0\ne0$, use the other variable instead. The nonzero [derivative](../../../../../derivative.md) uses $p\ne2$. Thus a solution lifts to $\boxed{x,y\in\mathbb Z_p}$ as required.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the analytic number theory and elliptic curves course of the University of Oxford](../../../../split.md)
6. [Analytic number theory and elliptic curves course of the University of Oxford](../../../../../analytic-number-theory-and-elliptic-curves-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
