<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the [plane quartic with exactly two nodes](../../../../../../plane-quartic-with-exactly-two-nodes.md)

$$
\boxed{C=V_+\bigl((X^2-Z^2)^2+XZY^2+Y^4\bigr)\subseteq\mathbb P^2_{\mathbb C}.}
$$

Put $d=X^2-Z^2$. Its partial [derivatives](../../../../../../derivative.md) are

$$
F_X=4Xd+ZY^2,\qquad F_Z=-4Zd+XY^2,\qquad F_Y=2XYZ+4Y^3.
$$

On $Y=0$, the equation gives $X^2=Z^2$, producing exactly $P_+=[1:0:1]$ and $P_-=[-1:0:1]$, and their gradients vanish.

There are no singular points with $Y\ne0$. Normalize $Y=1$. The derivative equations give $X=4dZ$ and $(16d^2+1)Z=0$. If $Z=0$, then $X=0$ and $F_Y=4\ne0$, so $Z\ne0$ and $d^2=-1/16$. The remaining equation gives $XZ=-2$, hence $Z^2=-1/(2d)$. But $d=X^2-Z^2=-2Z^2=1/d$, forcing $d^2=1$, a contradiction. Thus **the singular set is exactly $\{P_+,P_-\}$**.

In the chart $Z=1$ near $P_\varepsilon$, put $X=\varepsilon+u$, $Y=v$ with $\varepsilon=\pm1$. The lowest-degree part is $4u^2+\varepsilon v^2$, which splits into two distinct complex linear factors. Each singularity is therefore an [ordinary double point](../../../../../../ordinary-double-point.md), with two smooth transverse branches.

It remains to prove irreducibility. A repeated polynomial factor would make every point on that component singular, contradicting the finite singular set, so $F$ is reduced. If it were reducible, partition its irreducible factors into two coprime factors of degrees $r$ and $4-r$, $1\le r\le3$. Every intersection of the two components would be singular on $C$, hence one of the two [ordinary double points](../../../../../../ordinary-double-point.md). At an [ordinary double point](../../../../../../ordinary-double-point.md) shared by them, the two branches are transverse, so its intersection multiplicity is one. Their total intersection multiplicity would therefore be at most two. The [Bézout theorem](../../../../../../bezout-s-theorem.md) instead makes it $r(4-r)\ge3$. This contradiction proves **the displayed quartic is irreducible and has exactly two singular points**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
