<h1 id="15e/solution">Solution</h1>

↑ **Parent:** [15E](../15e.md)

Put $\pi=p-eA/c=m\dot q$. The [Hamilton equations](../../../../../hamilton-s-equations.md) are

$$
\dot q_i=\frac1m\left(p_i-\frac ecA_i\right),\qquad
\dot p_i=\frac e{mc}\sum_j\pi_j\partial_iA_j.
$$

Differentiate the [mechanical momentum](../../../../../mechanical-momentum.md) and substitute:

$$
m\ddot q_i=\frac ec\sum_j\dot q_j(\partial_iA_j-\partial_jA_i)-\frac ec\partial_tA_i.
$$

With $B=\nabla\times A$ and $E=-c^{-1}\partial_tA$ in this zero-scalar-potential gauge, this is $\boxed{m\ddot q=eE+(e/c)\dot q\times B}$, the [Lorentz force](../../../../../lorentz-force.md) in the units of the [Hamiltonian](../../../../../hamiltonian.md).

For $A=(-yB_0(z,t),0,0)$, $x$ is cyclic, so $p_x$ is conserved. Choose $p_x=0$, giving $\dot x=\Omega y$, where $\Omega=eB_0/(mc)$. Since $p_y=m\dot y$, its Hamilton equation gives $\dot p_y=-(e/c)B_0\dot x=-m\Omega^2y$, hence

$$
\boxed{\ddot y=-\Omega^2y,\qquad
H=\frac m2\dot z^2+E',\qquad E'=\frac m2(\dot y^2+\Omega^2y^2).}
$$

For nonzero constant $B_0$, the $(y,p_y)$ orbit is an ellipse of semiaxes $\sqrt{2E'/(m\Omega^2)}$ and $\sqrt{2mE'}$. Its enclosed phase-space area is $2\pi E'/|\Omega|$, so the [action variable](../../../../../action-variable.md) is

$$
\boxed{I(E',B_0)=\frac{E'}{|\Omega|}.}
$$

The absolute value keeps the action positive if the signed charge or [magnetic field](../../../../../magnetic-field.md) is negative.

When the field varies slowly along the trajectory, with $|d\Omega/dt|\ll\Omega^2$ and no zero-frequency crossing, [adiabatic invariance of the action](../../../../../adiabatic-invariance-of-the-action.md) makes $I$ approximately constant. Thus $E'\simeq I|\Omega(z,t)|$ and the slow motion has effective [Hamiltonian](../../../../../hamiltonian.md)

$$
\boxed{H_{\rm eff}=\frac{p_z^2}{2m}+I\left|\frac{eB_0(z,t)}{mc}\right|.}
$$

The [effective potential](../../../../../effective-potential.md) is the second term. Direct averaging checks its force: the exact equation is $m\ddot z=-m\Omega\partial_z\Omega\,y^2$, while the oscillator has $\langle y^2\rangle=E'/(m\Omega^2)$. Hence $m\ddot z=-I\partial_z|\Omega|$. Spatial field variation along the slow motion must satisfy the same adiabatic condition; slow explicit time variation alone does not control passage through a sharp spatial gradient. A time-dependent [effective potential](../../../../../effective-potential.md) need not conserve total energy.

## ↑ Ancestors (10)

1. [15E](../15e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
