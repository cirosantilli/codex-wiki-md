<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The assertion that [filtered colimits commute with finite limits in sets](../../../../../filtered-colimits-commute-with-finite-limits-in-sets.md) means that for every filtered category $\mathcal J$, every finite category $\mathcal I$, and every functor $D:\mathcal I\times\mathcal J\to\mathbf{Set}$, the canonical comparison

$$
\varinjlim_{j\in\mathcal J}\varprojlim_{i\in\mathcal I}D(i,j)
\longrightarrow
\varprojlim_{i\in\mathcal I}\varinjlim_{j\in\mathcal J}D(i,j)
$$

is a bijection. Surjectivity follows because an element on the right uses only finitely many representatives and compatibility equations, so filteredness moves all of them to one common stage. For injectivity, equality likewise consists of finitely many equalities, which become true at one later common stage.

The dual assertion fails in $\mathbf{Set}^{\mathrm{op}}$. Equivalently, [cofiltered limits need not commute with finite colimits in sets](../../../../../cofiltered-limits-need-not-commute-with-finite-colimits-in-sets.md). Index inverse systems by $n\in\mathbb N$, with arrows $n+1\to n$, and put

$$
A_n=\{m\in\mathbb N:m\geq n\},\qquad B_n=C_n=1,
$$

using the inclusions $A_{n+1}\hookrightarrow A_n$ and the unique maps $A_n\to B_n,C_n$. Since $A_n$ is nonempty, the pushout $B_n\sqcup_{A_n}C_n$ is a singleton at every stage, so its inverse limit is a singleton. But

$$
\varprojlim A_n=\bigcap_nA_n=\varnothing,
$$

and the pushout of the inverse limits is $1\sqcup_\varnothing1$, which has two elements. Thus a cofiltered limit fails to preserve this finite pushout.

Let $F$ be a [presheaf of sets on a topological space](../../../../../presheaf-of-sets-on-a-topological-space.md) $X$. The neighborhoods of $x$, ordered by reverse inclusion, form a filtered category, and

$$
F_x=\varinjlim_{U\ni x}F(U).
$$

The first result therefore says that the [stalk functor for presheaves of sets](../../../../../stalk-functor-for-presheaves-of-sets.md) preserves finite limits.

For a set $S$, define a presheaf $R_xS$ by

$$
(R_xS)(U)=
\begin{cases}
S,&x\in U,\\
1,&x\notin U,
\end{cases}
$$

with identity restrictions between neighborhoods of $x$ and the unique maps to $1$ otherwise. A natural transformation $F\to R_xS$ is exactly a compatible family of maps $F(U)\to S$ over neighborhoods of $x$, hence exactly a map $F_x\to S$. Thus

$$
\operatorname{Hom}(F,R_xS)\cong\operatorname{Hom}(F_x,S),
$$

so $R_x$ is right adjoint to the stalk functor.

Now restrict to [sheaves](../../../../../sheaf-mathematics.md). Suppose two morphisms $\alpha,\beta:F\rightrightarrows G$ induce the same map on every stalk. For $s\in F(U)$ and every $x\in U$, equality of the two germs gives a neighborhood $V_x\subseteq U$ on which $\alpha(s)$ and $\beta(s)$ agree. The $V_x$ cover $U$, so the uniqueness axiom for $G$ gives $\alpha(s)=\beta(s)$. Therefore the [joint stalk functor on sheaves of sets](../../../../../joint-stalk-functor-on-sheaves-of-sets.md)

$$
P:\mathbf{Sh}(X)\longrightarrow\mathbf{Set}^X,
\qquad F\longmapsto(F_x)_{x\in X},
$$

is faithful.

The presheaf $R_xS$ above is already a sheaf: an open containing $x$ has a cover member containing $x$, and compatibility forces one common element of $S$. Hence a right adjoint to $P$ sends a family $(S_x)$ to the product $\prod_xR_xS_x$, whose existence follows from the assumed closure of $\mathbf{Sh}(X)$ under limits.

Each stalk preserves finite limits, so $P$ preserves equalizers. If $P(f)$ is an isomorphism, its monicity and epicity are reflected by the faithful functor $P$; since $\mathbf{Sh}(X)$ is assumed [balanced](../../../../../balanced-category.md), $f$ is an isomorphism. Thus $P$ reflects isomorphisms. The [Beck comonadicity theorem](../../../../../beck-comonadicity-theorem.md) now applies: $P$ has a right adjoint, reflects isomorphisms, and preserves the required equalizers. Consequently $P$ is comonadic.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
