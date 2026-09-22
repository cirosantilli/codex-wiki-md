<h1 id="18a/solution">Solution</h1>

↑ **Parent:** [18A](../18a.md)

For a [conductor in electrostatic equilibrium](../../../../../conductor-in-electrostatic-equilibrium.md), the interior field is zero and the surface is equipotential. The tangential exterior field is zero. A thin Gaussian pillbox gives the normal jump $E_{\rm out}\cdot\mathbf n-E_{\rm in}\cdot\mathbf n=\sigma/\epsilon_0$. Thus, in vacuum and with $\mathbf n$ pointing out of the conductor,

$$
\boxed{\mathbf E_{\rm out}=\frac{\sigma}{\epsilon_0}\mathbf n.}
$$

These are the [electrostatic boundary conditions at a conductor](../../../../../electrostatic-boundary-conditions-at-a-conductor.md).

To obtain [electrostatic energy](../../../../../electrostatic-energy.md) in field form, integrate over the space outside the conductors, cutting it off first at a large sphere. From the [Maxwell equations](../../../../../maxwell-equations.md), $\nabla\cdot\mathbf E=\rho/\epsilon_0$ and $\mathbf E=-\nabla\phi$, so

$$
\nabla\cdot(\phi\mathbf E)=\frac{\rho\phi}{\epsilon_0}-|\mathbf E|^2.
$$

On a conductor boundary, the outward normal of the integration region points into the conductor, so its flux contribution is $-\phi_iQ_i/\epsilon_0$. At the remote outer boundary the flux integral tends to zero: for a localized charge distribution, $\phi=O(1/r)$ and $\mathbf E=O(1/r^2)$. The [divergence theorem](../../../../../divergence-theorem.md) therefore gives

$$
-\frac1{\epsilon_0}\sum_i\phi_iQ_i
=\frac1{\epsilon_0}\int_V\rho\phi\,d\tau
-\int_{\text{outside conductors}}|\mathbf E|^2\,d\tau.
$$

Since the field vanishes inside conductors,

$$
\boxed{W=\frac{\epsilon_0}{2}\int_{\mathbb R^3}|\mathbf E|^2\,d\tau.}
$$

The field integral is over all space, although the charges occupy a finite volume. For a finite outer integration boundary there is additionally the term $(\epsilon_0/2)\oint\phi\mathbf E\cdot d\mathbf S$.

For the [electrostatic energy of alternating-charge concentric shells](../../../../../electrostatic-energy-of-alternating-charge-concentric-shells.md), the total enclosed charge after shell $n$ is

$$
Q_{\le n}=q+2q\sum_{j=2}^n(-1)^{j+1}=(-1)^{n+1}q.
$$

By spherical symmetry and [Gauss's law](../../../../../gauss-s-law.md), the field is zero for $r<r_1$, and in every subsequent gap, including outside the last shell,

$$
|\mathbf E|=\frac{|q|}{4\pi\epsilon_0r^2}.
$$

Although its direction alternates, its squared magnitude is the same in every gap. Consequently

$$
\boxed{W=\frac{\epsilon_0}{2}\,4\pi
\int_{r_1}^{\infty}\frac{q^2}{16\pi^2\epsilon_0^2r^4}r^2\,dr
=\frac{q^2}{8\pi\epsilon_0r_1}.}
$$

The coefficient of $1/r_1$ is $q^2/(8\pi\epsilon_0)$, independent of the other radii and of the number of shells.

## ↑ Ancestors (10)

1. [18A](../18a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
