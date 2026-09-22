<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Expand the [divergence](../../../../divergence.md) of $\Phi\nabla\Psi-\Psi\nabla\Phi$. The cross terms cancel, leaving $\Phi\Delta\Psi-\Psi\Delta\Phi$. The [divergence theorem](../../../../divergence-theorem.md) gives [Green's second identity](../../../../green-second-identity.md),

$$
\int_V(\Phi\Delta\Psi-\Psi\Delta\Phi)dV=\int_S(\Phi\partial_n\Psi-\Psi\partial_n\Phi)dS.
$$

Use the [Green function](../../../../green-s-function-split.md) convention $\Delta_xG(x,x_0)=\delta(x-x_0)$. Integrating over a bounded [domain](../../../../domain-mathematical-analysis.md) containing $x_0$ yields $\boxed{\int_S\partial_nG\,dS=1}$. Thus zero [Neumann boundary data](../../../../neumann-boundary-data.md) would be incompatible with this unit [Dirac delta](../../../../dirac-delta-function.md) source. A suitable [Neumann Green function with constant boundary flux](../../../../neumann-green-function-with-constant-boundary-flux.md) instead has $\partial_nG=1/|S|$, where $|S|$ is the boundary area. Substituting $\Psi=G$, $\Delta\Phi=\sigma$, $\partial_n\Phi=f$ gives

$$
\boxed{\Phi(x_0)=\int_VG\sigma\,dV-\int_SGf\,dS+\frac1{|S|}\int_S\Phi\,dS.}
$$

The last term is an undetermined constant. The data must obey the [Neumann Poisson problem](../../../../neumann-poisson-problem.md) compatibility condition $\int_V\sigma\,dV=\int_Sf\,dS$, obtained by integrating the original equation. Under this condition an additive constant in $G$ cancels from the first two terms.

For the upper half-space, reflect the source to $x_0^*=(x_{0,1},x_{0,2},-x_{0,3})$. The [method of images](../../../../method-of-images.md) with equal-sign sources gives

$$
\boxed{G(x,x_0)=-\frac1{4\pi}\left(\frac1{|x-x_0|}+\frac1{|x-x_0^*|}\right).}
$$

The reflected singularity lies outside the [domain](../../../../domain-mathematical-analysis.md); on $z=0$ the two normal [derivatives](../../../../derivative.md) cancel, so $\partial_nG=-\partial_zG=0$. Its total unit flux passes through a large hemisphere at infinity, where $G\sim-1/(2\pi R)$. This is why the bounded-domain condition on the boundary flux cannot be applied to the infinite plane alone.

With zero interior source and the given point boundary source, the boundary representation is $\Phi(x_0)=-G((0,0,0),x_0)$. The terms at infinity vanish for this resulting $1/R$ field. Therefore

$$
\boxed{\Phi(x,y,z)=\frac1{2\pi\sqrt{x^2+y^2+z^2}},\qquad z>0.}
$$

To check the singular boundary condition, $-\partial_z\Phi=z/[2\pi(x^2+y^2+z^2)^{3/2}]$ is the [Poisson kernel for the upper half-space](../../../../poisson-kernel-for-the-upper-half-space.md). Its [integral](../../../../integral-split.md) over a horizontal plane is one and its [mass](../../../../mass.md) concentrates at the origin as $z\downarrow0$, giving $\partial_n\Phi=\delta(x)\delta(y)$ in the distributional sense. This is the [Neumann point source on a half-space boundary](../../../../neumann-point-source-on-a-half-space-boundary.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Paper 2](../../paper-2-split.md)
3. [2003](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
