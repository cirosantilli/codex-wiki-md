<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Using the radial-drift expression already derived, the factor $X-1$ cancels and gives

$$
\bar u_r=3A\sigma r\left[\frac52-(\frac52-2a)X\right].
$$

For $a=1$, $X=R/r$ and $\sigma=1/(15At)$, so

$$
\boxed{\bar u_r=\frac{5r-R}{10t}}.
$$

The instantaneous flow is inward for $r<R/5$ and outward for $R/5<r<R$. Nevertheless outward motion need not prevent eventual accretion. The trajectories in [accretion trajectories in a compact viscous similarity disk](../../../../../../accretion-trajectories-in-a-compact-viscous-similarity-disk.md) satisfy

$$
\frac{dr}{dt}-\frac{r}{2t}=-\frac C{10}t^{-3/5}.
$$

Multiplication by $t^{-1/2}$ and integration give

$$
\boxed{r(t)=Ct^{2/5}+K\sqrt t=R(t)+K\sqrt t}.
$$

A parcel at $r_i\in(0,R_i)$ at time $t_i>0$ has $K=(r_i-R_i)/\sqrt{t_i}<0$. It reaches the origin at

$$
\boxed{t_{\rm acc}=t_i\left(1-\frac{r_i}{R_i}\right)^{-10}<\infty}.
$$

Before arrival, $r/R=1+Kt^{1/10}/C$ decreases monotonically. Even a parcel initially moving outward eventually crosses $r/R=1/5$, turns inward, and is accreted. Only $K=0$, the outer-edge trajectory, never arrives; its [surface density of a disk](../../../../../../surface-density-of-a-disk.md) is zero. Thus almost every mass-carrying parcel is accreted in finite time.

For $a=5/4$, the coefficient $5/2-2a$ vanishes, leaving

$$
\boxed{\bar u_r=\frac{r}{2t}>0\quad(0<r<R)}.
$$

The trajectories are $r(t)=r_i\sqrt{t/t_i}$, so each parcel keeps a fixed ratio $r/R$. This is an expanding [nonaccreting similarity disk supplied by an inner torque](../../../../../../nonaccreting-similarity-disk-supplied-by-an-inner-torque.md), not an inward accretion solution.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
