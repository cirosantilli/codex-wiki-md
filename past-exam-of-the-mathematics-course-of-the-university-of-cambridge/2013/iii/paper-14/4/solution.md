<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Work first with coefficients $\mathbb F_2$. For a rank-$r$ real [vector bundle](../../../../../vector-bundle.md) $E\to B$ over a [CW complex](../../../../../cw-complex.md), choose a fibre metric and its [disk bundle](../../../../../disk-bundle.md) $D(E)$ and [sphere bundle](../../../../../sphere-bundle.md) $S(E)$. The mod-two [Thom class](../../../../../thom-class.md) is the unique class $U\in H^r(D(E),S(E);\mathbb F_2)$ restricting to the nonzero generator on every fibre pair. The [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) asserts that

$$
T:H^{j-r}(B;\mathbb F_2)\xrightarrow{\ \cong\ }H^j(D(E),S(E);\mathbb F_2),\qquad a\longmapsto\pi^*a\cup U.
$$

No orientation of the [vector bundle](../../../../../vector-bundle.md) is needed with these coefficients.

Let $j:H^*(D(E),S(E))\to H^*(D(E))$ forget the relative condition, and let $s:B\to D(E)$ be the zero section. Set $e_2(E)=s^*j(U)$, the top [Stiefel–Whitney class](../../../../../stiefel-whitney-class.md) $w_r(E)$. Since $D(E)$ retracts onto the zero section, $j(U)=\pi^*e_2(E)$. Thus the relative-to-absolute map corresponds under the [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) to multiplication by $e_2(E)$. Substituting these identifications into the [long exact sequence](../../../../../long-exact-sequence.md) in [relative cohomology](../../../../../relative-cohomology.md) of $(D(E),S(E))$ gives the [unoriented Gysin sequence](../../../../../unoriented-gysin-sequence.md)

$$
\cdots\longrightarrow H^{j-r}(B;\mathbb F_2)\xrightarrow{\cup e_2(E)}H^j(B;\mathbb F_2)\xrightarrow{p^*}H^j(S(E);\mathbb F_2)\longrightarrow H^{j-r+1}(B;\mathbb F_2)\xrightarrow{\cup e_2(E)}H^{j+1}(B;\mathbb F_2)\longrightarrow\cdots,
$$

where $p$ is the [sphere bundle](../../../../../sphere-bundle.md) projection.

Apply this to the [real tautological line bundle](../../../../../real-tautological-line-bundle.md) $\gamma_n\to\mathbb{RP}^n$. Its [sphere bundle](../../../../../sphere-bundle.md) is $S^n$, with projection the antipodal double cover, and put $t=e_2(\gamma_n)\in H^1(\mathbb{RP}^n;\mathbb F_2)$. Suppose $n\ge1$. The map on $H^0$ from the connected base to the connected sphere is an [isomorphism](../../../../../isomorphism.md), so exactness shows that multiplication by $t$ is injective from $H^0$ to $H^1$. Since both groups are one-dimensional, $t$ is a generator.

For $1<j<n$, the adjacent sphere [cohomology groups](../../../../../cohomology-group.md) in the [Gysin sequence](../../../../../gysin-sequence-of-a-sphere-bundle.md) vanish, so multiplication by $t$ is an [isomorphism](../../../../../isomorphism.md) from degree $j-1$ to degree $j$. If $n>1$, the top portion is

$$
0\longrightarrow H^{n-1}(\mathbb{RP}^n;\mathbb F_2)\xrightarrow{\cup t}H^n(\mathbb{RP}^n;\mathbb F_2)\longrightarrow H^n(S^n;\mathbb F_2)\longrightarrow H^n(\mathbb{RP}^n;\mathbb F_2)\longrightarrow0.
$$

The last nonzero arrow is surjective between one-dimensional groups, hence an [isomorphism](../../../../../isomorphism.md); the preceding arrow is zero, so multiplication by $t$ is again an [isomorphism](../../../../../isomorphism.md). For $n=1$ the earlier $H^0$ argument already gives the top multiplication. Thus $1,t,\ldots,t^n$ are the nonzero generators in their respective degrees, while $t^{n+1}=0$ by dimension. We obtain

$$
\boxed{H^*(\mathbb{RP}^n;\mathbb F_2)\cong\mathbb F_2[t]/(t^{n+1}),\qquad |t|=1.}
$$

For $n=0$ this says simply $H^*(\mathbb{RP}^0;\mathbb F_2)=\mathbb F_2$, with $t=0$. This computes the [mod-two cohomology ring of real projective space](../../../../../mod-two-cohomology-ring-of-real-projective-space.md), including its multiplication rather than only its additive groups.

Now use integral coefficients and an oriented rank-$n$ [vector bundle](../../../../../vector-bundle.md). Its orientation selects an integral [Thom class](../../../../../thom-class.md) $U$. Define its [Euler class](../../../../../euler-class-of-a-vector-bundle.md) by

$$
\boxed{e(E)=s^*j(U)\in H^n(B;\mathbb Z).}
$$

Again $j(U)=\pi^*e(E)$. The [cup product](../../../../../cup-product.md) of two relative classes in $H^*(D(E),S(E))$ agrees with the mixed relative/absolute product after forgetting the relative condition on either factor. Consequently

$$
\boxed{U\cup U=U\cup j(U)=U\cup\pi^*e(E).}
$$

This is the [cup square of a Thom class](../../../../../cup-square-of-a-thom-class.md). If $n$ is odd, [graded commutativity of the cup product](../../../../../graded-commutativity-of-the-cup-product.md) gives $U\cup U=-U\cup U$, hence $2U^2=0$. Since $U\cup\pi^*(2e(E))$ is, up to the graded sign, the [Thom isomorphism](../../../../../thom-isomorphism-theorem.md) image of $2e(E)$, its vanishing implies

$$
\boxed{2e(E)=0\qquad(n\text{ odd}).}
$$

Thus the [Euler class of an oriented odd-rank vector bundle is two-torsion](../../../../../euler-class-of-an-oriented-odd-rank-vector-bundle-is-two-torsion.md); the conclusion is integral and does not require the base [cohomology](../../../../../cohomology-split.md) to be torsion-free.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
