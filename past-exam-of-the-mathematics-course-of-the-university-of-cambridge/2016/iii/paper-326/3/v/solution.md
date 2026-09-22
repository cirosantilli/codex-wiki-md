<h1 id="3/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Take $F=(F^*)^*$ with the usual proper closed convex assumptions, so the [Fenchel-Moreau theorem](../../../../../../fenchel-moreau-theorem.md) identifies its conjugate with the supplied $F^*$. Put $z^k=u^k-\tau D^Tv^k$. The first update is $w^{k+1}=\operatorname{prox}_{F^*/\tau}(z^k/\tau)$. By [Moreau decomposition](../../../../../../moreau-decomposition.md), the second update is

$$
u^{k+1}=z^k-\tau\operatorname{prox}_{F^*/\tau}(z^k/\tau)=\operatorname{prox}_{\tau F}(z^k).
$$

Also $\tau(D^Tv^k+w^{k+1})=u^k-u^{k+1}$, so the argument in the final update contains $u^{k+1}-\tau(D^Tv^k+w^{k+1})=2u^{k+1}-u^k$. Eliminating the auxiliary variable gives

$$
\boxed{\begin{aligned}
u^{k+1}&=\operatorname{prox}_{\tau F}(u^k-\tau D^Tv^k),\\
v^{k+1}&=\operatorname{prox}_{\sigma G}\left(v^k+\sigma D(2u^{k+1}-u^k)\right).
\end{aligned}}
$$

This is the [primal-dual hybrid gradient method](../../../../../../chambolle-pock-algorithm.md) with extrapolation parameter one and the primal update performed first. Its [saddle point](../../../../../../saddle-point.md) function is $F(u)+\langle Du,v\rangle-G(v)$, corresponding to the primal objective $F(u)+G^*(Du)$.

For proper [lower semicontinuous](../../../../../../lower-semicontinuity.md) [convex functions](../../../../../../convex-function.md) and a nonempty saddle-point set in these finite-dimensional spaces, the standard [convergence of primal-dual hybrid gradient](../../../../../../convergence-of-primal-dual-hybrid-gradient.md) theorem gives the sufficient parameter condition

$$
\boxed{\tau>0,\qquad\sigma>0,\qquad\tau\sigma\|D\|_2^2<1.}
$$

Here $\|D\|_2$ is the [operator norm](../../../../../../operator-norm.md), or largest [singular value](../../../../../../singular-value.md). For $D\ne0$, one possible choice is $\tau=\sigma=\eta/\|D\|_2$ with $0<\eta<1$; for $D=0$ any positive steps satisfy the condition. The existence assumption is necessary: step sizes alone cannot guarantee convergence to a saddle point that does not exist.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
