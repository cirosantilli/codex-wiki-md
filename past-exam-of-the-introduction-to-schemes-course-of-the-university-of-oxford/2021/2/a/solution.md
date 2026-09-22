<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**Constructing the subsheaf.** On an [integral scheme](../../../../integral-scheme.md), every nonempty [open subset](../../../../open-set.md) is an [irreducible topological space](../../../../irreducible-topological-space.md) and hence a [connected space](../../../../connected-space.md). A [locally constant function](../../../../locally-constant-function.md) from such an [open subset](../../../../open-set.md) to $F$ is constant. Thus the [constant sheaf](../../../../constant-sheaf.md) $\underline F$ has sections $F$ on every nonempty [open subset](../../../../open-set.md), and the [structure sheaf](../../../../structure-sheaf-of-a-scheme.md) embeds in it by restriction to the [generic point](../../../../generic-point.md). Empty members of the given [open cover](../../../../open-cover.md) may be discarded.

For every [open subset](../../../../open-set.md) $W\subseteq X$, define

$$
\mathcal L(W)=\{s\in\underline F(W):\ f_i s|_{W\cap U_i}\in\mathcal O_X(W\cap U_i)\text{ for every }i\}.
$$

This is a subsheaf of the [sheaf of modules](../../../../sheaf-of-modules-split.md) $\underline F$: its condition is local, and compatible sections glue in $\underline F$, with the regularity conditions gluing in $\mathcal O_X$. On $U_i\cap U_j$, the hypothesis says that $f_j/f_i$ is a section of the [sheaf of units of the structure sheaf](../../../../sheaf-of-units-of-the-structure-sheaf.md). Therefore multiplication by it preserves $\mathcal O_X$, and

$$
f_i^{-1}\mathcal O_X|_{U_i\cap U_j}=f_j^{-1}\mathcal O_X|_{U_i\cap U_j}.
$$

It follows that $\mathcal L|_{U_i}=f_i^{-1}\mathcal O_{U_i}$: the condition with index $i$ implies every other condition on an overlap, and the converse is part of the definition. Multiplication by $1/f_i$ is an [isomorphism](../../../../isomorphism.md) $\mathcal O_{U_i}\to\mathcal L|_{U_i}$, with inverse multiplication by $f_i$. Hence $\mathcal L$ is an [invertible sheaf](../../../../line-bundle.md), or equivalently a [line bundle](../../../../line-bundle.md), and

$$
\boxed{\mathcal L(U_i)=\mathcal O_X(U_i)\cdot\frac1{f_i}\subseteq F.}
$$

These local descriptions also give uniqueness as a subsheaf of $\underline F$. This construction is the [divisor line bundle](../../../../divisor-line-bundle.md) for the local rational equations $f_i$.

**The tensor product.** Refine the two [open covers](../../../../open-cover.md) to $W_{ij}=U_i\cap V_j$. The ratios

$$
\frac{f_i g_j}{f_{i'}g_{j'}}=\frac{f_i}{f_{i'}}\frac{g_j}{g_{j'}}
$$

are sections of the [sheaf of units of the structure sheaf](../../../../sheaf-of-units-of-the-structure-sheaf.md) on the corresponding overlaps, so the products give a [line bundle](../../../../line-bundle.md) $\mathcal M\subseteq\underline F$ by the construction just proved. Multiplication in $F$ defines a [sheaf morphism](../../../../morphism-of-sheaves.md)

$$
\mathcal L\otimes_{\mathcal O_X}\mathcal L'\longrightarrow\mathcal M.
$$

On each $W_{ij}$ it sends the local generator $(1/f_i)\otimes(1/g_j)$ to the local generator $1/(f_i g_j)$. It is thus an [isomorphism](../../../../isomorphism.md) on an [open cover](../../../../open-cover.md), and hence an [isomorphism](../../../../isomorphism.md) globally. In particular,

$$
\boxed{(U_i\cap V_j,f_i g_j)\text{ represents }\mathcal L\otimes_{\mathcal O_X}\mathcal L'.}
$$

**The sign for projective twists.** Write [homogeneous coordinates](../../../../homogeneous-coordinate.md) $[x_0:\cdots:x_n]$ on [projective space](../../../../projective-space-split.md) $\mathbb P^n_{\mathbb Z}$, and let $U_i=D_+(x_i)$ be its standard [affine open cover](../../../../affine-open-cover.md). For any [integer](../../../../integer-split.md) $m$, take the nonzero elements of the [function field](../../../../function-field-of-an-algebraic-variety.md)

$$
\boxed{f_i=\left(\frac{x_0}{x_i}\right)^m\in\mathbb Q(x_1/x_0,\ldots,x_n/x_0)^*,\qquad 0\leq i\leq n.}
$$

Their ratios are $f_i/f_j=(x_j/x_i)^m$, which are sections of the [sheaf of units of the structure sheaf](../../../../sheaf-of-units-of-the-structure-sheaf.md) on $U_i\cap U_j$, including when $m<0$. The [twisting sheaf on projective space](../../../../twisting-sheaf-on-projective-space.md) $\mathcal O(m)$ has local generator $x_i^m$ on $U_i$. Divide a rational section of $\mathcal O(m)$ by $x_0^m$ to embed it in the [constant sheaf](../../../../constant-sheaf.md) of the [function field](../../../../function-field-of-an-algebraic-variety.md); the local generator becomes $(x_i/x_0)^m=1/f_i$. This identifies the constructed [line bundle](../../../../line-bundle.md) with $\mathcal O(m)$ and fixes the sign explicitly.

For $n\geq1$, $\operatorname{Pic}(\mathbb P^n_{\mathbb Z})\cong\mathbb Z$, with generator $[\mathcal O(1)]$; the displayed data gives all its powers, with $\mathcal O(m)\otimes\mathcal O(r)\cong\mathcal O(m+r)$ by the product rule above. If $n=0$, [projective space](../../../../projective-space-split.md) is $\operatorname{Spec}\mathbb Z$, its [Picard group](../../../../picard-group.md) is zero, and the same formula gives only the trivial [line bundle](../../../../line-bundle.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the introduction to schemes course of the University of Oxford](../../../split.md)
5. [Introduction to schemes course of the University of Oxford](../../../../introduction-to-schemes-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
