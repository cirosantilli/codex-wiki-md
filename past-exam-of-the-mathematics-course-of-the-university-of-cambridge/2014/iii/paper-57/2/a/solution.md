<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the perturbation velocity as $(u,v)$, the density amplitude as $\sigma_1$, and $\gamma_d=\epsilon\Omega$. Axisymmetry removes advection by the background azimuthal flow, but the radial perturbation advects the [Keplerian shear](../../../../../../keplerian-shear.md): $u\,\partial_xU_{g,y}=-3\Omega u/2$. Combining this with the [Coriolis force](../../../../../../coriolis-force.md) gives the linearized [shearing sheet](../../../../../../shearing-sheet.md) equations

$$
s\sigma_1+ik\sigma_0u=0,\qquad
(s+\gamma_d)u-2\Omega v=-ik\left(\frac{c^2}{\sigma_0}-\frac{2\pi G}{|k|}\right)\sigma_1,\qquad
(s+\gamma_d)v+\frac\Omega2u=0.
$$

The [razor-thin disk Poisson kernel](../../../../../../razor-thin-disk-poisson-kernel.md) supplies the self-gravity term. The $\Omega/2$ coefficient, rather than $2\Omega$, is essential: it includes the perturbed advection of the background velocity.

Put $A=c^2k^2-2\pi G\sigma_0|k|$ and $\omega^2=\Omega^2+A$. The determinant of the three amplitude equations is

$$
s\left[(s+\gamma_d)^2+\Omega^2\right]+A(s+\gamma_d)=0.
$$

Expanding it gives the [dust gravitational dispersion relation with gas drag](../../../../../../dust-gravitational-dispersion-relation-with-gas-drag.md)

$$
\boxed{s^3+2\epsilon\Omega s^2+(\omega^2+\epsilon^2\Omega^2)s
+\epsilon\Omega(\omega^2-\Omega^2)=0,\quad
\omega^2=\Omega^2-2\pi G\sigma_0|k|+c^2k^2.}
$$

Using a determinant avoids division by $s$ and retains the neutral/secular branch. The [radial epicyclic frequency](../../../../../../radial-epicyclic-frequency.md) of this [Keplerian shearing sheet](../../../../../../keplerian-shearing-sheet.md) is $\Omega$, so the three terms in $\omega^2$ represent rotational support, [self-gravity](../../../../../../self-gravity.md) and dust [pressure](../../../../../../pressure.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 57](../../../paper-57-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
