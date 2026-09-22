<h1 id="38a/solution">Solution</h1>

↑ **Parent:** [38A](../38a.md)

The displacement equation is $\rho\mathbf u_{tt}=(\lambda+\mu)\nabla(\nabla\cdot\mathbf u)+\mu\Delta\mathbf u$. With $\mathbf u=\nabla\phi+\nabla\times\boldsymbol\psi$ and divergence-free vector-potential gauge, divergence and curl give [wave equations](../../../../../wave-equation-split.md) with

$$
\boxed{c_P^2=(\lambda+2\mu)/\rho,\qquad c_S^2=\mu/\rho.}
$$

Thus $\phi_{tt}=c_P^2\Delta\phi$ and $\boldsymbol\psi_{tt}=c_S^2\Delta\boldsymbol\psi$, up to gauge constants. The [P wave](../../../../../p-wave.md) displacement is parallel to its propagation direction; [S wave](../../../../../s-wave.md) displacement is perpendicular, with two transverse polarizations.

Take the plane of incidence to be $xy$. Let $k$ be the shared tangential wave number, $h=(\omega^2/c_P^2-k^2)^{1/2}$ and $s=(\omega^2/c_S^2-k^2)^{1/2}$. Incident P, reflected P and reflected SV waves have respectively wave vectors $(k,h)$, $(k,-h)$ and $(k,-s)$. Thus the reflected P angle equals $\theta$ and $\sin\theta_S=(c_S/c_P)\sin\theta$. No SH wave is excited by this planar P incidence.

Use scalar potentials $\mathbf u=(\phi_x+\psi_y,\phi_y-\psi_x)$, with incident potential amplitude one, reflected P amplitude $R$, and reflected SV amplitude $Q$. At the surface their phases are common. Vanishing $xy$ and $yy$ [tractions](../../../../../traction.md) gives, with $D=s^2-k^2$,

$$
2kh(1-R)+DQ=0,\qquad D(1+R)+2ksQ=0.
$$

Eliminating $Q$ gives

$$
\boxed{R=\frac{4k^2hs-D^2}{4k^2hs+D^2}.}
$$

There is no reflected P wave precisely when $4k^2hs=D^2$. If $\beta=c_S^2/c_P^2$ and $\sigma=k^2c_S^2/\omega^2=\beta\sin^2\theta$, then $h=(\omega/c_S)\sqrt{\beta-\sigma}$, $s=(\omega/c_S)\sqrt{1-\sigma}$ and $D=(\omega^2/c_S^2)(1-2\sigma)$. Substitution proves

$$
\boxed{4\sigma\sqrt{1-\sigma}\sqrt{\beta-\sigma}=(1-2\sigma)^2.}
$$

The condition applies only to incidence angles in the physical range $0\leq\sigma\leq\beta$; it need not have a solution for every elastic-modulus ratio.

## ↑ Ancestors (10)

1. [38A](../38a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
