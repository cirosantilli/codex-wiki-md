<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the nonnegative-pairing [dual cone](../../../../../../dual-cone.md) $K^*=\{y:\langle y,s\rangle\geq0\text{ for all }s\in K\}$. The [Lagrangian](../../../../../../lagrangian.md) is $L(x,y)=c^Tx-y^T(Ax-b)$ for $y\in K^*$. Its infimum over unrestricted $x$ is finite exactly when $A^Ty=c$. Therefore the [conic dual problem](../../../../../../conic-dual-problem.md) is

$$
\boxed{\sup_y b^Ty\quad\text{subject to }A^Ty=c,\ y\in K^*=K.}
$$

The final equality uses the [self-dual cone](../../../../../../self-dual-cone.md) assumption.

For the canonical [self-concordant barrier](../../../../../../self-concordant-barrier.md), use its [logarithmically homogeneous barrier](../../../../../../logarithmically-homogeneous-barrier.md) normalization

$$
F(ts)=F(s)-\nu\log t,\qquad
\langle\nabla F(s),s\rangle=-\nu.
$$

At parameter $\mu>0$, the primal barrier problem is

$$
\min_{Ax-b\in\operatorname{int}K}\{c^Tx+\mu F(Ax-b)\}.
$$

Write $F_\dagger(y)=F^*(-y)$, the [Legendre dual cone barrier](../../../../../../legendre-dual-cone-barrier.md). The matching dual barrier problem is

$$
\min_{\substack{A^Ty=c\\y\in\operatorname{int}K}}\{-b^Ty+\mu F_\dagger(y)\}.
$$

Defining the dual barrier this way is valid generally; self-duality of the cone alone does not assert that an arbitrarily selected barrier equals its Legendre dual.

The joint [central path](../../../../../../central-path.md) characterization is

$$
\boxed{
Ax-b=s\in\operatorname{int}K,\quad
A^Ty=c,\quad y\in\operatorname{int}K,\quad
y=-\mu\nabla F(s).}
$$

The primal stationarity equation is $c+\mu A^T\nabla F(s)=0$, exactly the dual feasibility equation after defining $y$. For the dual relation, logarithmic homogeneity gives $\nabla F(s/\mu)=-y$, so $\nabla F_\dagger(y)=-s/\mu$. Thus dual stationarity is $-b+\mu\nabla F_\dagger(y)+Ax=0$, giving the same primal equation. At these points,

$$
\boxed{c^Tx-b^Ty=s^Ty=\nu\mu.}
$$

**Newton step.** At a chosen target parameter $\widehat\mu>0$, define

$$
r_p=Ax-b-s,\qquad r_d=A^Ty-c,\qquad
r_c=y+\widehat\mu\nabla F(s),\qquad H=\nabla^2F(s).
$$

Linearizing the three equality conditions gives the [central-path Newton system](../../../../../../central-path-newton-system.md)

$$
\boxed{\begin{aligned}
A\Delta x-\Delta s&=-r_p,\\
A^T\Delta y&=-r_d,\\
\Delta y+\widehat\mu H\Delta s&=-r_c.
\end{aligned}}
$$

Eliminating the slack and dual directions yields

$$
\boxed{\begin{aligned}
\widehat\mu A^THA\,\Delta x
&=r_d-A^Tr_c-\widehat\mu A^THr_p,\\
\Delta s&=A\Delta x+r_p,\\
\Delta y&=-r_c-\widehat\mu H\Delta s.
\end{aligned}}
$$

The barrier Hessian is positive definite. Full column rank of $A$ therefore makes $A^THA$ positive definite and the reduced solve unique. Use a damped step with $s+\alpha\Delta s$ and $y+\alpha\Delta y$ remaining interior; a full Newton step need not do so.

At an exact point with parameter $\mu$, choosing $\widehat\mu<\mu$ gives $r_p=r_d=0$ and $r_c=(\widehat\mu-\mu)\nabla F(s)$, the usual predictor towards the next path point. Infinitesimally,

$$
\frac{dx}{d\mu}
=-\frac1\mu(A^THA)^{-1}A^T\nabla F(s),\qquad
\frac{ds}{d\mu}=A\frac{dx}{d\mu},\qquad
\frac{dy}{d\mu}=-\nabla F(s)-\mu H\frac{ds}{d\mu}.
$$

The path definition presupposes interior feasibility and attainment of the barrier problems; strict primal-dual feasibility is a standard sufficient setting. The printed full-rank condition by itself is insufficient. For example $K=\mathbb R_+^2$, $A=(1,-1)^T$, $b=0$ and $c=0$ give the sole primal feasible point $x=0$, with no interior slack at all, despite full column rank. **Rank guarantees the Newton solve at an interior point, not existence of the central path.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
