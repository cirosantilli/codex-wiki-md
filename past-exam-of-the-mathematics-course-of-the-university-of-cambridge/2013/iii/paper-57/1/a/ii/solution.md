<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In [Bohmian mechanics](../../../../../../../de-broglie-bohm-theory.md) the particle has a definite position $\mathbf X(t)$ at every time. Its [wavefunction](../../../../../../../wave-function.md) obeys the usual autonomous wave equation, while its actual position follows the [guidance equation](../../../../../../../guidance-equation.md)

$$
\dot{\mathbf X}(t)=\mathbf v(\mathbf X(t),t),\qquad
\mathbf v=\frac{\hbar}{m}\nabla S=\frac{\mathbf j}{|\psi|^2}.
$$

Here $\mathbf j$ is the [probability current](../../../../../../../probability-current.md). The [Born rule](../../../../../../../born-rule.md) is the quantum-equilibrium choice of initial position distribution $\rho=|\psi|^2$; [quantum equilibrium equivariance](../../../../../../../quantum-equilibrium-equivariance.md) ensures that this distribution persists because it obeys the same [probability continuity equation](../../../../../../../probability-continuity-equation.md) as the wave amplitude. The [guidance equation](../../../../../../../guidance-equation.md) fixes the initial velocity as well as subsequent velocities: the second-order equation below does not permit an independent arbitrary initial velocity.

Define the [quantum potential](../../../../../../../quantum-potential.md)

$$
\boxed{Q=-\frac{\hbar^2}{2m}\frac{\nabla^2R}{R}}.
$$

Taking the [gradient](../../../../../../../gradient.md) of the real [Madelung equations](../../../../../../../madelung-equations.md) gives

$$
\hbar\partial_t\nabla S+\nabla\left(\frac{\hbar^2}{2m}|\nabla S|^2\right)=-\nabla(V+Q).
$$

On any smooth phase patch $\nabla\times\mathbf v=0$, so $\nabla(|\mathbf v|^2/2)=(\mathbf v\cdot\nabla)\mathbf v$. Along the actual path, differentiation is the [material derivative](../../../../../../../material-derivative.md) $D/Dt=\partial_t+\mathbf v\cdot\nabla$. Therefore

$$
\boxed{\frac{d(m\dot{\mathbf X})}{dt}=m\frac{D\mathbf v}{Dt}=-\nabla(V+Q)\big|_{\mathbf X(t)}}.
$$

This is the [Bohmian mechanics](../../../../../../../de-broglie-bohm-theory.md) Newton form: the classical force is supplemented by the amplitude-dependent [quantum potential](../../../../../../../quantum-potential.md). Neither division by $R$ nor a smooth phase is justified at a [wavefunction](../../../../../../../wave-function.md) node, so the derivation applies on nonzero-amplitude regions. A nonzero circulation around a node is compatible with the locally curl-free [guidance equation](../../../../../../../guidance-equation.md).

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 57](../../../../paper-57-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
