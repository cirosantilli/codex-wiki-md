<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Here $k$ is algebraically closed and $C$ is a connected [smooth projective curve](../../../../../smooth-projective-curve.md). For a [scheme](../../../../../scheme.md) $T$ over $k$, let $\pi:C_T=C\times_kT\to T$. The degree-$d$ [Picard functor of a curve](../../../../../picard-functor-of-a-curve.md) assigns

$$
\boxed{\operatorname{Pic}^d_C(T)=\{L\in\operatorname{Pic}(C_T):\deg(L|_{C_{\bar t}})=d\text{ for every geometric point }\bar t\}\big/\pi^*\operatorname{Pic}(T).}
$$

One can equivalently take the associated faithfully flat sheaf. It is essential to divide out by [line bundles](../../../../../line-bundle.md) from the base: a parameter space should remember the family on $C$, not an independent base line bundle.

Choose $p_0\in C(k)$. A class can be normalized as $L\otimes\pi^*(L|_{p_0\times T})^{-1}$, with its canonical trivialization along $p_0\times T$. Since $\pi_*\mathcal O_{C_T}=\mathcal O_T$, an automorphism of a [line bundle](../../../../../line-bundle.md) is multiplication by a base unit, and preserving this normalization forces that unit to be $1$. Descent of line bundles is effective, so normalized bundles satisfy the faithfully flat sheaf condition with no automorphism ambiguity. Thus this normalized description works on families, including nonreduced bases, rather than only on $k$-points.

We construct a representing scheme by [Picard charts from nonspecial divisors](../../../../../picard-charts-from-nonspecial-divisors.md). Fix $N\geq2g$ and put $r=N-g$. The [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md) $C^{(g)}$ represents [relative effective Cartier divisors on a curve](../../../../../relative-effective-cartier-divisor-on-a-curve.md) of degree $g$ and has a universal divisor $\Delta$. This uses the scheme symmetric product, not the naive set of unordered $T$-points. Locally on a smooth curve, a divisor of length $m$ is described by a monic polynomial in a smooth coordinate; its coefficients are elementary symmetric functions, so this construction includes coincident points in any characteristic. These local descriptions give the usual effective-divisor interpretation of the symmetric product.

Let $W\subset C^{(g)}$ be the open set where $H^1(C,\mathcal O(E))=0$. It is open by [semicontinuity theorem for coherent cohomology](../../../../../semicontinuity-theorem-for-coherent-cohomology.md). The [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(\mathcal O(E))=1$ there, so $E$ is the unique effective divisor in its line-bundle class. For every fixed effective divisor $B$ of degree $r$, take a copy $W_B$ of $W$, with family

$$
L_B=\mathcal O(B+\Delta)
$$

of degree $N$. Normalize it along $p_0$ as above.

This chart represents the open subfunctor defined by

$$
H^1(C,L_t(-B))=0.
$$

Indeed, for a family satisfying that condition, [cohomology and base change for line bundles on a curve](../../../../../cohomology-and-base-change-for-line-bundles-on-a-curve.md) makes $V=\pi_*L(-B)$ a [line bundle](../../../../../line-bundle.md) on $T$, with formation commuting with base change. The rank is one by [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md). The evaluation map

$$
\pi^*V\longrightarrow L(-B)
$$

is a nonzero section on each fibre, up to the base twist. Its zero scheme is a [relative effective Cartier divisor on a curve](../../../../../relative-effective-cartier-divisor-on-a-curve.md) $E$ of degree $g$. To check the family assertion, source and target are flat over $T$ and the fibre maps are injections of line bundles on an integral curve, so their cokernel is flat over $T$. Their zeros are Cartier, and the zero scheme is proper with finite fibres of length $g$, hence finite flat of degree $g$. It therefore defines a unique map $T\to W_B$. Conversely this construction recovers the family $\mathcal O(B+E)$ modulo a base line bundle.

The base-change step controls infinitesimal families as well. Locally, a finite free complex computes the two cohomology groups. Vanishing of its degree-one cokernel on fibres makes the last differential surjective by the [Nakayama lemma](../../../../../nakayama-lemma.md). Splitting that differential leaves a locally free degree-zero kernel of rank one and commutes with base change. This is the standard finite-complex form of the permitted cohomology semicontinuity and base-change results.

These chart subfunctors cover all degree-$N$ families. For a geometric-fibre [line bundle](../../../../../line-bundle.md) $L$ of degree $N$, the preceding solution gives $H^1(L)=0$ and $h^0(L)=N+1-g=r+1$. Choose $r$ points successively so that each imposes one independent condition on the current section space. At each stage that space is nonzero; a nonzero section has finitely many zeros, so a point outside its zero set can be chosen, also outside the finitely many previously chosen points. For their sum $B$,

$$
h^0(L(-B))=1,\qquad\deg L(-B)=g,
$$

and [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) forces $h^1(L(-B))=0$. The points may be chosen in $C(k)$ even when the fibre field extends $k$, since $C(k)$ is infinite and a nonzero section on the base-changed curve has only finitely many zeros. Thus fixed divisors $B$ defined over $k$ suffice. Upper semicontinuity gives an open neighbourhood on the base for each successful $B$.

It remains to glue the charts explicitly. On $W_B$, the locus

$$
W_{BB'}=\{E:H^1(C,\mathcal O(B+E-B'))=0\}
$$

is open. The line bundle inside the braces has degree $g$; its unique section up to scale has an effective zero divisor $E'$. Base change and the evaluation construction make $E\mapsto E'$ a morphism $W_{BB'}\to W_{B'}$. It satisfies $\mathcal O(B+E)\cong\mathcal O(B'+E')$. Reversing $B,B'$ gives its inverse. On triple overlaps the transition maps compose correctly because the residual effective divisor is unique. Hence the copies $W_B$ glue along these open isomorphisms to a [scheme](../../../../../scheme.md) $P^N$.

The normalized bundles $L_B$ glue as well: on overlaps their normalized isomorphisms exist and are unique, so they satisfy the cocycle condition. Let $\mathcal P_N$ denote the resulting universal normalized [line bundle](../../../../../line-bundle.md) on $C\times P^N$. For any $T$, the open cover where the conditions for some $B$ hold gives compatible maps $T\to W_B$, and thus a unique map $T\to P^N$. Pulling back $\mathcal P_N$ reverses this procedure. We have established a natural bijection

$$
\boxed{\operatorname{Hom}_k(T,P^N)\cong\operatorname{Pic}^N_C(T).}
$$

This proves representability of the full functor, not just a parametrization of individual line bundles. The nonspecial-divisor construction is also recorded in [Stacks Project, Picard scheme of a curve](https://stacks.math.columbia.edu/tag/0B9R).

Finally tensoring by $\mathcal O_C((N-d)p_0)$ is a natural isomorphism $\operatorname{Pic}^d_C\to\operatorname{Pic}^N_C$ for every integer $d$. Transporting the universal bundle back constructs its degree-$d$ representative $P^d$, usually denoted $\operatorname{Pic}^d_{C/k}$. Thus **every degree component is represented**. These identifications depend on the chosen point and twist; intrinsically the degree-zero component is a group scheme and each degree component is its torsor.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
