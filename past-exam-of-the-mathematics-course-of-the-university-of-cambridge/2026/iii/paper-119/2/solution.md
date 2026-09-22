<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

An [idempotent morphism](../../../../../idempotent-morphism.md) satisfies $e^2=e$ and splits if $e=ir$ with $ri=1$. Form the relative [Karoubi envelope](../../../../../karoubi-envelope.md) $\mathcal C[\check E]$: its objects are $(A,e)$ for $e\in E$, and

$$
\mathcal C[\check E]((A,e),(B,f))=\{u:A\to B:u=fue\}.
$$

The functor $A\mapsto(A,1_A)$ is full and faithful. Each $e\in E$ splits through $(A,e)$ using $e$ in both directions. If a functor $F:\mathcal C\to\mathcal D$ comes with splittings $F(e)=i_er_e$, define its extension by $(A,e)\mapsto$ the splitting object and $u\mapsto r_fF(u)i_e$. This gives the required factorization, unique up to the unique compatible natural isomorphism.

A preorder $R$ is reflexive and transitive, so $R\circ R=R$: transitivity gives one inclusion and reflexivity the other. If it is an equivalence relation, the quotient relation $q:X\to X/R$ satisfies $q^\mathsf{op}q=R$ and $qq^\mathsf{op}=1$, so it splits in [category of relations](../../../../../category-of-relations.md) $\mathbf{Rel}$. Conversely, writing a split preorder as $R=ir$, $ri=1$ and using reflexivity and transitivity shows $R=R^\mathsf{op}$; hence it is an equivalence relation.

Let $B$ be the set of join-inaccessible elements of a completely algebraic lattice $A$, and put

$$
i(a)=\{b\in B:b\leq a\},\qquad r(S)=\bigvee S.
$$

Then $ri=1_A$, while $r(S)\leq a$ exactly when $S\subseteq i(a)$, so $r\dashv i$. Join-inaccessibility gives $i(\bigvee_j a_j)=\bigcup_ji(a_j)$, so $i$ preserves all joins. Conversely, given such $r\dashv i$ with $ri=1$, each $r\{b\}$ is join-inaccessible: if $r\{b\}\leq\bigvee S$, adjunction and preservation of joins put $b$ in some $i(s)$, whence $r\{b\}\leq s$. Finally,

$$
a=r(i(a))=\bigvee_{b\in i(a)}r\{b\},
$$

so $A$ is completely algebraic.

Under the supplied full embedding $\mathbf{Rel}\to\mathbf{CSLat}$, a set goes to its power-set lattice and a preorder goes to the associated idempotent. Splitting those idempotents gives exactly the retracts of power sets by adjoint join maps characterized above. Therefore $\mathbf{Rel}[\check E]$ is equivalent to the full subcategory of complete join-semilattices consisting of completely algebraic lattices.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2026](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
