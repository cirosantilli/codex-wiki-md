<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Choose a contractible free $G$-space $EG$, with $BG=EG/G=K(G,1)$ the [classifying space of a discrete group](../../../../../classifying-space-of-a-discrete-group.md). The [Borel construction](../../../../../borel-construction.md) gives the fibration

$$
S^{n-1}\longrightarrow E=EG\times_GS^{n-1}\longrightarrow BG.
$$

Because the action on the sphere is free, the map $E\to S^{n-1}/G$ has contractible fibre $EG$ and is a [homotopy equivalence](../../../../../homotopy-equivalence.md). The quotient is a closed $(n-1)$-dimensional manifold, so $H^k(E;\mathbb F)=0$ for $k>n-1$.

The hypothesis on integral sphere cohomology makes the $G$-action on $H^{n-1}(S^{n-1};\mathbb F)$ trivial as well. Thus the [Serre spectral sequence](../../../../../serre-spectral-sequence.md) has just two rows, both copies of $H^*(BG;\mathbb F)$, in fibre degrees zero and $n-1$. If $u$ is the fibre generator, the only possible differential is $d_n$, and its [transgression](../../../../../transgression.md) defines

$$
\Delta=d_n(u)\in H^n(BG;\mathbb F).
$$

The multiplicative differential rule gives $d_n(a u)=(-1)^{|a|}a\smile\Delta$. Up to the graded sign, this is multiplication by $\Delta$. For $i>0$, the terms $E_\infty^{i,n-1}$ and $E_\infty^{i+n,0}$ must both vanish because their total degrees exceed $n-1$. The first vanishing says the relevant multiplication map has zero [kernel](../../../../../kernel-of-a-linear-map.md); the second says it has zero [cokernel](../../../../../cokernel.md). Therefore

$$
\boxed{\Delta\smile-:H^i(BG;\mathbb F)\xrightarrow{\sim}H^{i+n}(BG;\mathbb F),\qquad i>0}.
$$

This is [periodic group cohomology from a free sphere action](../../../../../periodic-group-cohomology-from-a-free-sphere-action.md). Degree zero was excluded for a reason: $E_\infty^{0,n-1}$ can contribute to the quotient's top cohomology.

For $C_p=\mathbb Z/p$, use its periodic free resolution with alternating maps $g-1$ and $N=1+g+\cdots+g^{p-1}$. Applying $\operatorname{Hom}_{\mathbb Z[C_p]}(-,\mathbb F_p)$ makes every differential zero, so $H^i(BC_p;\mathbb F_p)$ is one-dimensional in every nonnegative degree. The two-step shift of the resolution supplies a nonzero degree-two class $u$ whose [cup product](../../../../../cup-product.md) gives the periodicity isomorphisms. For odd $p$, let $v$ be a nonzero degree-one class. Graded commutativity gives $v^2=0$, and the shift gives nonzero $v u^k$ and $u^k$ in every degree. For $p=2$, the two resolution maps agree over $\mathbb F_2[C_2]$, giving a one-step shift whose degree-one class has nonzero powers. Hence the [cohomology ring of a finite cyclic group over its prime field](../../../../../cohomology-ring-of-a-finite-cyclic-group-over-its-prime-field.md) is

$$
\boxed{H^*(BC_p;\mathbb F_p)=
\begin{cases}
\mathbb F_2[v],&p=2,\quad |v|=1,\\
\Lambda_{\mathbb F_p}(v)\otimes\mathbb F_p[u],&p\text{ odd},\quad |v|=1,\ |u|=2.
\end{cases}}
$$

Here the exterior factor is an [exterior algebra](../../../../../exterior-algebra.md) and the polynomial factor is a [polynomial ring](../../../../../polynomial-ring.md). For odd $p$, $u$ may be chosen as the [Bockstein homomorphism](../../../../../bockstein-homomorphism.md) of $v$.

If $G$ contained $C_p\times C_p$, restriction would give that subgroup the same free, cohomologically trivial sphere action. It would therefore also have period $n$ in positive-degree cohomology. But $B(C_p\times C_p)\simeq BC_p\times BC_p$, and the [Künneth theorem](../../../../../kunneth-theorem.md) gives

$$
\dim_{\mathbb F_p}H^i(B(C_p\times C_p);\mathbb F_p)
=\sum_{a+b=i}1=i+1.
$$

These dimensions strictly increase, so the groups in degrees $i$ and $i+n$ cannot be isomorphic. Thus **$G$ contains no subgroup isomorphic to $\mathbb Z/p\times\mathbb Z/p$ for any prime $p$**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 127](../../paper-127-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
