<h1 id="b/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The endpoint $\alpha=0$ in the printed nonnegative-parameter hypothesis must be excluded. We first establish the intended result for $\alpha>0$, then describe that endpoint exactly.

Write $X,Y$ for the two directional matrices; they commute because they act on separate tensor-product coordinates. At a limit $V$, the intermediate vector also has a limit $\widetilde V$. Subtract the two limiting equations in the form that cancels $X\widetilde V$ and $YV$; this gives $2\alpha(\widetilde V-V)=0$. Hence $\widetilde V=V$ for $\alpha>0$. Substitution then gives $(X+Y)V=h^2f$, precisely the required discrete equation.

Eliminating the intermediate vector gives the [alternating direction implicit iteration](../../../../../alternating-direction-implicit-iteration.md) [matrix](../../../../../matrix.md)

$$
G=(\alpha I-Y)^{-1}(\alpha I+X)(\alpha I-X)^{-1}(\alpha I+Y).
$$

The [sine](../../../../../sine.md)-product basis simultaneously diagonalizes $X,Y$, with [eigenvalues](../../../../../eigenvalue.md) $-\xi_p$ and $-\eta_q$, where

$$
\xi_p=4\sin^2(p\pi h/2)>0,\qquad
\eta_q=4\sin^2(q\pi h/2)>0.
$$

Thus

$$
\boxed{\lambda_{pq}(G)=\frac{\alpha-\xi_p}{\alpha+\xi_p}\,
\frac{\alpha-\eta_q}{\alpha+\eta_q}.}
$$

For $\alpha>0$, each factor has modulus strictly less than one. Hence $\rho(G)<1$, proving convergence from every starting vector to the unique discrete solution.

At $\alpha=0$ the two factors are both $-1$, so $G=I$. The forcing terms cancel in the composed iteration as well, and **$V^{k+1}=V^k$ for every starting vector**. An incorrect initial vector therefore remains incorrect forever, even though the sequence is constant and has a limit. This disproves both the literal fixed-point implication and the claimed general convergence-to-solution assertion at zero; strict positivity of $\alpha$ is the necessary repair.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../../split.md)
6. [Numerical solution of differential equations course of the University of Oxford](../../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
