<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Lipschitz constant](../../../../../../lipschitz-constant.md) convention $\|f\|_L=\sup_{x\ne y}|f(x)-f(y)|/d(x,y)$ in the final quantity; it is a seminorm, with constants having value zero. Also interpret the [coupling](../../../../../../coupling.md) space as $\mathcal P(X\times X)$. The printed $\mathcal P(X,Y)$ has an undefined $Y$. The third quantity has a duplicated printed label; it is placed in part iii here, with the fourth in part iv.

First prove weak [optimal transport](../../../../../../optimal-transport.md) duality. For any feasible continuous pair $f,g$ and any [coupling of probability distributions](../../../../../../coupling.md) $\pi$ with marginals $P,Q$,

$$
\int f\,dP+\int g\,dQ
=\int_{X\times X}(f(x)+g(y))\,d\pi(x,y)
\leq\int_{X\times X}d(x,y)\,d\pi(x,y).
$$

Taking the supremum over pairs and infimum over [couplings](../../../../../../coupling.md) gives **$m_d(P,Q)\leq W(P,Q)$**. These quantities are finite: $P\otimes Q$ is a [coupling](../../../../../../coupling.md) and the continuous cost $d$ is bounded on the [compact metric space](../../../../../../compact-metric-space.md) $X\times X$. The zero pair is feasible, so $0\leq m_d\leq W\leq\operatorname{diam}X$.

The reverse inequality is established in part ii by finite approximation and a proof of the required finite [linear programming duality](../../../../../../linear-programming-duality.md). Parts iii and iv then show that all the dual formulations agree.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
