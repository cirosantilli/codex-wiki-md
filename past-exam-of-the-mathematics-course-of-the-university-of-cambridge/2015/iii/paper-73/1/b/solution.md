<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\mathbf n=\mathbf X/R$, $\zeta=6\pi\mu a$, and let

$$
\mathsf G(\mathbf r)=\frac{I+\widehat{\mathbf r}\widehat{\mathbf r}}{8\pi\mu r},\qquad\mathsf A=\zeta\mathsf G(\mathbf X)=\frac{3a}{4R}(I+\mathbf n\mathbf n).
$$

Use the [method of reflections for Stokes flow](../../../../../../method-of-reflections-for-stokes-flow.md). At the fixed [sphere](../../../../../../sphere.md), the first [sphere](../../../../../../sphere.md) produces the incident [Stokeslet](../../../../../../stokeslet.md) [velocity](../../../../../../velocity.md) $\mathbf u_\infty(0)=\mathsf A\mathbf V$ to leading order. In [Faxén translation law](../../../../../../faxen-s-first-law.md), set the second [sphere](../../../../../../sphere.md)'s translational [velocity](../../../../../../velocity.md) to zero. The applied holding [force](../../../../../../force.md) is therefore

$$
\boxed{\mathbf F_2=-\frac{9\pi\mu a^2}{2R}\left[\mathbf V+(\mathbf V\cdot\mathbf n)\mathbf n\right]+O\left(\frac{\mu Va^4}{R^3}\right).}
$$

The first [sphere](../../../../../../sphere.md)'s finite-radius [potential dipole](../../../../../../potential-dipole.md) adds $O(Va^3/R^3)$ to the incident [velocity](../../../../../../velocity.md), as does the [Laplacian](../../../../../../laplacian.md) term in [Faxén translation law](../../../../../../faxen-s-first-law.md) at the fixed [sphere](../../../../../../sphere.md). Multiplying by $\zeta$ gives the stated next correction. There is no intermediate $O(\mu Va^3/R^2)$ term. This is the [holding force and torque for a sphere in a distant Stokeslet](../../../../../../holding-force-and-torque-for-a-sphere-in-a-distant-stokeslet.md).

The [vorticity](../../../../../../vorticity.md) of a [Stokeslet](../../../../../../stokeslet.md) at displacement $\mathbf r$ is $\mathbf F\times\mathbf r/(4\pi\mu r^3)$. At the fixed [sphere](../../../../../../sphere.md), $\mathbf r=-\mathbf X$, so

$$
\boldsymbol\omega_\infty(0)=-\frac{3a}{2R^3}\mathbf V\times\mathbf X.
$$

Set its [angular velocity](../../../../../../angular-velocity.md) to zero in [Faxén rotation law](../../../../../../faxen-s-rotational-law.md). The applied holding couple is

$$
\boxed{\mathbf G_2=-4\pi\mu a^3\boldsymbol\omega_\infty(0)=\frac{6\pi\mu a^4}{R^3}\mathbf V\times\mathbf X+O\left(\frac{\mu Va^6}{R^4}\right).}
$$

The displayed sign is the external couple needed to oppose the ambient rotation, rather than the hydrodynamic couple on the [sphere](../../../../../../sphere.md).

The leading reflected flow at the first [sphere](../../../../../../sphere.md) is $\mathsf G(\mathbf X)\mathbf F_2=-\mathsf A^2\mathbf V$. Apply [Faxén translation law](../../../../../../faxen-s-first-law.md) there with its prescribed [force](../../../../../../force.md) $\mathbf F=\zeta\mathbf V$. Since $(I+\mathbf n\mathbf n)^2=I+3\mathbf n\mathbf n$, the [mobility correction from a fixed distant sphere](../../../../../../mobility-correction-from-a-fixed-distant-sphere.md) is

$$
\boxed{\dot{\mathbf X}=\mathbf V-\frac{9a^2}{16R^2}\left[\mathbf V+3(\mathbf V\cdot\mathbf n)\mathbf n\right]+O\left(\frac{Va^4}{R^4}\right).}
$$

The next correction comes from finite-radius terms in the incident/reflected flow and in [Faxén translation law](../../../../../../faxen-s-first-law.md), together with the fixed [sphere](../../../../../../sphere.md)'s induced [stresslet](../../../../../../force-dipole-flow.md) and holding-couple [rotlet](../../../../../../rotlet.md). Each gives $O(Va^4/R^4)$ at the first [sphere](../../../../../../sphere.md). The symbol $\mathbf V$ is its isolated-sphere [velocity](../../../../../../velocity.md) scale, not its actual [velocity](../../../../../../velocity.md) in the two-sphere problem.

The first [sphere](../../../../../../sphere.md) has no applied couple. Its [angular velocity](../../../../../../angular-velocity.md) follows from [Faxén rotation law](../../../../../../faxen-s-rotational-law.md) and the reflected [Stokeslet](../../../../../../stokeslet.md):

$$
\boldsymbol\Omega_1=\frac{\mathbf F_2\times\mathbf X}{8\pi\mu R^3}+O\left(\frac{Va^4}{R^5}\right)=\boxed{-\frac{9a^2}{16}\frac{\mathbf V\times\mathbf X}{R^4}+O\left(\frac{Va^4}{R^5}\right).}
$$

The component of $\mathbf F_2$ parallel to $\mathbf X$ contributes no [vorticity](../../../../../../vorticity.md). The next reflected [rotlet](../../../../../../rotlet.md) and [stresslet](../../../../../../force-dipole-flow.md) give the stated error order.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 73](../../../paper-73-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
