<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $\mathbf u=\nabla\times(\psi\hat{\mathbf y})$,

$$
\boxed{u=-\psi_z,\qquad w=\psi_x}.
$$

Hence $u_x+w_z=-\psi_{zx}+\psi_{xz}=0$, so [mass conservation](../../../../../../mass-conservation.md) holds identically. Removing the hydrostatic part by writing

$$
p=-\rho gz+p',
$$

and taking the curl of the [Stokes flow](../../../../../../stokes-flow-split.md) equation gives the biharmonic equation

$$
\boxed{\nabla^4\psi=0}.
$$

For a [Fourier mode](../../../../../../fourier-mode.md) proportional to $e^{ikx}$ with $k>0$, decay as $z\to-\infty$ selects

$$
\psi=(A+Cz)e^{kz}e^{ikx}.
$$

The velocity and pressure fields are therefore

$$
\boxed{
u=-[C+k(A+Cz)]e^{kz}e^{ikx}},
$$



$$
\boxed{
w=ik(A+Cz)e^{kz}e^{ikx}},
$$



$$
\boxed{
p=-\rho gz+2i\mu kC\,e^{kz}e^{ikx}}.
$$

Direct substitution verifies the momentum equation.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
