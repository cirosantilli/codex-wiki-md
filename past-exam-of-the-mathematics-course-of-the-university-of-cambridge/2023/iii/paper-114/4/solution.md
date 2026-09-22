<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An $R$-orientation of a rank-$r$ [vector bundle](../../../../../vector-bundle.md) $E\to B$ is a coherent choice of generator in

$$
H^r(E_b,E_b\setminus\{0\};R)
$$

for every fiber. Equivalently, it is a [Thom class](../../../../../thom-class.md) $u_E\in H^r(D(E),S(E);R)$ restricting to those generators. The [Euler class of a vector bundle](../../../../../euler-class-of-a-vector-bundle.md) is

$$
e(E)=s^*j^*u_E\in H^r(B;R),
$$

where $j:(D(E),\varnothing)\to(D(E),S(E))$ forgets the subspace and $s$ is the zero section.

The [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) is

$$
H^q(B;R)\xrightarrow{\sim}H^{q+r}(D(E),S(E);R),
\qquad a\longmapsto\pi^*a\smile u_E.
$$

Insert these isomorphisms into the long exact cohomology sequence of $(D(E),S(E))$ and use the deformation retraction $D(E)\simeq B$. This gives the [Gysin sequence of a sphere bundle](../../../../../gysin-sequence-of-a-sphere-bundle.md)

$$
\cdots\to H^{q-r}(B)
\xrightarrow{\smile e(E)}H^q(B)
\xrightarrow{\pi^*}H^q(S(E))
\to H^{q-r+1}(B)
\xrightarrow{\smile e(E)}H^{q+1}(B)\to\cdots.
$$

To verify the labelled maps, represent $a$ under the Thom isomorphism by $\pi^*a\smile u_E$. Its image in $H^*(D(E))$ pulls back along the zero section to

$$
a\smile s^*j^*u_E=a\smile e(E).
$$

Thus multiplication by the Euler class is exactly the map from relative to absolute cohomology in the pair sequence.

Now let $M^m\subset S^n$ and let $V$ be its tubular neighborhood. The normal bundle has rank $r=n-m$. With $\mathbb F_2$ coefficients it is automatically oriented. Since $n>2m+1$, one has $r>m+1$, so its Euler class lies above the dimension of $M$ and vanishes. The Gysin sequence consequently splits into short exact sequences of vector spaces and gives

$$
H^q(\partial V;\mathbb F_2)
\cong H^q(M;\mathbb F_2)\oplus H^{q-r+1}(M;\mathbb F_2).
$$

On the other hand, [Alexander duality](../../../../../alexander-duality.md) gives

$$
\widetilde H^q(S^n\setminus M;\mathbb F_2)
\cong\widetilde H_{n-q-1}(M;\mathbb F_2).
$$

Over the field $\mathbb F_2$, the latter is naturally dual to $\widetilde H^{n-q-1}(M;\mathbb F_2)$, which expresses the complement cohomology entirely in terms of that of $M$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
