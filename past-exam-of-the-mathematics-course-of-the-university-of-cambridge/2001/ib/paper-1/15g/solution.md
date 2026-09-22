<h1 id="15g/solution">Solution</h1>

↑ **Parent:** [15G](../15g.md)

Put $\theta=x-t$. Taking the [gradient](../../../../../gradient.md) of the [velocity potential](../../../../../velocity-potential.md) gives

$$
\boxed{\boldsymbol u=(-\epsilon y\sin\theta,\ \epsilon\cos\theta)},\qquad
\boxed{\nabla\cdot\boldsymbol u=-\epsilon y\cos\theta}.
$$

The motion is not generally incompressible; a [velocity potential](../../../../../velocity-potential.md) ensures irrotationality, not zero [divergence](../../../../../divergence.md). Both components have zero time average at each fixed point because their sine and cosine averages vanish.

The fluid acceleration is the [material derivative](../../../../../material-derivative.md) $D\boldsymbol u/Dt=\partial_t\boldsymbol u+(\boldsymbol u\cdot\nabla)\boldsymbol u$. Direct differentiation gives

$$
a_x=\epsilon y\cos\theta+\epsilon^2(y^2-1)\sin\theta\cos\theta,
\qquad
a_y=\epsilon\sin\theta+\epsilon^2y\sin^2\theta.
$$

Averaging over one period at fixed $(x,y)$ therefore yields

$$
\boxed{\overline{\boldsymbol a}=(0,\epsilon^2y/2)}.
$$

This need not be the [derivative](../../../../../derivative.md) of the mean velocity: the nonlinear advective term remains after averaging.

The dyed particle obeys the [Lagrangian trajectory](../../../../../lagrangian-trajectory.md) equations

$$
\dot x=-\epsilon y\sin(x-t),\qquad \dot y=\epsilon\cos(x-t),\qquad x(0)=y(0)=0.
$$

Expand $x=\epsilon x_1+\epsilon^2x_2+O(\epsilon^3)$ and $y=\epsilon y_1+\epsilon^2y_2+O(\epsilon^3)$, for bounded times. The first-order equations give $x_1=0$, $\dot y_1=\cos t$, so $y_1=\sin t$. At second order,

$$
\dot x_2=\sin^2t,\qquad \dot y_2=0.
$$

Integrating with zero initial values verifies

$$
\boxed{x(t)=\epsilon^2\left(\frac t2-\frac{\sin2t}{4}\right)+O(\epsilon^3),\qquad y(t)=\epsilon\sin t+O(\epsilon^3)}.
$$

The velocity averaged along this particle over $0\leq t\leq2\pi$ is its displacement divided by $2\pi$. Hence

$$
\boxed{\overline{\boldsymbol u}_{\mathrm{particle}}=(\epsilon^2/2,0)+O(\epsilon^3)}.
$$

This [Stokes drift](../../../../../stokes-drift.md) is a Lagrangian mean; it does not contradict the zero [Eulerian mean velocity](../../../../../eulerian-mean-flow.md) at a fixed point. The secular term is a small-parameter expansion, not an assertion of uniform accuracy as $t\to\infty$.

## ↑ Ancestors (10)

1. [15G](../15g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
