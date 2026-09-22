<h1 id="7e/solution">Solution</h1>

↑ **Parent:** [7E](../7e.md)

For a moving circuit, [Faraday's law](../../../../../faraday-s-law-of-induction.md) takes the form

$$
\boxed{\mathcal E(t)=\oint_{C(t)}(\mathbf E+\mathbf v\times\mathbf B)\cdot d\boldsymbol\ell=-\frac d{dt}\int_{S(t)}\mathbf B\cdot\mathbf n\,dS.}
$$

Here $C(t)$ is the instantaneous wire [contour](../../../../../complex-integration-contour.md), $\mathbf v$ its local material [velocity](../../../../../velocity.md), and $S(t)$ any spanning surface. The [contour](../../../../../complex-integration-contour.md) [orientation](../../../../../orientation-of-a-simplex.md) and surface [normal vector](../../../../../normal-vector.md) obey the right-hand convention. The [integral](../../../../../integral.md) on the right is the [magnetic flux](../../../../../magnetic-flux.md), differentiated with both the field and circuit position allowed to vary. The [electric field](../../../../../electric-field.md) term is the electric force per unit [electric charge](../../../../../electric-charge.md) around the wire, and $\mathbf v\times\mathbf B$ supplies the [motional electromotive force](../../../../../motional-electromotive-force.md). Their sum is the [electromotive force](../../../../../electromotive-force.md) driving charge around the moving circuit. The condition $\nabla\cdot\mathbf B=0$ makes the [magnetic flux](../../../../../magnetic-flux.md) independent of the spanning surface.

Choose the initial loop [normal vector](../../../../../normal-vector.md) to be $+\mathbf e_y$, so [rotation](../../../../../rotation-mathematics.md) about $+\mathbf e_z$ gives $\mathbf n(t)=(-\sin\Omega t,\cos\Omega t,0)$. The spatially uniform [magnetic field](../../../../../magnetic-field.md) gives

$$
\Phi(t)=\pi a^2B_0\bigl[-\sin\Omega t\cos\omega t+\cos\Omega t\sin\omega t\bigr]=\pi a^2B_0\sin((\omega-\Omega)t).
$$

Using [Ohm's law](../../../../../ohm-s-law.md) for the resistive loop,

$$
\boxed{I(t)=\frac{\pi a^2B_0(\Omega-\omega)}R\cos((\omega-\Omega)t).}
$$

Positive [electric current](../../../../../electric-current.md) is measured in the [contour](../../../../../complex-integration-contour.md) [orientation](../../../../../orientation-of-a-simplex.md) associated with $\mathbf n(t)$. Reversing that convention reverses the signed answer. When $\Omega=\omega$, the [magnetic flux](../../../../../magnetic-flux.md) is constant and the induced [electric current](../../../../../electric-current.md) vanishes. This uses the usual thin resistive-circuit approximation with [self-inductance](../../../../../self-inductance.md) neglected.

## ↑ Ancestors (10)

1. [7E](../7e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
