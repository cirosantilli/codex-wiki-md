<h1 id="29i/solution">Solution</h1>

↑ **Parent:** [29I](../29i.md)

Use the maximizing form of the [Pontryagin maximum principle](../../../../../pontryagin-maximum-principle.md). For a cost-minimization problem there are a nonnegative multiplier $\lambda_0$ and a costate $\psi$, not both identically zero, with [Hamiltonian](../../../../../hamiltonian.md) $\mathscr H=\psi b-\lambda_0c$. The optimal control maximizes $\mathscr H$, the costate obeys $\dot\psi=-\mathscr H_x$, and free terminal time at the fixed terminal state zero gives $\mathscr H(\tau)=\lambda_0C'(\tau)$. There is no fixed terminal costate value since the terminal state is fixed. In the normal case scale $\lambda_0=1$.

For the energy problem $b=-u$, $c=up(t)$, $C=-R$, so $\psi$ is constant and the normal [Hamiltonian](../../../../../hamiltonian.md) is $u(p_*-p(t))$, where $p_*=-\psi$. Maximization gives full power for $p(t)<p_*$ and zero power for $p(t)>p_*$; either value, or a fractional value, is allowed on a price tie. On the final active arc, the free-time condition gives

$$
\boxed{p_*+R'(\tau_*)=p(\tau_*).}
$$

This is the [threshold energy scheduling with a completion reward](../../../../../threshold-energy-scheduling-with-a-completion-reward.md) rule. In this example the normal case is justified: an abnormal constant costate would require either no processing or processing at all times, and free-time transversality would then force that nonzero costate to vanish.

For $p_*=1/4$, processing starts at $t=1/2$. Energy $1/2$ is completed at $\tau=1$, before the price rises again. Its cost and reward are

$$
\boxed{\int_{1/2}^{1}(t-1)^2dt=1/24,\qquad R(1)=1/2,\qquad J=-11/24.}
$$

Any threshold carrying completion into day two has $\tau\geq2$ and reward at most $1/3$. Since energy cost is nonnegative, $J\geq-1/3>-11/24$, so it is suboptimal.

For a global check, even any completion time $\tau\geq5/4$ has reward at most $4/9<11/24$ and cannot beat the displayed candidate. Also $\tau\geq1/2$ since power is bounded by one. At a fixed $\tau\in[1/2,5/4]$, the cheapest half-unit of processing consists of the last half-unit interval $[\tau-1/2,\tau]$: every earlier point has a price at least as large as every selected point. Exchanging any earlier powered interval with a later unpowered cheaper one proves this rearrangement claim, also for fractional controls.

Write $h=3/2-\tau\in[1/4,1]$. This minimal cost minus reward is

$$
J(h)=h^2/2-h/4+1/24-\frac1{5/2-h},
$$

with

$$
J'(h)=h-1/4-\frac1{(5/2-h)^2},\qquad
J''(h)=1-\frac2{(5/2-h)^3}>0.
$$

It has its unique minimum at $h=1/2$, where $J'=0$. The selected interval is then $[1/2,1]$ and its threshold is $h^2$. Consequently

$$
\boxed{p_*=1/4\text{ is globally optimal}.}
$$

The terminal condition also checks: $1/4+R'(1)=1/4-1/4=p(1)=0$.

## ↑ Ancestors (10)

1. [29I](../29i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
