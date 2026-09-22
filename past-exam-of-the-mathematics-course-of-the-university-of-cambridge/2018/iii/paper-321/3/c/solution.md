<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For an [axisymmetric vertical mode of a shearing sheet](../../../../../../axisymmetric-vertical-mode-of-a-shearing-sheet.md) in this [Boussinesq approximation](../../../../../../boussinesq-approximation.md), the perturbations have no horizontal gradients, so background-shear advection vanishes. The linear [Coriolis acceleration](../../../../../../coriolis-acceleration.md) and perturbation advection of the background shear give

$$
su'_x-2\Omega u'_y=-N^2\theta',\qquad
su'_y+\frac\Omega2u'_x=0,\qquad
su'_z=-\frac{ik}{\rho_0}P',
$$

while [thermal conduction](../../../../../../thermal-conduction.md) and [incompressibility](../../../../../../incompressible-flow.md) give

$$
(s+\beta)\theta'=u'_x,\qquad iku'_z=0,\qquad \beta=\xi k^2>0.
$$

Here $\beta$ is the [thermal diffusion rate of a Fourier mode](../../../../../../thermal-diffusion-rate-of-a-fourier-mode.md), not the cooling exponent in Question 2. Since $k\ne0$, [incompressibility](../../../../../../incompressible-flow.md) forces $u'_z=0$, and the vertical momentum equation then forces $P'=0$ for this nonzero-[wavenumber](../../../../../../wavenumber.md) amplitude.

The three remaining amplitudes satisfy

$$
\begin{pmatrix}s&-2\Omega&N^2\\\Omega/2&s&0\\-1&0&s+\beta\end{pmatrix}
\begin{pmatrix}u'_x\\u'_y\\\theta'\end{pmatrix}=0.
$$

A nontrivial solution requires the [determinant](../../../../../../determinant.md) to vanish, giving the [convective overstability](../../../../../../convective-overstability.md) [dispersion relation](../../../../../../dispersion-relation.md)

$$
\boxed{(s+\beta)(s^2+\Omega^2)+N^2s=0,\quad\text{or}\quad
s^3+\beta s^2+(N^2+\Omega^2)s+\beta\Omega^2=0.}
$$

No division by $s$ or $s+\beta$ was needed, so the [thermal energy mode of a shearing sheet](../../../../../../thermal-energy-mode-of-a-shearing-sheet.md) is retained. The notation $N^2$ denotes a signed [buoyancy frequency](../../../../../../buoyancy-frequency.md) squared and can be negative for an adverse stratification; it must not be restricted to the square of a real positive frequency.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
