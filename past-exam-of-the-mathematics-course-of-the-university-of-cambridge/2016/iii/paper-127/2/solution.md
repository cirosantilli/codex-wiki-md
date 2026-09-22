<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Choose the [Hopf map](../../../../../hopf-map.md) $\eta$ and orientations so its [Hopf invariant](../../../../../hopf-invariant.md) is one. The [cellular cohomology](../../../../../cellular-cohomology.md) of $Y_d$ is $\mathbb Z$ in degrees $0,2,4$ and zero otherwise. Let $x,z$ be generators in degrees two and four. Precomposing $\eta$ with a degree-$d$ self-map of $S^3$ represents $d\eta$. The induced map of mapping cones is the identity on the two-cell and has degree $d$ on the four-cell. Since the Hopf mapping cone has cup square equal to its top generator, naturality of the [cup product](../../../../../cup-product.md) gives $x^2=dz$. Equivalently, [precomposition scales the Hopf invariant by degree](../../../../../precomposition-scales-the-hopf-invariant-by-degree.md). Hence

$$
\boxed{H^*(Y_d;\mathbb Z)=\mathbb Z[x,z]/(x^2-dz,xz,z^2),
\qquad |x|=2,\quad |z|=4}.
$$

The coefficient is $d$, not $d^2$: multiplication in $\pi_3(S^2)$ is being used, rather than postcomposition by a degree-$d$ map of the target sphere.

For $X=X_{d,f}$, the only nonzero cellular boundary is $C_4\to C_3$, multiplication by $f$. Thus its [cellular cohomology](../../../../../cellular-cohomology.md) gives

$$
H^q(X;\mathbb Z)=
\begin{cases}
\mathbb Z,&q=0,2,\\
\ker(f:\mathbb Z\to\mathbb Z),&q=3,\\
\mathbb Z/f\mathbb Z,&q=4,\\
0,&\text{otherwise}.
\end{cases}
$$

Let $x$ again generate $H^2$, and let $z$ be the class of the four-cell cochain. Collapsing the three-sphere gives a map $X\to Y_d$ which pulls the degree-two generator back to $x$ and the degree-four generator back to $z$. Hence $x^2=dz$, now interpreted modulo $f$. Every other product of positive-degree classes vanishes by dimension. This is the [cohomology ring of a Hopf attachment with a sphere summand](../../../../../cohomology-ring-of-a-hopf-attachment-with-a-sphere-summand.md). More explicitly, if $f\ne0$,

$$
\boxed{H^*(X;\mathbb Z)=\mathbb Z[x,z]/(fz,x^2-dz,xz,z^2)}.
$$

If $f=0$, there is additionally a generator $y$ of degree three, with $xy=y^2=yz=0$. The displayed description of the groups uses $\mathbb Z/0\mathbb Z=\mathbb Z$, so the zero case is included. In particular, a nonzero $f$ kills the degree-three cohomology but can leave torsion in degree four.

There are no one-cells, and attaching cells of dimension at least three does not change $\pi_1$. Thus $X$ is [simply connected](../../../../../simply-connected-space.md). The [Hurewicz theorem](../../../../../hurewicz-theorem.md) in degree two gives

$$
\boxed{\pi_1(X)=0,\qquad\pi_2(X)\cong H_2(X;\mathbb Z)\cong\mathbb Z}.
$$

To compute $\pi_3$, choose a map $g:X\to\mathbb{CP}^\infty=K(\mathbb Z,2)$ representing $x$. This [Eilenberg–MacLane space](../../../../../eilenberg-maclane-space.md) can be realized by the [classifying space](../../../../../classifying-space.md) of $S^1$. On $S^2$ the map is the standard inclusion; on $S^3$ it is constant, and it extends over the four-cell since $\pi_3(K(\mathbb Z,2))=0$. Its [homotopy fibre](../../../../../homotopy-fiber.md) $T$ is the pullback of the universal [circle bundle](../../../../../circle-bundle.md) $S^\infty\to\mathbb{CP}^\infty$. The map on $\pi_2$ is an isomorphism, so the [long exact sequence of homotopy groups of a fibration](../../../../../long-exact-sequence-of-homotopy-groups-of-a-fibration.md) gives $\pi_1(T)=\pi_2(T)=0$ and $\pi_3(T)\cong\pi_3(X)$. Therefore the [Hurewicz theorem](../../../../../hurewicz-theorem.md) identifies the latter with $H_3(T;\mathbb Z)$.

Over $W=S^2\vee S^3$, the circle-bundle total space is

$$
P=S^3\cup_{S^1}(S^1\times S^3).
$$

The first summand is the [Hopf fibration](../../../../../hopf-fibration.md) total space over $S^2$, and the second is the trivial bundle over $S^3$. Their intersection is the fibre over the wedge point. The [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) gives $H_3(P)=\mathbb Z A\oplus\mathbb Z B$, with generators from the two three-spheres. These are the lifts of $\eta_1$ and $i_2$. The circle bundle over $W$ also has a 2-connected total space, so lifting and the [Hurewicz theorem](../../../../../hurewicz-theorem.md) identify $d\eta_1+f i_2$ with $dA+fB$.

Over the attached four-disc the bundle is trivial. The resulting relative pair has the homology of $(S^1\times D^4,S^1\times S^3)$, so $H_4(T,P)=\mathbb Z$ and $H_3(T,P)=0$. Its boundary map sends a generator to the lift of the attaching map, namely $dA+fB$. The [long exact sequence in relative homology](../../../../../long-exact-sequence-in-relative-homology.md) now gives

$$
H_3(T)=\frac{\mathbb Z A\oplus\mathbb Z B}{\langle dA+fB\rangle}.
$$

Applying [Smith normal form](../../../../../smith-normal-form.md) to this one relation proves the [third homotopy group of a Hopf attachment with a sphere summand](../../../../../third-homotopy-group-of-a-hopf-attachment-with-a-sphere-summand.md):

$$
\boxed{\pi_3(X_{d,f})\cong\mathbb Z\oplus\mathbb Z/\gcd(d,f)\mathbb Z}.
$$

Since $d>0$, the greatest common divisor is positive even when $f=0$. This derivation uses the required map to an [Eilenberg–MacLane space](../../../../../eilenberg-maclane-space.md) and determines the extension, rather than merely the orders of its pieces.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 127](../../paper-127-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
