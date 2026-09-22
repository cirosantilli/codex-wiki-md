<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Introduce the primal slack $s=Ax-b\in K$. The [Lagrangian](../../../../../../lagrangian.md) is $L(x,y)=c^\top x-\langle y,Ax-b\rangle$, with $y\in K^*=K$. Minimizing over $x$ is finite only when $A^\top y=c$. Thus the [conic dual problem](../../../../../../conic-dual-problem.md) is

$$
\boxed{\sup_y b^\top y\quad\text{subject to }A^\top y=c,\quad y\in K.}
$$

The primal-dual gap at feasible points is $c^\top x-b^\top y=\langle s,y\rangle\geq0$. Self-duality specifies the multiplier cone; it does not alone guarantee feasible or bounded problems. The central-path discussion assumes primal and dual strict feasibility and a finite optimum. These additional existence conditions are not implied by the given full column rank of $A$.

Let $F$ be the canonical logarithmically homogeneous [self-concordant barrier](../../../../../../self-concordant-barrier.md), with parameter $\nu$ and $F(ts)=F(s)-\nu\log t$. For each $\mu>0$, minimizing $c^\top x+\mu F(Ax-b)$ defines the primal [central path](../../../../../../central-path.md). Its stationarity defines the dual path through $y=-\mu\nabla F(s)\in\operatorname{int}K$. The joint characterization is

$$
\boxed{s=Ax-b\in\operatorname{int}K,\quad A^\top y=c,\quad
 y\in\operatorname{int}K,\quad y+\mu\nabla F(s)=0.}
$$

Euler's identity for logarithmic homogeneity gives $\langle s,\nabla F(s)\rangle=-\nu$, so $\boxed{\langle s,y\rangle=\nu\mu}$. The gap tends to zero as $\mu\downarrow0$. If $F_*(y)=\sup_{s\in\operatorname{int}K}[-\langle y,s\rangle-F(s)]$ is the dual barrier, the equivalent dual relation is $s=-\mu\nabla F_*(y)$. A self-dual cone does not justify identifying two arbitrary primal and dual barrier functions without this relation.

For a target parameter $\bar\mu>0$, form residuals $r_p=Ax-b-s$, $r_d=A^\top y-c$ and $r_c=y+\bar\mu\nabla F(s)$. Linearization gives the [central-path Newton system](../../../../../../central-path-newton-system.md)

$$
\boxed{A\Delta x-\Delta s=-r_p,\qquad A^\top\Delta y=-r_d,\qquad
\Delta y+\bar\mu\nabla^2F(s)\Delta s=-r_c.}
$$

For a strictly feasible primal-dual iterate with $r_p=r_d=0$, elimination reduces it to

$$
\bar\mu A^\top\nabla^2F(s)A\Delta x=-A^\top r_c,\quad
\Delta s=A\Delta x,\quad
\Delta y=-r_c-\bar\mu\nabla^2F(s)\Delta s.
$$

The barrier Hessian is positive definite and $A$ has full column rank, so the reduced matrix is positive definite. Alternatively a changing path parameter can be included as an additional linear term $\Delta\mu\nabla F(s)$; the displayed system instead fixes the new target parameter before solving.

This is an [interior-point method](../../../../../../interior-point-method.md) because iterates stay in the cone interiors where the barrier and its gradient/Hessian are defined. A full Newton step need not do so. Use a fraction-to-boundary or backtracking step: decrease $\alpha>0$ until $s+\alpha\Delta s$ and $y+\alpha\Delta y$ lie in $\operatorname{int}K$, then enforce an appropriate barrier or residual decrease. Such a positive step exists because the current points are interior. Local barrier norms can also certify an interior step via the [Dikin ellipsoid](../../../../../../dikin-ellipsoid.md).

For a practical starting point, choose $e\in\operatorname{int}K$ and solve a [conic phase-I problem](../../../../../../conic-phase-i-problem.md), for example minimizing $t$ subject to $Ax-b+te\in K$ and $t\geq-1$. A large positive $t$ with an arbitrary $x$ gives a strictly feasible start for this auxiliary problem. A feasible point with $t<0$ certifies $Ax-b\in\operatorname{int}K$. If the original problem is strictly feasible, a small negative $t$ is feasible, so phase I can find such a certificate. A similar feasibility procedure handles the dual equality and interior. Alternatively an infeasible-start primal-dual method or homogeneous self-dual embedding starts with interior cone variables while allowing nonzero linear residuals, and can report infeasibility rather than presume an interior solution exists.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
