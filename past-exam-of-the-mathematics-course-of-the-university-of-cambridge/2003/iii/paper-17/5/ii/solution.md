<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define

$$
F:B^4(1)\longrightarrow\mathbb{CP}^2\setminus\{z_3=0\},\qquad
F(w_1,w_2)=[w_1:w_2:\sqrt{1-|w|^2}].
$$

Every projective point with $z_3\ne0$ has a unique unit representative whose third coordinate is positive real, so $F$ is a [diffeomorphism](../../../../../../diffeomorphism.md). More explicitly, in the affine coordinate $u=(z_1/z_3,z_2/z_3)$ its inverse is $w=u/\sqrt{1+|u|^2}$. Lift $F$ to the unit sphere by $\widetilde F(w)=(w,\sqrt{1-|w|^2})$. The last coordinate is real, so its contribution $dx_3\wedge dy_3$ pulls back to zero. The reduction identity therefore yields

$$
\boxed{F^*\Omega=\widetilde F^*\omega_{st}=\omega_{st}|_{\mathbb C^2}.}
$$

This proves the [symplectic ball chart in complex projective space](../../../../../../symplectic-ball-chart-in-complex-projective-space.md) directly, including the precise unit radius.

For the final unheaded request, embed the two disjoint balls in this chart. Fix arbitrary $0<\rho_i<r_i$, and choose intermediate radii $\rho_i<\rho_i'<r_i$. On the images of the balls of radius $\rho_i'$, transport the standard [complex structure](../../../../../../complex-structure.md) by the given [symplectic embeddings](../../../../../../symplectic-embedding.md). It is compatible with $\Omega$. Their smaller closed neighborhoods are compact and disjoint. Choose a global [Riemannian metric](../../../../../../riemannian-metric.md) agreeing there with the associated compatible metrics, using a [partition of unity](../../../../../../partition-of-unity.md) outside these neighborhoods, and apply the metric construction. The resulting global [compatible almost complex structure](../../../../../../compatible-almost-complex-structure.md) $J$ agrees with the transported standard structure on each ball of radius $\rho_i$ and on a slightly larger neighborhood. This extends metrics, rather than averaging [almost complex structures](../../../../../../almost-complex-manifold.md).

Let $p_1,p_2$ be the centres. They are distinct. The degree-one [J-holomorphic curve](../../../../../../pseudoholomorphic-curve.md) supplied in the question has total area $\pi$, because its [homology class](../../../../../../homology-class.md) is the projective line class. We use the sharp Euclidean version of the [Monotonicity theorem for a J-holomorphic curve](../../../../../../monotonicity-theorem-for-a-j-holomorphic-curve.md): a nonconstant holomorphic curve through the centre of a standard complex ball, with no boundary in the ball and counted with its parametrization multiplicities, has area in the radius-$\rho$ ball at least $\pi\rho^2$. This includes branched points: their density is a positive integer $m$, and the stronger lower bound is $m\pi\rho^2$. One way to see the constant is that complex curves are calibrated [minimal surfaces](../../../../../../minimal-surface.md); their stationary area ratio $\operatorname{area}(C\cap B(\rho))/\rho^2$ is nondecreasing and its limit at the centre is $m\pi$.

The closed degree-one curve cannot stay entirely inside either chart ball: there the form is exact, so [Stokes theorem](../../../../../../stokes-theorem.md) would give zero total area, contradicting its positive area. Thus the branch through each centre crosses the surrounding spheres, and the stated monotonicity bound applies to each restriction. The two ball images are disjoint, so their area contributions add without overlap. It follows that

$$
\pi\rho_1^2+\pi\rho_2^2\leq\int_C\Omega=\pi.
$$

Letting both smaller radii increase to their original radii gives

$$
\boxed{r_1^2+r_2^2\leq1.}
$$

This [two-ball packing obstruction in the projective plane](../../../../../../two-ball-packing-obstruction-in-the-projective-plane.md) is sharper than volume alone: a volume comparison would only give $r_1^4+r_2^4\leq1$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
