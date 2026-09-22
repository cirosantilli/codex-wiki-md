<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take the equilibrium [mass density](../../../../../density.md) to be constant and absorb any conservative equilibrium force into the [pressure](../../../../../pressure.md). The linearized [ideal magnetohydrodynamic induction equation](../../../../../ideal-magnetohydrodynamic-induction-equation.md), using the [solenoidal vector field](../../../../../solenoidal-vector-field.md) conditions, is

$$
\partial_t\mathbf b=(\mathbf B\cdot\nabla)\mathbf u-(\mathbf u\cdot\nabla)\mathbf B.
$$

For $\mathbf B=Jr\mathbf e_\phi$, differentiation of the cylindrical basis is important. Acting on a vector whose cylindrical components have azimuthal dependence $e^{im\phi}$ gives $(\mathbf B\cdot\nabla)\mathbf u=imJ\mathbf u+J\mathbf e_z\times\mathbf u$. Also $(\mathbf u\cdot\nabla)\mathbf B=J\mathbf e_z\times\mathbf u$. These basis contributions cancel in induction, giving **$i\omega\mathbf b=imJ\mathbf u$**.

The perturbation of the [Lorentz force](../../../../../lorentz-force.md) is

$$
(\nabla\times\mathbf b)\times\mathbf B+(\nabla\times\mathbf B)\times\mathbf b=(\mathbf B\cdot\nabla)\mathbf b+(\mathbf b\cdot\nabla)\mathbf B-\nabla(\mathbf B\cdot\mathbf b).
$$

Both of the first two terms now contribute a basis-rotation term. With $\widetilde p=p_1/\rho+\mathbf B\cdot\mathbf b/(\mu_0\rho)$, the linearized [ideal magnetohydrodynamic momentum equation](../../../../../ideal-magnetohydrodynamic-momentum-equation.md) is therefore

$$
\boxed{i\omega\mathbf u=-\nabla\widetilde p+\frac1{\mu_0\rho}(imJ\mathbf b+2J\mathbf e_z\times\mathbf b),\qquad i\omega\mathbf b=imJ\mathbf u.}
$$

The magnetic part of $\widetilde p$ is the perturbation of [magnetic pressure](../../../../../magnetic-pressure.md), not an extra restoring force to retain after projecting out [pressure](../../../../../pressure.md).

Put $D=\omega^2-m^2\widetilde J^2$, where $\widetilde J=J/\sqrt{\mu_0\rho}$. For $mJ\ne0$, substitute $\mathbf u=\omega\mathbf b/(mJ)$ into the momentum equation and multiply by $mJ$. Taking a curl removes the modified [pressure](../../../../../pressure.md). Since

$$
\nabla\times(\mathbf e_z\times\mathbf b)=\mathbf e_z\nabla\cdot\mathbf b-\partial_z\mathbf b=-ik\mathbf b,
$$

we obtain the [uniform-current toroidal-field curl reduction](../../../../../uniform-current-toroidal-field-curl-reduction.md)

$$
D\nabla\times\mathbf b=-2mk\widetilde J^2\mathbf b.
$$

A second curl, using $\nabla\times\nabla\times\mathbf b=-\nabla^2\mathbf b$, gives

$$
\boxed{\nabla^2\mathbf b=-\frac{4m^2k^2\widetilde J^4}{(\omega^2-m^2\widetilde J^2)^2}\mathbf b.}
$$

The divided expression assumes $D\ne0$. If $mkJ\ne0$, the undivided curl equation shows that $D=0$ would force $\mathbf b=0$, so this restriction loses no such magnetic mode. The $k=0$ degenerate limit can instead be taken in the undivided equations; it has no growing branch of the kind considered below. Axisymmetric $m=0$ disturbances are likewise excluded by the [velocity](../../../../../velocity.md) elimination, and induction gives no nonzero-frequency magnetic disturbance in this particular equilibrium.

For a vector Laplacian eigenmode with $\alpha^2+k^2>0$, elimination gives

$$
D^2=\frac{4m^2k^2\widetilde J^4}{\alpha^2+k^2},\qquad \boxed{\omega^2_\pm=\widetilde J^2\left(m^2\pm\frac{2|mk|}{\sqrt{\alpha^2+k^2}}\right).}
$$

Thus **both squared frequencies are real**. The lower branch satisfies $\omega_-^2\geq\widetilde J^2(|m|^2-2|m|)$, so it is positive for $|m|>2$. For $|m|=2$ it is positive when $\alpha\ne0$, but the printed strict-positivity statement needs an endpoint qualification: **$|m|=2$, $\alpha=0$ permits a neutral mode unless boundary conditions exclude it**.

This is a genuine counterexample to the unqualified endpoint, not merely a loose algebraic bound. The [neutral quadrupolar perturbation of a uniform-current toroidal field](../../../../../neutral-quadrupolar-perturbation-of-a-uniform-current-toroidal-field.md)

$$
\mathbf b=Cr(\mathbf e_r+i\mathbf e_\phi)e^{2i\phi+ikz},\qquad \mathbf u=0,\qquad \widetilde p=0,\qquad \omega=0
$$

is regular at the axis, is solenoidal, and has $\nabla\times\mathbf b=k\mathbf b$, hence $\nabla^2\mathbf b=-k^2\mathbf b$. Also $\mathbf e_z\times\mathbf b=-i\mathbf b$, so the non-gradient part of the linearized [Lorentz force](../../../../../lorentz-force.md) vanishes for $m=2$. The gas-pressure perturbation $p_1=-\mathbf B\cdot\mathbf b/\mu_0$ cancels its [magnetic pressure](../../../../../magnetic-pressure.md) gradient, as required by $\widetilde p=0$. Taking its real part gives a real disturbance. Decay at radial infinity or an appropriate homogeneous radial boundary condition would exclude it, restoring strict positivity for the allowed eigenmodes; no such condition is printed.

For $|m|=1$ the lower branch is unstable precisely when

$$
\boxed{m=\pm1,\qquad k\ne0,\qquad \alpha^2<3k^2.}
$$

At equality it is marginal. With the time convention $e^{i\omega t}$, the growing member has $\omega=-is$ and

$$
s=|\widetilde J|\sqrt{\frac{2|k|}{\sqrt{\alpha^2+k^2}}-1}.
$$

The other branch remains oscillatory. Actual admissibility of a chosen $\alpha$ depends on the radial domain and its [boundary conditions](../../../../../boundary-condition.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 59](../../paper-59-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
