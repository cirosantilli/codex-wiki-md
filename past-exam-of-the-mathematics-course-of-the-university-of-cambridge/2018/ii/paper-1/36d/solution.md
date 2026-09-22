<h1 id="36d/solution">Solution</h1>

↑ **Parent:** [36D](../36d.md)

Use the [Minkowski metric](../../../../../minkowski-metric.md) $\eta=\operatorname{diag}(-1,1,1,1)$ and define the [electromagnetic field tensor](../../../../../electromagnetic-field-tensor.md) by

$$
F^{\mu\nu}=\partial^\mu A^\nu-\partial^\nu A^\mu.
$$

As a rank-two [Lorentz tensor](../../../../../lorentz-tensor.md), it transforms under a [Lorentz transformation](../../../../../lorentz-transformation.md) as

$$
\boxed{F'^{\mu\nu}(x')
=\Lambda^\mu{}_{\rho}\Lambda^\nu{}_{\sigma}F^{\rho\sigma}(x).}
$$

Two independent quadratic [electromagnetic field invariants](../../../../../electromagnetic-field-invariants.md) are

$$
I_1=\frac12F_{\mu\nu}F^{\mu\nu},
\qquad
I_2=\frac12F_{\mu\nu}\widetilde F^{\mu\nu},
\qquad
\widetilde F^{\mu\nu}=\frac12\varepsilon^{\mu\nu\rho\sigma}F_{\rho\sigma}.
$$

With $A^\mu=(\phi/c,\mathbf A)$, $\mathbf E=-\nabla\phi-\partial_t\mathbf A$, and $\mathbf B=\nabla\times\mathbf A$, the components are

$$
F^{\mu\nu}=
\begin{pmatrix}
0&E_x/c&E_y/c&E_z/c\\
-E_x/c&0&B_z&-B_y\\
-E_y/c&-B_z&0&B_x\\
-E_z/c&B_y&-B_x&0
\end{pmatrix}.
$$

Direct contraction gives

$$
\boxed{I_1=\mathbf B^2-\frac{\mathbf E^2}{c^2}=S,}
\qquad
\boxed{I_2=-\frac{2}{c}\mathbf E\mathbin\cdot\mathbf B=-\frac{2}{c}T,}
$$

where the sign of $I_2$ changes if the opposite spacetime orientation is chosen. Since both are complete tensor contractions, $S$ and $T$ are [Lorentz scalars](../../../../../lorentz-scalar.md).

For a constant uniform field, the [relativistic Lorentz force](../../../../../relativistic-lorentz-force.md) is a constant-coefficient [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation.md). Its solution is the [matrix exponential](../../../../../matrix-exponential.md)

$$
\boxed{u^\mu(\tau)=
\left[\exp\left(\frac{q\tau}{m}F\right)\right]^\mu{}_{\nu}u^\nu(0)
=\sum_{n=0}^{\infty}\frac1{n!}
\left(\frac{q\tau}{m}\right)^n
(F^n)^\mu{}_{\nu}u^\nu(0).}
$$

Now $S=T=0$ implies that the field is a [null electromagnetic field](../../../../../null-electromagnetic-field.md):

$$
\mathbf E\perp\mathbf B,
\qquad |\mathbf E|=c|\mathbf B|.
$$

The stated axes allow us to choose

$$
\mathbf B=B\mathbf e_z,
\qquad
\mathbf E=cB\mathbf e_x.
$$

Put $\Omega=qB/m$. On the $(ct,x,y)$ coordinates, the mixed tensor divided by $B$ is

$$
N=\begin{pmatrix}0&1&0\\1&0&1\\0&-1&0\end{pmatrix},
\qquad N^3=0.
$$

The particle starts with [four-velocity](../../../../../four-velocity.md) $u(0)=(c,0,0,0)$, so the exponential terminates after its quadratic term and gives

$$
u^0=c\left(1+\frac{\Omega^2\tau^2}{2}\right),
\qquad
u^x=c\Omega\tau,
\qquad
u^y=-\frac{c\Omega^2\tau^2}{2},
\qquad u^z=0.
$$

Integrating with the particle initially at the origin gives the [relativistic trajectory in a constant null crossed field](../../../../../relativistic-trajectory-in-a-constant-null-crossed-field.md)

$$
x=\frac{c\Omega\tau^2}{2},
\qquad
y=-\frac{c\Omega^2\tau^3}{6}.
$$

Eliminating $\tau$ yields

$$
\boxed{y^2=Ax^3,
\qquad A=\frac{2qB}{9mc}.}
$$

If the original positive $x$ direction is opposite to $\mathbf E$, both the sign of $x$ and the displayed signed coefficient reverse.

## ↑ Ancestors (10)

1. [36D](../36d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
