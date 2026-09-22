<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [J-holomorphic curve](../../../../../pseudoholomorphic-curve.md) is a map $u:(\Sigma,j)\to(X,J)$ from a [Riemann surface](../../../../../riemann-surfaces.md) satisfying $du\circ j=J\circ du$. The target [almost complex structure](../../../../../almost-complex-manifold.md) need not be integrable; the equation still behaves like a nonlinear elliptic version of complex analysis. On a [symplectic manifold](../../../../../symplectic-manifold.md) it is particularly effective when $J$ is compatible with $\omega$, because complex analysis then controls [symplectic area](../../../../../symplectic-area.md). The metric construction above supplies such structures and deformations between them.

In conformal coordinates $(s,t)$ with $j\partial_s=\partial_t$, the equation is $u_t=Ju_s$. With $g=\omega(\cdot,J\cdot)$, an arbitrary map satisfies

$$
\frac12(|u_s|^2+|u_t|^2)
=\omega(u_s,u_t)+\frac12|u_t-Ju_s|^2.
$$

This follows by expanding the last square and using $g(Ju_s,u_t)=\omega(u_s,u_t)$. Integrating proves the [Energy identity for a J-holomorphic curve](../../../../../energy-identity-for-a-j-holomorphic-curve.md). In particular,

$$
E(u)=\int_\Sigma u^*\omega
$$

for a [J-holomorphic curve](../../../../../pseudoholomorphic-curve.md), and its energy depends only on its [homology class](../../../../../homology-class.md) when the domain is closed. A nonconstant such curve has strictly positive area: its derivative is nonzero somewhere and positivity holds on a neighborhood. It also minimizes energy among maps in the same [homology class](../../../../../homology-class.md) with the same domain [conformal structure](../../../../../conformal-structure.md). Thus analytic bounds can be obtained from topological information.

The equation is the zero set of the [Cauchy–Riemann operator](../../../../../cauchy-riemann-operator.md) $\bar\partial_Ju=\tfrac12(du+J\circ du\circ j)$. Linearization at a solution, with respect to a connection, has the form

$$
D_u\xi=\tfrac12\bigl(\nabla\xi+J\nabla\xi\circ j+(\nabla_\xi J)du\circ j\bigr).
$$

The last term has differential order zero. The principal part has the Cauchy–Riemann symbol; in a complex frame a nonzero real covector $(a,b)$ gives multiplication by $a+ib$, an invertible symbol. This establishes ellipticity. On a closed domain the resulting operator between suitable [Sobolev spaces](../../../../../sobolev-space-split.md) is a [Fredholm operator](../../../../../fredholm-operator.md). The [Riemann-Roch index for a real Cauchy-Riemann operator](../../../../../riemann-roch-index-for-a-real-cauchy-riemann-operator.md) is $2n(1-g)+2c_1(A)$ for a fixed genus-$g$ domain, where $2n=\dim X$ and $A=u_*[\Sigma]$. For spheres, removing the six real dimensions of domain reparametrization gives

$$
\dim\mathcal M_A=2n+2c_1(A)-6,
$$

provided the curve is simple and regular. Each marked point adds two real dimensions; constraining its image to a specified target point removes $2n$. These are the [dimension formula for regular J-holomorphic spheres](../../../../../dimension-formula-for-regular-j-holomorphic-spheres.md) and its incidence version.

Here regular means that $D_u$ is [surjective](../../../../../surjective-function.md). Then the [implicit function theorem](../../../../../implicit-function-theorem.md) makes the [moduli space](../../../../../moduli-space.md) locally smooth of this index. The [generic transversality for simple holomorphic spheres](../../../../../generic-transversality-for-simple-holomorphic-spheres.md) theorem asserts that a residual set of smooth compatible $J$ makes all simple spheres in specified countably many classes regular, and that generic incidence constraints and generic one-parameter deformations are transverse. It does not assert regularity for all multiple covers. This distinction matters whenever one tries to count curves. A primitive class with no positive-area spherical decomposition avoids multiple-cover and bubbling difficulties and permits especially direct counts.

