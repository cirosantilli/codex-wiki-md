<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Take a finite presentation $T=\langle x_1,\ldots,x_r\mid R_1,\ldots,R_s\rangle$. For a [closed-manifold realization of a finitely presented fundamental group](../../../../../closed-manifold-realization-of-a-finitely-presented-fundamental-group.md), begin with a five-dimensional ball and attach $r$ one-handles, giving a compact oriented five-manifold $W_1$ with [fundamental group](../../../../../fundamental-group.md) the free group on the $x_i$. Represent the relators by disjoint embedded circles in its four-dimensional boundary. General position allows them to be embedded and disjoint, and their oriented normal bundles admit framings. Attach a two-handle along each such circle. The resulting compact five-manifold $W$ has

$$
\pi_1(W)=\langle x_1,\ldots,x_r\mid R_1,\ldots,R_s\rangle=T
$$

by the [Seifert-van Kampen theorem](../../../../../seifert-van-kampen-theorem.md). Now set $B=\partial W$. It is a compact connected smooth four-manifold without boundary. Turning this [handle decomposition](../../../../../handle-decomposition.md) upside down gives a relative handle decomposition of $(W,B)$ with handles of indices three, four and five only. Attaching such handles does not change the [fundamental group](../../../../../fundamental-group.md): there are no new one-handles or two-handle relations. Thus $\pi_1(B)\to\pi_1(W)$ is an isomorphism and

$$
\boxed{\pi_1(B)\cong T.}
$$

These are the differential-topological handle facts used in the construction; the dimension-five thickening ensures the boundary retains the prescribed [fundamental group](../../../../../fundamental-group.md).

Now assume $T$ finite. Choose any smooth [Riemannian metric](../../../../../riemannian-metric.md) on $B$ and lift it to its [universal cover](../../../../../universal-cover.md) $\widetilde B$. This cover is compact, since its degree is $|T|$, and simply connected. Its [deck transformations](../../../../../deck-transformation.md) give a free isometric $T$-action. For the two [Gassmann equivalent](../../../../../gassmann-equivalence.md) subgroups put

$$
M_i=U_i\backslash\widetilde B.
$$

Each is a closed [Riemannian manifold](../../../../../riemannian-manifold.md), and $\widetilde B$ is its simply connected universal cover, with [deck transformation group](../../../../../deck-transformation-group.md) $U_i$. Consequently $\pi_1(M_i)\cong U_i$.

Here is the complete spectral argument behind the [Sunada theorem](../../../../../sunada-theorem.md) in this situation. Each finite-dimensional upstairs [eigenspace](../../../../../eigenspace.md) $E_\lambda$ is a representation of $T$, because the action is isometric and commutes with the [Laplace-Beltrami operator](../../../../../laplace-beltrami-operator.md). Functions downstairs correspond exactly to invariant functions upstairs, so their multiplicities are $\dim E_\lambda^{U_i}$. Averaging the representation matrices over a subgroup is a projection onto its invariant subspace. Taking its [trace](../../../../../matrix-trace.md) gives

$$
\dim E_\lambda^{U_i}=\frac1{|U_i|}\sum_{u\in U_i}\chi_\lambda(u).
$$

The [character](../../../../../character-of-a-representation.md) $\chi_\lambda$ is constant on each [conjugacy class](../../../../../conjugacy-class.md) of $T$. [Gassmann equivalence](../../../../../gassmann-equivalence.md) means $|U_1\cap C|=|U_2\cap C|$ for every such class $C$; summing these equalities also gives $|U_1|=|U_2|$. The two averages are therefore equal for every $\lambda$. **The quotients are isospectral, with $\pi_1(M_i)\cong U_i$.**

If $U_2=tU_1t^{-1}$, the map $[x]_{U_1}\mapsto[tx]_{U_2}$ is well defined, invertible and isometric because $t$ acts by an [isometry](../../../../../isometry.md) upstairs. **Conjugate subgroups give isometric quotients.**

For an explicit example with different [fundamental groups](../../../../../fundamental-group.md), use the [order-sixteen Gassmann pair](../../../../../order-sixteen-gassmann-pair.md)

$$
H_1=C_4\times C_4,\qquad H_2=Q_8\times C_2.
$$

Embed each in $T=S_{16}$ by left multiplication on its own sixteen elements, identified with the same sixteen-point set. These [regular representations](../../../../../regular-representation.md) are faithful. Both groups have one identity element, three elements of order two, and twelve of order four: in $C_4^2$ the elements of order dividing two are precisely its four even-coordinate elements; in $Q_8\times C_2$ they are the four elements in $\{1,-1\}\times C_2$. Every remaining element has order four.

In a regular action, an order-$k$ element is a product of $16/k$ disjoint $k$-cycles. Thus each subgroup intersects the identity [conjugacy class](../../../../../conjugacy-class.md) of $S_{16}$ in one element, the class of type $2^8$ in three, the class of type $4^4$ in twelve, and every other class in zero. They are [Gassmann equivalent](../../../../../gassmann-equivalence.md). However $H_1$ is abelian and $H_2$ is nonabelian, so they are not isomorphic. Apply the preceding construction with [fundamental group](../../../../../fundamental-group.md) $S_{16}$ and these subgroups. It produces

$$
\boxed{\operatorname{Spec}(M_1)=\operatorname{Spec}(M_2),\qquad
\pi_1(M_1)\cong C_4^2\not\cong Q_8\times C_2\cong\pi_1(M_2).}
$$

In particular they cannot even be homeomorphic, and therefore cannot be isometric.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
