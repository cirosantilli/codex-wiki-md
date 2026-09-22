<h1 id="17e/solution">Solution</h1>

↑ **Parent:** [17E](../17e.md)

In SI units, the two curl [Maxwell equations](../../../../../maxwell-equations.md) are

$$
\nabla\times\mathbf B=\mu_0\mathbf j+\mu_0\epsilon_0\mathbf E_t,
\qquad \nabla\times\mathbf E=-\mathbf B_t.
$$

Use the vector identity $\nabla\cdot(\mathbf E\times\mathbf B)=\mathbf B\cdot(\nabla\times\mathbf E)-\mathbf E\cdot(\nabla\times\mathbf B)$ to obtain

$$
\partial_t\left(\frac{\epsilon_0E^2}{2}+\frac{B^2}{2\mu_0}\right)
+\nabla\cdot\frac{\mathbf E\times\mathbf B}{\mu_0}
=-\mathbf j\cdot\mathbf E.
$$

Integration over the fixed volume and the [divergence theorem](../../../../../divergence-theorem.md) give [Poynting's theorem](../../../../../poynting-theorem.md):

$$
\boxed{\frac{d}{dt}\int_V\left(\frac{\epsilon_0E^2}{2}+\frac{B^2}{2\mu_0}\right)dV
+\int_S\mathbf P\cdot\mathbf n\,dS=-\int_V\mathbf j\cdot\mathbf E\,dV,
\qquad \mathbf P=\frac{\mathbf E\times\mathbf B}{\mu_0}.}
$$

The first term is the rate of change of stored [electromagnetic energy](../../../../../electromagnetic-energy.md). The surface integral is the outward energy flux carried by the [Poynting vector](../../../../../poynting-vector.md). The right side is minus the power delivered by the field to matter; for an [Ohmic conductor](../../../../../ohmic-conductor.md) it is minus the [Ohmic heating](../../../../../joule-heating.md) rate. Thus energy lost from the field either flows out or does work on charges.

For the specified transverse [plane wave](../../../../../plane-wave.md), both divergence [Maxwell equations](../../../../../maxwell-equations.md) hold because $E_y$ depends only on $x,t$. Faraday's equation requires

$$
\boxed{\mathbf B=\frac{kE_0}{\omega}(0,0,1)\cos(kx-\omega t).}
$$

Here we take the magnetic wave associated with the electric wave, without an additional static background field. Ampère's vacuum equation then gives $k^2=\mu_0\epsilon_0\omega^2$, equivalently

$$
\boxed{\omega^2=c^2k^2,\qquad c=(\mu_0\epsilon_0)^{-1/2}.}
$$

Thus all four vacuum [Maxwell equations](../../../../../maxwell-equations.md) are satisfied. The [Poynting vector](../../../../../poynting-vector.md) is $\mathbf P=(kE_0^2/(\mu_0\omega))\cos^2(kx-\omega t)\mathbf e_x$, and averaging over a period gives

$$
\boxed{\langle\mathbf P\rangle=\frac{kE_0^2}{2\mu_0\omega}\mathbf e_x.}
$$

For propagation in the positive $x$ direction, $\omega=ck$ and this is $E_0^2\mathbf e_x/(2\mu_0c)$. It represents the mean energy transmitted per unit area per unit time, the wave's time-averaged [energy flux](../../../../../energy-flux.md) per unit area, directed along its propagation.

## ↑ Ancestors (10)

1. [17E](../17e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
