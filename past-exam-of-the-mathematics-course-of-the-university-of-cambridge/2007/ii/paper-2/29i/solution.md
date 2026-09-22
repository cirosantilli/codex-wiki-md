<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

For fixed terminal time and fixed endpoint, use the maximizing form of the [Pontryagin maximum principle](../../../../../pontryagin-maximum-principle.md). For dynamics $\dot q=f(q,u,t)$ and running cost $L$, there are multipliers $(p,p_0)$, not all zero, with $p_0\ge0$, and [Hamiltonian of an optimal-control problem](../../../../../hamiltonian-of-an-optimal-control-problem.md) $\mathscr H=p\cdot f-p_0L$. Along an optimum, $\dot q=\mathscr H_p$, $\dot p=-\mathscr H_q$, and the chosen control maximizes $\mathscr H$ over admissible controls almost everywhere. Fixed terminal state imposes no prescribed terminal value of $p$; fixed time imposes no free-time condition $\mathscr H(T)=0$. The normal case scales $p_0=1$; abnormal extremals have $p_0=0$.

For this problem the normal [Hamiltonian of an optimal-control problem](../../../../../hamiltonian-of-an-optimal-control-problem.md) is

$$
\mathscr H=p_xu+p_yv+k(uy-vx)-\frac12(u^2+v^2),\qquad \dot k=0.
$$

Maximization gives $u=p_x+ky$, $v=p_y-kx$. The [costate](../../../../../costate.md) equations give $\dot p_x=kv$, $\dot p_y=-ku$, hence $\dot u=2kv$, $\dot v=-2ku$. Nonzero velocities rotate at constant angular rate, and rotational symmetry permits $u(0)=A$, $v(0)=0$. For a closed path, $2k=2\pi n$, with integer $n\ne0$. Then $z(1)=A^2/(2\pi n)$, so the required positive endpoint has $n>0$, $A^2=2\pi n$ and cost $\pi n$.

To prove a global minimum rather than only classify stationary extremals, write $r=(x,y)$ and subtract its time average; this changes neither its derivative nor $\int(y\dot x-x\dot y)dt$. The resulting closed mean-zero path satisfies the periodic [Wirtinger inequality](../../../../../wirtinger-inequality.md) $\int|r|^2\le(4\pi^2)^{-1}\int|\dot r|^2$. This follows immediately by its Fourier expansion: each nonzero mode of the derivative has squared multiplier at least $4\pi^2$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) now gives

$$
1=|z(1)|\le\left(\int|r|^2\right)^{1/2}\left(\int|\dot r|^2\right)^{1/2}
\le\frac1{2\pi}\int_0^1(u^2+v^2)dt.
$$

The argument extends to square-integrable controls by the periodic Sobolev/Fourier interpretation. Thus the cost is at least $\pi$ for every feasible control. Equality is attained by

$$
\boxed{u=\sqrt{2\pi}\cos(2\pi t),\quad v=-\sqrt{2\pi}\sin(2\pi t),\quad
x=\frac{\sin(2\pi t)}{\sqrt{2\pi}},\quad y=\frac{\cos(2\pi t)-1}{\sqrt{2\pi}},\quad
z=t-\frac{\sin(2\pi t)}{2\pi}.}
$$

These satisfy every endpoint and have cost $\pi$. Therefore **the minimum is $\pi$**, an [area-constrained quadratic control cost](../../../../../area-constrained-quadratic-control-cost.md). The global inequality also prevents an overlooked abnormal candidate from lowering it; in fact an abnormal finite maximizing [Hamiltonian of an optimal-control problem](../../../../../hamiltonian-of-an-optimal-control-problem.md) would force both linear control coefficients to vanish and then force zero velocity, incompatible with $z(1)=1$.

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
