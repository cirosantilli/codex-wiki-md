<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Assume $X$ is a connected [compact Riemann surface](../../../../../compact-riemann-surface.md) of [geometric genus](../../../../../geometric-genus.md) $g\ge1$. Work first in $\operatorname{Pic}^{g-1}(X)$, translating back to the [Jacobian variety](../../../../../jacobian-variety.md) by tensoring with $\mathcal O_X(-(g-1)p_0)$ when desired. Put

$$
\Theta=W_{g-1}=\{L:\deg L=g-1,\ h^0(X,L)>0\}.
$$

This is the image of the [Abelian sum map](../../../../../abel-map-of-an-algebraic-curve.md) from $X^{(g-1)}$. The [Riemann singularity theorem](../../../../../riemann-singularity-theorem.md) asserts that this image is a reduced [Cartier divisor](../../../../../cartier-divisor-split.md) and that

$$
\boxed{\operatorname{mult}_L\Theta=h^0(X,L).}
$$

Here multiplicity means the order of a local defining equation in the [maximal ideal](../../../../../maximal-ideal.md) of the smooth ambient [Jacobian variety](../../../../../jacobian-variety.md). Consequently **the singular points are precisely the classes with at least two independent sections**. We will prove the multiplicity equality, including the nonvanishing of its proposed leading term.

Choose an effective [divisor](../../../../../divisor.md) $E$ of degree $n\ge g$, and a local holomorphic family $\mathcal L$ of degree-$g-1$ [line bundles](../../../../../line-bundle.md) about $L$ on $X\times U$, where $U$ is a small neighborhood in $\operatorname{Pic}^{g-1}(X)$. Such a family is obtained by varying the [Čech cocycles](../../../../../cech-cocycle-condition.md) of a [line bundle](../../../../../line-bundle.md). Since $\deg L'(E)>2g-2$ for all $L'\in U$, [Serre duality](../../../../../serre-duality.md) gives $H^1(L'(E))=0$; the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(L'(E))=n$. The [cohomology and base change for line bundles on a curve](../../../../../cohomology-and-base-change-for-line-bundles-on-a-curve.md) then identifies

$$
A=\pi_*\mathcal L(E),\qquad B=\pi_*(\mathcal L(E)|_E)
$$

as [vector bundles](../../../../../vector-bundle.md) of rank $n$. Evaluation defines a [matrix](../../../../../matrix.md) $M:A\to B$. For each $L'$, its exact sequence is

