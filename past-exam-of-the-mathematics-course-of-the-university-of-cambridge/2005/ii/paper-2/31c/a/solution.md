<h1 id="31c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a localized traveling wave put $q(x,t)=Q(\xi)$ with $\xi=x-ct-x_0$, and require $Q,Q',Q''\to0$ at infinity. The modified KdV equation integrates once to $Q''-cQ+2Q^3=0$. Multiplying by $Q'$ and integrating again gives

$$
(Q')^2=cQ^2-Q^4.
$$

A nonzero decaying real solution requires $c>0$. Separating on the rising or falling half of the wave and using the indicated inverse-hyperbolic-secant integral yields

$$
\boxed{q(x,t)=\pm\sqrt c\,\operatorname{sech}\big[\sqrt c(x-ct-x_0)\big],\qquad c>0.}
$$

The signs and translations are arbitrary. Differentiating the sech profile verifies $Q''=cQ-2Q^3$ directly. The relevant antiderivative is the inverse hyperbolic secant, since $d(\operatorname{arcsech}x)/dx=-1/[x\sqrt{1-x^2}]$ for $0<x<1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [31C](../../31c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
