<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The ordinary [Poincare duality](../../../../../poincare-duality.md) statement here is for a compact [manifold](../../../../../topological-manifold.md) without boundary, of dimension $d$, oriented over the [field](../../../../../field.md) $F$. Its [fundamental class](../../../../../fundamental-class.md) $[M]_F$ induces [isomorphisms](../../../../../isomorphism.md)

$$
H^q(M;F)\xrightarrow{\ a\mapsto[M]_F\frown a\ }H_{d-q}(M;F)
$$

for every $q$. For a [manifold](../../../../../topological-manifold.md) with boundary the appropriate statement is [Poincare-Lefschetz duality](../../../../../lefschetz-duality.md) with relative groups; the ordinary pairing need not be nondegenerate. Over a [field](../../../../../field.md), the [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) identifies $H^{d-q}(M;F)$ with the full dual of $H_{d-q}(M;F)$. The cap-cup evaluation identity and duality therefore make

$$
H^q(M;F)\times H^{d-q}(M;F)\longrightarrow F,\qquad (a,b)\longmapsto\langle a\smile b,[M]_F\rangle
$$

a [perfect pairing](../../../../../perfect-pairing.md). Explicitly, a nonzero $a$ has a nonzero [cap product](../../../../../cap-product.md), and a linear functional $b$ on its [homology group](../../../../../homology-group.md) takes a nonzero value on that product. The same argument in the other variable proves nonsingularity. On the whole graded [cohomology](../../../../../cohomology-split.md), define $B(a,b)$ by taking the degree-$d$ part of $a\smile b$ before evaluation. For a nonzero component $a_q$ choose $b$ homogeneous of degree $d-q$ to pair nontrivially with it. All other components contribute zero in degree $d$. This proves that the [Poincare duality pairing](../../../../../poincare-duality-pairing.md) is a [nondegenerate bilinear form](../../../../../nondegenerate-bilinear-form.md) on $H^*(M;F)$; it need not be symmetric on all degrees.

Put $r=2n+1$, so $r$ is positive and odd, and orient each $S^r\times S^r$ by its product [orientation](../../../../../orientation-of-a-simplex.md). The [Künneth theorem](../../../../../kunneth-theorem.md) gives [integral cohomology](../../../../../integral-cohomology.md) $\mathbb Z$ in degrees zero and $2r$, $\mathbb Z^2$ in degree $r$, and zero elsewhere. Its two degree-$r$ generators $\alpha,\beta$ have $\alpha^2=\beta^2=0$, $\alpha\beta$ equal to its top [orientation class](../../../../../fundamental-class.md), and $\beta\alpha=-\alpha\beta$.

For a [connected sum of oriented manifolds](../../../../../connected-sum-of-oriented-manifolds.md), [excision](../../../../../excision-theorem.md) and the long [exact sequence](../../../../../exact-sequence.md) for deleting a ball show that deleting a ball removes the top [homology](../../../../../homology-split.md) class and leaves all lower positive [homology groups](../../../../../homology-group.md) unchanged. The boundary [sphere](../../../../../sphere.md) represents zero in the punctured [manifold](../../../../../topological-manifold.md): it is the boundary of its relative fundamental chain. In the [Mayer–Vietoris sequence](../../../../../mayer-vietoris-sequence.md) for the two punctured pieces joined along the separating [sphere](../../../../../sphere.md), the [orientation class](../../../../../fundamental-class.md) of the connected sum maps onto that [sphere](../../../../../sphere.md)'s class. The intermediate positive groups are consequently the [direct sums](../../../../../direct-sum.md) of the groups of the two original [manifolds](../../../../../topological-manifold.md). This also covers $r=1$, where the [sphere](../../../../../sphere.md) is a [circle](../../../../../circle.md) and the boundary-class observation is necessary in the middle degree. Iterating and applying the [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) gives

$$
\boxed{H^q(W_g;\mathbb Z)\cong\begin{cases}\mathbb Z,&q=0,2r,\\\mathbb Z^{2g},&q=r,\\0,&\text{otherwise}.\end{cases}}
$$