$$
0\longrightarrow H^0(L')\longrightarrow A_{L'}\xrightarrow{M(L')}B_{L'}\longrightarrow H^1(L')\longrightarrow0.
$$

Thus $f=\det M$ vanishes exactly on $\Theta$.

The function $f$ is not identically zero. To exhibit a degree-$g-1$ [line bundle](../../../../../line-bundle.md) with no section, choose $g$ distinct points $p_1,\ldots,p_g$ giving independent evaluation functionals on $H^0(K_X)$. Such points can be chosen successively because a nonzero [holomorphic differential form](../../../../../holomorphic-differential-form.md) cannot vanish everywhere. For $F=\sum p_i$, the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(\mathcal O_X(F))=1$. Choose $q$ outside $F$. The unique section of $\mathcal O_X(F)$ does not vanish at $q$, so $\mathcal O_X(F-q)$ has no section. Therefore the evaluation [determinant](../../../../../determinant.md) genuinely cuts out a hypersurface. Its support is irreducible, since it is the image of the irreducible [symmetric product of a curve](../../../../../symmetric-product-of-a-curve.md) $X^{(g-1)}$.

Fix now $L\in\Theta$, and put $r=h^0(L)=h^1(L)$, the equality following from the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md). The [matrix](../../../../../matrix.md) $M(L)$ has an invertible $(n-r)$ by $(n-r)$ block. After invertible holomorphic row and column operations, its local form is

$$
\begin{pmatrix}I_{n-r}&0\\0&N(x)\end{pmatrix},\qquad N(0)=0,
$$

where $N$ is $r$ by $r$. More explicitly, eliminate the invertible block by its [Schur complement](../../../../../schur-complement.md); the discarded [determinant](../../../../../determinant.md) is a holomorphic unit. Hence $f$ is a unit times $\det N$. Every entry of $N$ lies in the [maximal ideal](../../../../../maximal-ideal.md), so its order is at least $r$.

The linear term of $N$ is the cup-product map

$$
N_1(\xi):H^0(L)\longrightarrow H^1(L),\qquad s\longmapsto\xi\smile s,\quad\xi\in H^1(\mathcal O_X).
$$

To verify this, deform the transition functions as $g_{ij}(1+\varepsilon\xi_{ij})$ and try to lift a section $s$ to $s+\varepsilon s'$. Its first-order gluing equation has right side $\xi_{ij}s_j$, whose [Čech cohomology](../../../../../cech-cohomology.md) class is exactly the obstruction to the lift. The kernel-to-cokernel derivative of the evaluation [matrix](../../../../../matrix.md) gives that same obstruction. Under [Serre duality](../../../../../serre-duality.md), if $s_1,\ldots,s_r$ and $t_1,\ldots,t_r$ are bases of $H^0(L)$ and $H^0(K_X\otimes L^{-1})$, then

$$
(N_1(\xi))_{ji}=\langle\xi,s_it_j\rangle.
$$

We must show that this [matrix](../../../../../matrix.md) is invertible for some $\xi$; otherwise the lower bound on multiplicity would not be an equality.

For each of these two $r$-dimensional section spaces, there are $r$ distinct points with independent evaluations. Choose them successively, using a section in the remaining kernel to find the next point. The set of such $r$-tuples is a nonempty open subset of $X^r$. The two open sets intersect because $X^r$ is irreducible, and we may avoid their diagonals. Choose $q_1,\ldots,q_r$ in that intersection and trivialize $L$ and $K_X$ there. Both [matrices](../../../../../matrix.md)

$$
S_{ki}=s_i(q_k),\qquad T_{kj}=t_j(q_k)
$$

are invertible. Let $\xi\in H^0(K_X)^*=H^1(\mathcal O_X)$ be the sum of the evaluation functionals at these points, with any nonzero weights $c_k$. Then

$$
N_1(\xi)=T^t\operatorname{diag}(c_1,\ldots,c_r)S
$$

is invertible. It follows that the degree-$r$ polynomial $\det N_1$ is nonzero, so $\operatorname{ord}_L f=r$. This proves the needed [invertible cup-product direction for a line bundle on a curve](../../../../../invertible-cup-product-direction-for-a-line-bundle-on-a-curve.md) by an explicit construction.

We still need to identify this [determinant](../../../../../determinant.md) hypersurface with the reduced image, rather than a multiple of it. Choose $g-1$ distinct points imposing independent conditions on $H^0(K_X)$. For their sum $D$, the [Riemann-Roch theorem](../../../../../riemann-roch-theorem.md) gives $h^0(D)=h^0(K_X-D)=1$. At its class, the calculation above gives order one. The [determinant](../../../../../determinant.md) hypersurface has irreducible support, so its sole [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) coefficient is one everywhere. A local hypersurface in a smooth space with these [divisor on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md) coefficients is reduced. Thus it is exactly the reduced image $W_{g-1}$, and the multiplicity formula holds for that image itself.

The argument gives the useful additional description

$$
\boxed{\text{the tangent cone at }L\text{ is defined by }\det(\xi\smile-)=0.}
$$

For $r=1$, its nonzero linear equation is $\langle\xi,st\rangle=0$. This agrees with the [derivative of the Abelian sum map](../../../../../derivative-of-the-abelian-sum-map.md): if $\operatorname{div}(s)=D$, then $st$ is the unique [holomorphic differential form](../../../../../holomorphic-differential-form.md) vanishing along $D$. For $r\ge2$, the local equation has no linear term and the point is singular. When $g=1$, $W_0$ is the single trivial [line bundle](../../../../../line-bundle.md) in $\operatorname{Pic}^0(X)$, with multiplicity one; the argument includes this case using the empty effective [divisor](../../../../../divisor.md). In genus zero there is no $W_{g-1}$ of effective [divisors on an algebraic curve](../../../../../divisor-on-an-algebraic-curve.md), so that hypothesis is necessary.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
