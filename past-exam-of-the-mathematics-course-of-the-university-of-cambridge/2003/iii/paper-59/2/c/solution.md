<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

To determine the nonlinear [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md), solve the four slaved steady equations exactly. Set

$$
k=\frac{h}{(4-h)\sigma^2}=\frac{\pi^2}{\alpha^2\sigma^2},\qquad u=a^2.
$$

The nonzero [equilibrium points](../../../../../../equilibrium-point-of-a-dynamical-system.md) satisfy

$$
b=\frac{a}{1+u},\quad c=\frac{u}{1+u},\quad d=\frac{a}{\sigma(1+ku)},\quad e=\frac{ku}{1+ku},\qquad
r=(1+u)\left(1+\frac{q}{1+ku}\right).
$$

Thus

$$
r-(1+q)=[1-q(k-1)]u+qk(k-1)u^2+O(u^3).
$$

If $k\le1$, the coefficient of $u$ is positive for every physical $q\ge0$: there is **no change of pitchfork direction at a nonnegative rotation parameter**. If $k>1$, the change occurs at

$$
\boxed{q_D=r_\Omega^2=\frac1{k-1}=\frac{(4-h)\sigma^2}{h-(4-h)\sigma^2},\qquad r_D=1+q_D.}
$$

Below $q_D$ the nonzero branch lies on $r>r_P$; above $q_D$ it initially lies on $r<r_P$. At $q_D$, $r-r_D=ku^2+O(u^3)$, so $|a|$ grows like $(r-r_D)^{1/4}$ rather than the ordinary square-root scaling.

The [rational equilibrium curve at a degenerate pitchfork](../../../../../../rational-equilibrium-curve-at-a-degenerate-pitchfork.md) also gives the nearby [saddle-node bifurcations](../../../../../../saddle-node-bifurcation.md) of the two reflection-related nonzero branches. For $q>q_D$,

$$
\boxed{u_{SN}=\frac{\sqrt{q(k-1)}-1}{k},\qquad
r_{SN}=\frac{k-1+q+2\sqrt{q(k-1)}}{k},}
$$

and

$$
r_P-r_{SN}=\frac{(\sqrt{q(k-1)}-1)^2}{k}.
$$

The two [saddle-node bifurcations](../../../../../../saddle-node-bifurcation.md) occur on one parameter curve by reflection symmetry; its separation from the [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) curve is quadratic in $q-q_D$.

The stability statement needs a further condition. At $r_P$, the other coupled [eigenvalues](../../../../../../eigenvalue.md) have polynomial $s^2+(1+2\sigma)s+\sigma[(1+\sigma)-(1-\sigma)q]$. They are stable only for $q<q_{TB}$. If $q_D<q_{TB}$, a one-dimensional [centre manifold](../../../../../../center-manifold.md) gives the local form $a'=\chi a[\Delta-[1-q(k-1)]a^2-ka^4+\cdots]$, where $\Delta=r-r_P$ and $\chi=\sigma/[(1+\sigma)-(1-\sigma)q_D]>0$. The quintic term stabilizes the large branch. The interval $r_{SN}<r<r_P$ then has a stable conductive state and two stable finite-amplitude states, with the two small unstable branches separating their [basins of attraction](../../../../../../basin-of-attraction.md). This is the usual subcritical convection [hysteresis](../../../../../../hysteresis.md). If $q_D>q_{TB}$, the branch still reverses its direction, but the trivial state already has an additional unstable mode; this equilibrium-curve calculation alone does not imply a stable bistable wedge. At equality a two-dimensional [centre manifold](../../../../../../center-manifold.md) is essential.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 59](../../../paper-59-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
