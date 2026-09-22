<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $M$ for the mass parameter throughout; the PDF uses $m$ in its formulas and $M$ in the subsequent prose for the same quantity. Set $a=r_j>0$. The [Jaffe model](../../../../../../jaffe-model.md) density simplifies to

$$
\rho(r)=\frac{Ma}{4\pi r^2(r+a)^2}.
$$

Its enclosed [mass](../../../../../../mass.md) is

$$
M(r)=4\pi\int_0^r\rho(s)s^2\,ds=Ma\int_0^r\frac{ds}{(s+a)^2}=\boxed{\frac{Mr}{r+a}}.
$$

It tends to $M$ as $r\to\infty$, verifying the total mass. It tends to zero at the center, so the cusp carries no extra point mass.

Spherical symmetry gives $\Phi'(r)=GM(r)/r^2=GM/[r(r+a)]$. Integrating with $\Phi(\infty)=0$ gives

$$
\Phi(r)=-GM\int_r^\infty\frac{ds}{s(s+a)}=\boxed{\frac{GM}{a}\log\frac{r}{r+a}}.
$$

This also directly satisfies the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md): differentiating $r^2\Phi'=GMr/(r+a)$ gives $4\pi Gr^2\rho(r)$. The [circular speed](../../../../../../circular-speed.md) is

$$
\boxed{v_c^2(r)=r\Phi'(r)=\frac{GM}{r+a}.}
$$

For $r\ll a$, $v_c=\sqrt{GM/a}[1-r/(2a)+O((r/a)^2)]$ is approximately constant. For $r\gg a$, $v_c=\sqrt{GM/r}[1-a/(2r)+O((a/r)^2)]\propto r^{-1/2}$. Thus the finite-mass model has an inner nearly flat [galaxy rotation curve](../../../../../../galaxy-rotation-curve.md) and an outer Keplerian decline.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