The other central ingredient is [Gromov compactness for spheres](../../../../../gromov-compactness-for-spheres.md). On a compact symplectic target, a sequence of holomorphic spheres with uniformly bounded area and smoothly converging tame [almost complex structures](../../../../../almost-complex-manifold.md) has a subsequence converging to a finite bubble tree, smoothly away from finitely many domain points after reparametrizations. The areas and [homology classes](../../../../../homology-class.md) of the nonconstant components add to those of the original maps; constant components account for stable marked configurations. This is [compactness](../../../../../compact-space.md) of stable maps, not ordinary smooth [compactness](../../../../../compact-space.md) of the original parametrizations.

The proof mechanism explains why bubbling is indispensable. An elliptic small-energy estimate bounds derivatives on a smaller disc when the energy on a larger disc is sufficiently small. Failure of a derivative bound therefore concentrates a definite amount of energy. Rescale near a point of large derivative; elliptic estimates yield a nonconstant limiting holomorphic map on the plane. Its finite energy allows the point at infinity to be filled in by the [removal of a finite-energy holomorphic puncture](../../../../../removal-of-a-finite-energy-holomorphic-puncture.md) theorem, producing a sphere. Repeating extracts further spheres. Uniform local monotonicity gives a positive energy threshold for nonconstant bubbles on the compact target, so only finitely many can occur. Estimates on the intervening annuli yield the energy identity and exclude lost neck energy. These statements give the analytic content behind the [compactness](../../../../../compact-space.md) theorem, while identifying the exact place where a smooth limit alone fails.

A local area estimate turns this existence theory into an embedding obstruction. In a standard complex ball, holomorphic curves are calibrated by the standard [symplectic form](../../../../../symplectic-form.md), so their parametrized [symplectic area](../../../../../symplectic-area.md) is their Riemannian area. They are stationary [minimal surfaces](../../../../../minimal-surface.md). The minimal-surface monotonicity formula says that $\operatorname{area}(C\cap B(\rho))/\rho^2$ is nondecreasing wherever the curve has no boundary in the ball. At a point of multiplicity $m$, its limiting density is $m\pi$. Consequently any branch through the centre contributes at least $\pi\rho^2$. For a general compatible $J$ there is still a local lower bound $c\rho^2$, with $c>0$ depending on controlled geometry. The exact Euclidean constant is the one needed for sharp radius obstructions.

Here is a global existence argument that feeds this estimate. Put

$$
Y=S^2(a)\times T^{2n-2},\qquad F=[S^2\times\{q\}],
$$

with the product [symplectic form](../../../../../symplectic-form.md), sphere area $a$, and a constant [symplectic form](../../../../../symplectic-form.md) on the [torus](../../../../../torus.md). Since the [torus](../../../../../torus.md) has zero second [homotopy group](../../../../../homotopy-group.md), every spherical class is $kF$ for an integer $k$. A nonconstant holomorphic sphere in this class has area $ka>0$, so $k\geq1$. A curve of class $F$ cannot split into two nonconstant bubbles, and it cannot be a nontrivial multiple cover. This supplies the [compactness](../../../../../compact-space.md) required for [fibre spheres in a sphere-torus product](../../../../../fibre-spheres-in-a-sphere-torus-product.md).

For the product [complex structure](../../../../../complex-structure.md), every sphere of class $F$ has constant [torus](../../../../../torus.md) projection: it lifts to a holomorphic map from the sphere to $\mathbb C^{n-1}$, whose coordinates are constant. Its sphere projection has degree one. Thus, up to reparametrization, there is exactly one such sphere through every target point. It is regular because its pulled-back [tangent bundle](../../../../../tangent-bundle.md) is $\mathcal O(2)\oplus\mathcal O^{n-1}$ on $\mathbb{CP}^1$, and the first [cohomology](../../../../../cohomology-split.md) of each summand vanishes. Its linearized [Dolbeault operator](../../../../../dolbeault-operator.md) therefore has zero [cokernel](../../../../../cokernel.md).

