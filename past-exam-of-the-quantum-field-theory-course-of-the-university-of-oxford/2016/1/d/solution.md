<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Under the finite [dilation](../../../../uniform-dilation.md), the [volume element](../../../../volume-element.md) transforms as $d^4x'=e^{4\alpha}d^4x$, whereas $\partial'_\mu\phi'(x')=e^{-2\alpha}\partial_\mu\phi(x)$. Thus the [kinetic term](../../../../kinetic-term.md) and [quartic interaction](../../../../quartic-interaction.md) both acquire the factor $e^{-4\alpha}$. Their factors cancel the [Jacobian determinant](../../../../jacobian-determinant.md), proving

$$
\boxed{S[\phi']=S[\phi]\quad(m=0).}
$$

A [mass term](../../../../mass-term.md) would instead acquire a net factor $e^{2\alpha}$ in the [action](../../../../action.md) and break this [scale invariance](../../../../scale-invariance.md).

For the [Noether current](../../../../noether-current.md), use the variation at the same coordinate, rather than comparing values at different coordinates:

$$
\delta_0\phi(x)=\phi'(x)-\phi(x)
=-\alpha\bigl(\phi+x^\nu\partial_\nu\phi\bigr).
$$

At $m=0$, the corresponding [Lagrangian density](../../../../lagrangian-density.md) variation is $\delta_0\mathcal L=-\alpha(4+x\cdot\partial)\mathcal L=-\alpha\partial_\mu(x^\mu\mathcal L)$. Thus $J_0^\mu=-x^\mu\mathcal L$, and the stated [Noether current](../../../../noether-current.md) convention gives

$$
\boxed{j^\mu=-x_\nu T^{\mu\nu}-\phi\partial^\mu\phi.}
$$

The frequently used [dilatation current](../../../../dilatation-current.md) $D^\mu=x_\nu T^{\mu\nu}+\phi\partial^\mu\phi$ is $-j^\mu$; this is solely an overall parameter convention. In the convention $D^\mu=x_\nu T^{\mu\nu}-V^\mu$, the [virial current](../../../../virial-current.md) is $V^\mu=-\phi\partial^\mu\phi$.

Using [solution](../b/solution.md) and the [trace](../../../../matrix-trace.md) computed in [solution](../c/solution.md) gives the useful identity

$$
\partial_\mu D^\mu
=T^\mu{}_{\mu}+x^\nu F\partial_\nu\phi+(\partial\phi)^2+\phi\Box\phi
=m^2\phi^2+\bigl(\phi+x^\nu\partial_\nu\phi\bigr)F.
$$

It follows that $\boxed{\partial_\mu j^\mu=0}$ in the massless theory [on shell](../../../../on-shell.md). Equivalently, $x_\nu\Omega^{\mu\nu}$ is a [conserved current](../../../../conserved-current.md), since its [divergence](../../../../divergence.md) is the [trace](../../../../matrix-trace.md) of the improved [stress-energy tensor](../../../../stress-energy-tensor-split.md) [on shell](../../../../on-shell.md). These are classical [scale invariance](../../../../scale-invariance.md) statements; the nonzero [beta function](../../../../beta-function.md) in [solution](../../4/d/solution.md) explains why the interacting quantum theory need not retain them.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../../4/d/solution.md)
