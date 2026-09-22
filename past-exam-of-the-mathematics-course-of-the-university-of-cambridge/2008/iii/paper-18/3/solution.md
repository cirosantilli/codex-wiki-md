<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For singular cochains $a\in C^p(X;R)$ and $b\in C^q(X;R)$, define the [cup product](../../../../../cup-product.md) on a singular $(p+q)$-simplex by

$$
(a\smile b)(\sigma)=a(\sigma|[v_0,\ldots,v_p])\,b(\sigma|[v_p,\ldots,v_{p+q}]).
$$

The identity $\delta(a\smile b)=\delta a\smile b+(-1)^pa\smile\delta b$ makes this descend to cohomology. The induced product is associative, unital and graded-commutative: $ab=(-1)^{pq}ba$ in degrees $p,q$.

For finite [CW complexes](../../../../../cw-complex.md), the [integral cohomological Künneth theorem for finite cell complexes](../../../../../integral-cohomological-kunneth-theorem-for-finite-cell-complexes.md) is the split short exact sequence

$$
0\longrightarrow\bigoplus_{p+q=n}H^p(X;\mathbb Z)\otimes H^q(Y;\mathbb Z)\xrightarrow{\times}H^n(X\times Y;\mathbb Z)\longrightarrow\bigoplus_{p+q=n+1}\operatorname{Tor}_1^{\mathbb Z}(H^p(X;\mathbb Z),H^q(Y;\mathbb Z))\longrightarrow0.
$$

The splitting need not be natural. If the factor cohomology is torsion-free, the [cohomological cross product](../../../../../cohomological-cross-product.md) is an isomorphism, with multiplication $(a\times b)(c\times d)=(-1)^{|b||c|}ac\times bd$.

A genus-$g$ closed oriented surface has cellular groups $H^0=\mathbb Z$, $H^1=\mathbb Z^{2g}$, $H^2=\mathbb Z$, and no higher cohomology. Choose the positive orientation class $\omega$ and a symplectic basis $a_i,b_i$ of $H^1$. The [cohomology ring of a closed oriented surface](../../../../../cohomology-ring-of-a-closed-oriented-surface.md) is specified by

$$
\boxed{a_ia_j=b_ib_j=0,\qquad a_ib_j=\delta_{ij}\omega,\qquad b_ia_j=-\delta_{ij}\omega,\qquad \omega H^{>0}=0,}
$$

with unit $1\in H^0$. These products follow by representing their [Poincare duality](../../../../../poincare-duality.md) classes by oriented handle curves: the $i$th meridian meets the $i$th longitude once positively, curves on distinct handles have zero intersection, and swapping two oriented curves reverses the intersection sign. In general, for closed oriented $n$-manifolds and transverse oriented submanifolds of codimensions $p,q$, the [cup product](../../../../../cup-product.md) of their Poincare-dual classes is the dual class of their oriented intersection. Complementary-dimensional intersections give the signed point count $\langle\alpha\beta,[M]\rangle$.

For $\Sigma_2$, the four curves $A_1,B_1,A_2,B_2$ give $a_1b_1=a_2b_2=\omega$ and all other pairings zero apart from their negatives in reversed order. Thus the degree-one [intersection pairing on an oriented surface](../../../../../intersection-pairing-on-an-oriented-surface.md) is two symplectic blocks, and the point class is dual to $\omega$.

For $\Sigma_2\times\Sigma_2$, let $a_i,b_i,\omega_1$ come from the first factor and $c_j,d_j,\omega_2$ from the second. The [Künneth theorem](../../../../../kunneth-theorem.md) gives their graded tensor-product ring, whose additive ranks in degrees $0,1,2,3,4$ are

$$
\boxed{(1,8,18,8,1).}
$$

The top orientation class is $\Omega=\omega_1\omega_2$. The two fiber surfaces $\{p\}\times\Sigma_2$ and $\Sigma_2\times\{q\}$ have dual classes $\omega_1,\omega_2$, intersect once positively and have zero self-intersection. The other sixteen degree-two classes are products of degree-one classes and are dual, up to the chosen orientation convention, to products of handle curves. Their intersections are encoded by

$$
\omega_1^2=\omega_2^2=0,\qquad (a_ic_j)(b_kd_l)=-\delta_{ik}\delta_{jl}\Omega,\qquad(a_id_j)(b_kc_l)=\delta_{ik}\delta_{jl}\Omega.
$$

The minus sign in the first mixed formula comes from commuting $c_j$ past $b_k$. These classes together with the fiber classes give the [intersection form of a product of two closed oriented surfaces](../../../../../intersection-form-of-a-product-of-two-closed-oriented-surfaces.md), here nine hyperbolic blocks. Complementary degrees one and three are similarly paired, for example $a_i(b_k\omega_2)=\delta_{ik}\Omega$; geometrically this pairs a three-dimensional product submanifold with a transverse loop. This exhibits the full duality, not just the additive groups.

The [Lefschetz fixed-point theorem](../../../../../lefschetz-fixed-point-theorem.md) says that a self-map of a compact polyhedron with nonzero [Lefschetz number](../../../../../lefschetz-number.md) has a fixed point, where $L(f)=\sum_q(-1)^q\operatorname{tr}(f_*:H_q(-;\mathbb Q)\to H_q(-;\mathbb Q))$. A map homotopic to the identity has $L(f)=\chi$, and [Euler characteristic of a product](../../../../../euler-characteristic-of-a-product.md) gives

$$
0=L(f)=(2-2g_1)(2-2g_2).
$$

Consequently

$$
\boxed{g_1=1\text{ or }g_2=1.}
$$

The product $g_1g_2$ itself is not determined by the printed assumptions. For every $h\geq0$, translation by a nonzero torus point, times the identity on $\Sigma_h$, is a fixed-point-free map of $\Sigma_1\times\Sigma_h$ homotopic to the identity, and its genus product is $h$. Thus the exact conclusion is the criterion for [fixed-point-free self-maps homotopic to the identity on products of surfaces](../../../../../fixed-point-free-self-maps-homotopic-to-the-identity-on-products-of-surfaces.md), rather than a single value of $g_1g_2$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