Here $g\geq1$; under the conventional extension $W_0=S^{2r}$ the same formula holds with a zero middle group.

Let $\omega$ be the top cohomological [orientation class](../../../../../fundamental-class.md). The connected-sum [pinch map](../../../../../pinch-map.md) to the wedge of the $g$ [sphere](../../../../../sphere.md) products gives degree-one projections to each summand. Pull back the two factor classes from summand $i$ to obtain $\alpha_i,\beta_i$. Their product is $\omega$, since the projection has degree one. Classes from different wedge summands have zero positive-degree [cup products](../../../../../cup-product.md), and [graded commutativity of the cup product](../../../../../graded-commutativity-of-the-cup-product.md) supplies the reversed sign. Thus the full [cohomology ring of a connected sum of odd-dimensional sphere products](../../../../../cohomology-ring-of-a-connected-sum-of-odd-dimensional-sphere-products.md) is the graded [free abelian group](../../../../../free-abelian-group.md) just displayed with multiplication

$$
\boxed{\alpha_i\alpha_j=\beta_i\beta_j=0,\qquad \alpha_i\beta_j=\delta_{ij}\omega,\qquad \beta_j\alpha_i=-\delta_{ij}\omega.}
$$

The unit is $1$, and $\omega$ times any positive-degree class is zero by dimension. This describes all products, including $\omega^2=0$.

The smooth [involution](../../../../../involution.md) is a [diffeomorphism](../../../../../diffeomorphism.md), since it is its own inverse. Its fixed set is closed; discreteness and compactness therefore make it finite. The supplied positivity of $\det(I-Df_x)$ makes every fixed point nondegenerate with local index $+1$. The [Lefschetz-Hopf fixed-point theorem](../../../../../lefschetz-hopf-fixed-point-theorem.md) then gives

$$
\#\operatorname{Fix}(f)=L(f)=2-\operatorname{tr}T,\qquad T=f^*:H^r(W_g;\mathbb R)\to H^r(W_g;\mathbb R).
$$

Indeed the degree-zero and top-degree traces are both one, because the [manifold](../../../../../topological-manifold.md) is connected and $f$ preserves its [orientation](../../../../../orientation-of-a-simplex.md); the middle degree is odd.

On $V=H^r(W_g;\mathbb R)$, the form $\Omega(a,b)=\langle a\smile b,[W_g]\rangle$ is a nondegenerate [alternating bilinear form](../../../../../alternating-bilinear-form.md) by [Poincare duality](../../../../../poincare-duality.md) and the oddness of $r$. Thus it is a [symplectic vector space](../../../../../symplectic-vector-space.md) of dimension $2g$. Naturality and [orientation](../../../../../orientation-of-a-simplex.md) preservation show that $T$ preserves $\Omega$, and $T^2=I$. For the [eigenspaces of a symplectic involution](../../../../../eigenspaces-of-a-symplectic-involution.md), write $V=V_+\oplus V_-$: the polynomial $(t-1)(t+1)$ has distinct roots over $\mathbb R$. If $v_+\in V_+$ and $v_-\in V_-$, then $\Omega(v_+,v_-)=\Omega(Tv_+,Tv_-)=-\Omega(v_+,v_-)$, so the two [vector subspaces](../../../../../vector-subspace.md) are orthogonal. Each restricted form is nondegenerate, since a vector annihilating its own [vector subspace](../../../../../vector-subspace.md) also annihilates the other and hence all of $V$. Their dimensions are therefore even, say $\dim V_+=2a$, $\dim V_-=2b$, with $a+b=g$. Consequently

$$
\operatorname{tr}T=2a-2b=2g-4b,\qquad \#\operatorname{Fix}(f)=2-2g+4b.
$$

This proves the [fixed-point congruence for an involution on an odd-sphere connected sum](../../../../../fixed-point-congruence-for-an-involution-on-an-odd-sphere-connected-sum.md):

$$
\boxed{\#\operatorname{Fix}(f)\equiv2-2g\pmod4.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 114](../../paper-114-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
