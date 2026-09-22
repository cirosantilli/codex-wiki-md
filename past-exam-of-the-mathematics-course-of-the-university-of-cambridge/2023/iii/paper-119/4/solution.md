<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Because $F:\mathbf{Set}\to\mathbf{Set}$ preserves finite limits and colimits, $F(1)$ is a singleton and $F(\varnothing)=\varnothing$. For $x\in X$, let $\bar x:1\to X$ select $x$ and define

$$
\alpha_X(x)=F(\bar x)(*),
$$

where $*$ is the unique element of $F(1)$. This is natural in $X$. Any [natural transformation](../../../../../natural-transformation.md) $1_{\mathbf{Set}}\to F$ has the unique possible component at $1$, and naturality along every $\bar x$ forces the displayed value, so $\alpha$ is unique.

If $x\ne y$, the [equalizer](../../../../../equaliser.md) of $\bar x,\bar y:1\rightrightarrows X$ is empty. Since $F$ preserves this equalizer, $F(\bar x)(*)\ne F(\bar y)(*)$. Hence every $\alpha_X$ is injective, so $\alpha$ is pointwise monic.

Finite-colimit preservation makes $\alpha_n:n\to F(n)$ bijective for every finite set. Use the stated characterization of $\mathbb N$ by the coproduct diagram

$$
1\xrightarrow{0}\mathbb N\xleftarrow{s}\mathbb N
$$

and the coequalizer of $s,1_{\mathbb N}:\mathbb N\rightrightarrows\mathbb N$. Applying $F$ preserves both diagrams. Naturality and uniqueness in this characterization identify $\alpha_{\mathbb N}:\mathbb N\to F(\mathbb N)$ as an isomorphism.

For a countable family $(A_n)$, let $p:\coprod_nA_n\to\mathbb N$ record the summand. Each square

$$
\begin{array}{ccc}
A_n&\longrightarrow&\coprod_kA_k\\
\downarrow&&\downarrow p\\
1&\xrightarrow{n}&\mathbb N
\end{array}
$$

is a [pullback](../../../../../pullback-category-theory.md). Applying $F$ and using $F(1)\cong1$ and $F(\mathbb N)\cong\mathbb N$ shows that $F(A_n)$ is exactly the fiber of $F(p)$ over $n$. Those fibers partition $F(\coprod_nA_n)$, so the canonical map

$$
\coprod_nF(A_n)\longrightarrow F\left(\coprod_nA_n\right)
$$

is bijective. Thus $F$ preserves [countable coproducts](../../../../../countable-coproduct.md).

Now choose $x\in F(A)\setminus\alpha_A(A)$ and define

$$
U=\{A'\subseteq A:x\in\operatorname{im}(F(A')\to F(A))\}.
$$

It is upward closed. Since $A=A'\sqcup(A\setminus A')$ and $F$ preserves binary coproducts, $x$ lies in exactly one of the two summands, so exactly one of $A'$ and its complement lies in $U$. Pullback preservation gives closure under finite intersections.

For countable completeness, take $A_n\in U$ and put $B=\bigcap_nA_n$. If $B\notin U$, then $A\setminus B\in U$. Partition $A$ into $B$ and the sets

$$
C_n=(A\setminus A_n)\setminus\bigcup_{k<n}(A\setminus A_k),
$$

which record the first failed membership. Since $F$ preserves countable coproducts, exactly one cell of this partition lies in $U$. It cannot be $B$, so some $C_n\in U$. But $C_n\subseteq A\setminus A_n$, forcing $A\setminus A_n\in U$, contrary to $A_n\in U$. Hence $B\in U$.

Finally no finite $K$ belongs to $U$. Indeed, $F(K)\cong K$ through $\alpha_K$, so if $x$ came from $F(K)$ then naturality would put $x$ in the image of $\alpha_A$. Thus $U$ is a [countably complete ultrafilter](../../../../../countably-complete-ultrafilter.md) and is [nonprincipal](../../../../../nonprincipal-ultrafilter.md).

Conversely, let $U$ be such an ultrafilter on $A$ and define the [ultrapower endofunctor of sets](../../../../../ultrapower-endofunctor-of-sets.md)

$$
F(B)=B^A/{\sim_U}.
$$

It preserves the terminal object and products: the map

$$
[(f,g)]\longmapsto([f],[g])
$$

is bijective because $U$ is closed under finite intersections. It preserves equalizers because an equality holding for an equivalence class holds on a $U$-large set, and the representative can be changed off that set to land in the equalizer. Hence it preserves all finite limits.

For $f:A\to\coprod_nB_n$, countable completeness implies that one index fiber

$$
\{a:f(a)\in B_n\}
$$

belongs to $U$; otherwise the countable intersection of all complementary fibers would be empty and belong to $U$. Thus every class $[f]$ lies in one and only one $F(B_n)$, proving preservation of countable coproducts.

The class of the identity map $A\to A$ is not represented by a constant map, since every equality set $\{a:a=a_0\}$ is a singleton and is not in $U$. Therefore $\alpha_A:A\to F(A)$ is not surjective. Since $\alpha$ is the unique natural transformation from the identity functor to $F$, a natural isomorphism $1_{\mathbf{Set}}\cong F$ would have to equal $\alpha$, which is impossible.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
