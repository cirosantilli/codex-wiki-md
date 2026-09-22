<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the equilibrium [ideal gas](../../../../../../ideal-gas.md) be at rest, with uniform $\rho_0,p_0$ and $\mathbf B_0=B_0\mathbf e_z$. This local wave calculation neglects gravity, viscosity and magnetic diffusion. Define the [adiabatic sound speed](../../../../../../adiabatic-sound-speed.md) $c\equiv v_s=(\gamma p_0/\rho_0)^{1/2}$, the [Alfvén speed](../../../../../../alfven-speed.md) $v_a=B_0/(\mu_0\rho_0)^{1/2}$, and a [wavevector](../../../../../../wavevector.md) $\mathbf k=k(\sin\theta,0,\cos\theta)$, where $k=|\mathbf k|$ and $\theta$ is its angle to the equilibrium [magnetic field](../../../../../../magnetic-field.md). Perturbations have dependence $e^{i\mathbf k\cdot\mathbf x-i\omega t}$ and [phase speed](../../../../../../phase-speed.md) $v=\omega/k$.

The [linearized ideal magnetohydrodynamic equations](../../../../../../linearized-ideal-magnetohydrodynamic-equations.md) for [mass conservation](../../../../../../mass-conservation.md), [pressure](../../../../../../pressure.md), induction and momentum give

$$
\delta\rho=\frac{\rho_0}{\omega}\mathbf k\cdot\mathbf u',\qquad
\delta p=c^2\delta\rho,\qquad
\mathbf b=\frac{\mathbf B_0(\mathbf k\cdot\mathbf u')-\mathbf u'(\mathbf k\cdot\mathbf B_0)}\omega,
$$



$$
\omega\rho_0\mathbf u'=\mathbf k\delta p-
\frac1{\mu_0}\left[(\mathbf k\cdot\mathbf B_0)\mathbf b-\mathbf k(\mathbf B_0\cdot\mathbf b)\right].
$$

The relation between [pressure](../../../../../../pressure.md) and [mass density](../../../../../../density.md) follows from eliminating $\mathbf k\cdot\mathbf u'$ between the two material evolution equations; it applies to the nonzero-frequency wave sector. The induction result automatically has $\mathbf k\cdot\mathbf b=0$.

The $y$ [MHD wave polarization](../../../../../../magnetohydrodynamic-wave-polarization.md) is perpendicular to both the field and [wavevector](../../../../../../wavevector.md). It has $\delta p=\delta\rho=0$ and obeys

$$
\omega^2u'_y=v_a^2k^2\cos^2\theta\,u'_y.
$$

Thus the transverse [Alfvén wave](../../../../../../alfven-wave.md) has

$$
\boxed{v_A^2=v_a^2\cos^2\theta}.
$$

In the $x$-$z$ plane the two remaining [velocity](../../../../../../velocity.md) components instead obey the [symmetric matrix](../../../../../../symmetric-matrix.md) eigenproblem

$$
v^2\binom{u'_x}{u'_z}
=\begin{pmatrix}
v_a^2+c^2\sin^2\theta&c^2\sin\theta\cos\theta\\
c^2\sin\theta\cos\theta&c^2\cos^2\theta
\end{pmatrix}\binom{u'_x}{u'_z}.
$$

Taking its [determinant](../../../../../../determinant.md) gives $v^4-(c^2+v_a^2)v^2+c^2v_a^2\cos^2\theta=0$. Solving this [quadratic equation](../../../../../../quadratic-equation.md) in $v^2$ derives both [magnetoacoustic wave](../../../../../../magnetosonic-wave.md) [phase speeds](../../../../../../phase-speed.md),

$$
\boxed{v_{f,\mathrm{slow}}^2=\frac{c^2+v_a^2}{2}\pm
\sqrt{\frac{(c^2+v_a^2)^2}{4}-c^2v_a^2\cos^2\theta}}.
$$

The plus sign is the [fast magnetosonic wave](../../../../../../fast-magnetosonic-wave.md), the minus sign the [slow magnetosonic wave](../../../../../../slow-magnetosonic-wave.md). The radicand is nonnegative, since it equals $[(c^2-v_a^2)^2+4c^2v_a^2\sin^2\theta]/4$. Both squared speeds are nonnegative. Each nonzero mode has forward and backward propagation; an advected [entropy](../../../../../../entropy.md) disturbance is a separate zero-frequency mode in this static equilibrium.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
