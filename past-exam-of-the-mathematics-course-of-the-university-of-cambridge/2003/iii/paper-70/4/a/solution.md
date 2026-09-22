<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For [antiplane shear](../../../../../../antiplane-shear.md), the only nonzero infinitesimal [strains](../../../../../../strain.md) are $e_{13}=e_{31}=w_{,1}/2$ and $e_{23}=e_{32}=w_{,2}/2$. Their trace is zero. The isotropic constitutive law $\sigma_{ij}=\lambda_L e_{kk}\delta_{ij}+2\mu e_{ij}$ consequently gives

$$
\boxed{\sigma_{13}=\sigma_{31}=\mu w_{,1},\qquad
\sigma_{23}=\sigma_{32}=\mu w_{,2},}
$$

with every other component zero. The first two equations of motion vanish because the fields are independent of $x_3$. The third is $\rho w_{,tt}=\sigma_{31,1}+\sigma_{32,2}$, hence

$$
\boxed{\nabla^2w-\frac1{c^2}w_{,tt}=0,\qquad c^2=\mu/\rho.}
$$

The PDF omits the final equals-zero; this is the equation supplied by momentum balance.

For a steadily moving field put $x=x_1-Vt$ and $\beta=\sqrt{1-V^2/c^2}$. In the subsonic case $|V|<c$, the equation becomes $\beta^2w_{xx}+w_{x_2x_2}=0$. With $y=\beta x_2$ it reduces to $w_{xx}+w_{yy}=0$. Thus $w$ is a [harmonic function](../../../../../../harmonic-function.md) and, on a simply connected region, has a [harmonic conjugate](../../../../../../harmonic-conjugate.md); there is a [holomorphic function](../../../../../../holomorphic-function.md) $H(z)$ such that

$$
\boxed{w=\operatorname{Re}H(z),\qquad z=x+iy.}
$$

This is [steadily moving antiplane shear](../../../../../../steadily-moving-antiplane-shear.md). The representation is local on more general domains unless the conjugate's periods vanish. The subsonic condition is essential: at or above the shear-wave speed the coordinate rescaling is degenerate or the equation is hyperbolic rather than this elliptic harmonic problem.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
