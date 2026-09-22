<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

In this context a [nowhere locally homogeneous metric](../../../../../nowhere-locally-homogeneous-metric.md), also called a bumpy metric, is a smooth [Riemannian metric](../../../../../riemannian-metric.md) for which no two distinct nonempty open subsets are isometric with their induced metrics. Equivalently every [local isometry](../../../../../local-isometry.md) between open subsets is the identity wherever defined: a nonidentity [local isometry](../../../../../local-isometry.md) sends some point $x$ to a distinct point, and restriction to sufficiently small disjoint neighborhoods would violate the first formulation. This is the local-isometry meaning of the terminology here; degeneracy of periodic [geodesics](../../../../../geodesic.md) is a different use of the word bumpy.

[Sunada's local isometry lemma](../../../../../sunada-local-isometry-lemma.md) states that on a compact smooth manifold without boundary of dimension $m\ge2$ the [nowhere locally homogeneous metrics](../../../../../nowhere-locally-homogeneous-metric.md) contain a [residual set](../../../../../residual-set.md) in the space of smooth [Riemannian metrics](../../../../../riemannian-metric.md) with its $C^\infty$ topology. In particular they are dense, by the [Baire category theorem](../../../../../baire-category-theorem.md). A [residual set](../../../../../residual-set.md) is a countable intersection of open dense sets. The dimension assumption matters: every one-dimensional [Riemannian metric](../../../../../riemannian-metric.md) is locally $ds^2$ in arclength coordinates and has local translations.

The [jet bundle of maps](../../../../../jet-bundle-of-maps.md) $J^k(M,N)$ consists of equivalence classes $j_x^kf$ of smooth maps near $x$, where two maps agree to order $k$ at $x$ in coordinate charts. Its projection to $M\times N$ sends $j_x^kf$ to $(x,f(x))$. For a [multi-index](../../../../../multi-index-notation.md) $\alpha$ in $m$ variables there are $\binom{m+r-1}{r}$ derivatives of order $r$. Thus a coordinate chart consists of the source point, the target point, and $n$ coefficients for every derivative order $1$ through $k$. Summing the counts gives

$$
\boxed{\dim J^k(M,N)=m+n\binom{m+k}{k},\qquad
\dim J^k_{x,y}(M,N)=n\left(\binom{m+k}{k}-1\right).}
$$

This includes $J^0(M,N)=M\times N$. The fibre over $(x,y)$ is the space of truncated Taylor maps with fixed constant term $y$, locally modeled on

$$
\bigoplus_{r=1}^k\operatorname{Sym}^r(T_x^*M)\otimes T_yN.
$$

For $k=1$ its identification with $\operatorname{Hom}(T_xM,T_yN)$ is canonical. For higher $k$, changes of target coordinates mix derivatives of different orders, so this is a coordinate or connection-dependent description, not a canonical vector-bundle identification. The truncation $J^k\to J^{k-1}$ is an [affine bundle](../../../../../affine-bundle.md) modeled on the pullback of $\operatorname{Sym}^k(T^*M)\otimes TN$ over $M\times N$.

For the density assertion put $A=\overline U_i$ and $B=\overline U_j$. **Their closures must be distinct**. If $A=B$, the identity is an [isometry](../../../../../isometry.md) for every [Riemannian metric](../../../../../riemannian-metric.md), and the requested complement is empty. Under the intended distinct-domain assumption, the smooth closed-ball hypothesis makes $A$ and $B$ regular closed domains, equal to the closures of their interiors. After interchanging them if necessary, there is a nonempty open set $W$ with compact closure in $\operatorname{int}(A)\setminus B$. Otherwise each interior would be contained in the other closure, forcing $A=B$.

Take any smooth [Riemannian metric](../../../../../riemannian-metric.md) $g$. If $\operatorname{vol}_g(A)\ne\operatorname{vol}_g(B)$, it already lies outside $\mathcal S_{ij}$, because an [isometry](../../../../../isometry.md) preserves the [Riemannian volume form](../../../../../riemannian-volume-form.md). If the volumes agree, choose a nonzero nonnegative smooth [bump function](../../../../../bump-function.md) $\eta$ supported in $W$ and set

$$
g_t=(1+t\eta)g\qquad(t>0).
$$

These are positive definite [Riemannian metrics](../../../../../riemannian-metric.md), they agree with $g$ on $B$, and $g_t\to g$ in $C^\infty$ as $t\downarrow0$, since every derivative of $g_t-g$ is $t$ times a fixed compactly supported smooth tensor. Their [Riemannian volume forms](../../../../../riemannian-volume-form.md) satisfy

$$
dV_{g_t}=(1+t\eta)^{m/2}dV_g.
$$

Hence $\operatorname{vol}_{g_t}(B)=\operatorname{vol}_g(B)$ whereas $\operatorname{vol}_{g_t}(A)>\operatorname{vol}_g(A)$ for every $t>0$. In particular

$$
\left.\frac{d}{dt}\right|_{t=0}\operatorname{vol}_{g_t}(A)=\frac m2\int_A\eta\,dV_g>0.
$$

The two domains cannot be isometric for $g_t$. Every $C^\infty$ neighborhood of $g$ therefore meets the complement of $\mathcal S_{ij}$, proving

$$
\boxed{\overline{\mathcal C\mathcal S_{ij}}=\operatorname{Met}^{\infty}(M)\quad\text{if }\overline U_i\ne\overline U_j.}
$$

This [localized volume perturbation](../../../../../localized-volume-perturbation.md) proves the requested density even when the two domains overlap, and works in every positive dimension. It does not by itself prove the stronger residual local-isometry statement: fixed isometric closures and arbitrary isometric open subsets are different conditions.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
