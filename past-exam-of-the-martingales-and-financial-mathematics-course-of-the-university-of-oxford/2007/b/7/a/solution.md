<h1 id="b/7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the usual nondegenerate positive-rate case $r>0$, $\sigma>0$, $K>0$. Define the [Black-Scholes equation](../../../../../black-scholes-equation.md)

$$
\mathcal LV=V_t+\tfrac12\sigma^2S^2V_{SS}+rSV_S-rV,
\qquad g(S)=(K-S)_+.
$$

The American value dominates immediate exercise. Its discounted value is a [supermartingale](../../../../../supermartingale.md) under the [risk-neutral measure](../../../../../risk-neutral-measure.md), so $\mathcal LV\leq0$, with equality where it is optimal to continue. The [obstacle problem](../../../../../obstacle-problem.md) is

$$
\boxed{V\geq g,\quad\mathcal LV\leq0,\quad
(V-g)\mathcal LV=0,\quad V(T,S)=g(S).}
$$

Equivalently $\max(\mathcal LV,g-V)=0$.

For the put, write the exercise boundary as $S=b(t)$. On $S>b(t)$ solve $\mathcal LV=0$; on $0<S\leq b(t)$ set $V=K-S$. Value matching and [smooth pasting](../../../../../smooth-pasting.md) require

$$
\boxed{V(t,b(t))=K-b(t),\qquad V_S(t,b(t))=-1.}
$$

The remaining conditions are $V(t,0)=K$, $V(t,S)\to0$ as $S\to\infty$, and the terminal [contingent claim payoff](../../../../../contingent-claim-payoff.md), with $b(T-)=K$ in this positive-rate setting. The boundary is an unknown to be found with the price, which is what makes this a [free boundary problem](../../../../../free-boundary-problem.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [7](../../7.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