Since $c_1(F)=2$, the [moduli space](../../../../../moduli-space.md) with one marked point has expected real dimension $2n$. Imposing passage through a fixed point gives dimension zero. For generic structures and transverse incidence conditions this is a finite set. Along a generic path of structures its one-point solutions form a compact one-dimensional cobordism: [compactness](../../../../../compact-space.md) holds because splitting and multiple covers were excluded. Its boundary contains the endpoint solutions. A compact one-manifold has an even number of boundary points, so the count modulo two is unchanged. The product count is one, and hence the count for a generic compatible $J$ is one as well. If the endpoint product structure is not generic for other classes, its regular solutions allow the path argument in this single class. Approximating an arbitrary compatible $J$ by generic structures and applying [compactness](../../../../../compact-space.md) supplies a limiting sphere of class $F$ through the prescribed point. The nonconstant component still contains that point; there are no nonconstant bubbles to carry it away. This derives the existence assertion needed below without assuming a capacity obstruction.

Now suppose a [symplectic embedding](../../../../../symplectic-embedding.md) sends $B^{2n}(r)$ into the [symplectic cylinder](../../../../../symplectic-cylinder.md) $B^2(R)\times\mathbb R^{2n-2}$. Choose $0<\rho<\rho'<r$. The image of the closed radius-$\rho'$ ball is compact. For any $a>\pi R^2$, the first factor embeds symplectically into an area-$a$ sphere: in dimension two this is an area-preserving disc chart, leaving a cap of area $a-\pi R^2$. Enclose the remaining compact coordinate projection in a sufficiently large rectangular fundamental domain of a symplectic [torus](../../../../../torus.md). The compact ball image thereby embeds into $S^2(a)\times T^{2n-2}$.

Choose a compatible $J$ agreeing with the transported standard [complex structure](../../../../../complex-structure.md) near the radius-$\rho$ ball, by extending its associated metric and applying the polar construction. The sphere of class $F$ through the centre has area $a$. It cannot be contained in the ball image, where the [symplectic form](../../../../../symplectic-form.md) is exact. Euclidean monotonicity therefore gives $a\geq\pi\rho^2$. The choices of $a>\pi R^2$ and $\rho<r$ were arbitrary, so

$$
\boxed{B^{2n}(r)\hookrightarrow B^2(R)\times\mathbb R^{2n-2}\text{ symplectically}\quad\Longrightarrow\quad r\leq R.}
$$

For $n=1$ the same conclusion is simply area comparison; for $n\geq2$ the cylinder has infinite volume, so this proof detects a restriction that volume misses. This is the [Gromov non-squeezing theorem](../../../../../non-squeezing-theorem.md), derived from the curve existence and sharp area estimates above.

The associated [Gromov width](../../../../../gromov-width.md) is

$$
c_G(U,\omega)=\sup\{\pi r^2:B^{2n}(r)\text{ admits a symplectic embedding into }(U,\omega)\}.
$$

Composition of embeddings proves monotonicity. Rescaling coordinates in a ball proves $c_G(U,c\omega)=c\,c_G(U,\omega)$ for $c>0$. Non-squeezing, together with the evident inclusions, gives

$$
\boxed{c_G(B^{2n}(R))=c_G(B^2(R)\times\mathbb R^{2n-2})=\pi R^2.}
$$

These are the normalization, monotonicity and conformality properties of a [symplectic capacity](../../../../../symplectic-capacity.md). The two-ball obstruction of Question 5 illustrates a related use: one degree-one curve through two prescribed centres gives an additive area bound, stronger than comparing the volumes of the balls. The common method is to arrange standard complex geometry in the region one wants to measure, obtain a global holomorphic curve by deformation and [compactness](../../../../../compact-space.md), and compare its globally fixed area with local monotonicity lower bounds.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
