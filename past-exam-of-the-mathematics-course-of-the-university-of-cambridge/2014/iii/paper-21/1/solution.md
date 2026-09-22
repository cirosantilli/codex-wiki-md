<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**There is no computable presentation of a [nonstandard model of Peano arithmetic](../../../../../non-standard-model-of-arithmetic.md).** We prove [Tennenbaum theorem](../../../../../tennenbaum-s-theorem.md) by obtaining a [computable set](../../../../../computable-set.md) separating two [recursively inseparable sets](../../../../../recursively-inseparable-sets.md).

Fix an effective enumeration $(\varphi_e)$ of [partial computable functions](../../../../../computable-function.md), implemented by deterministic machines, and put

$$
U=\{e:\varphi_e(e)\downarrow=0\},\qquad V=\{e:\varphi_e(e)\downarrow=1\}.
$$

These are disjoint [computably enumerable sets](../../../../../recursively-enumerable-set.md). To see that they are [recursively inseparable sets](../../../../../recursively-inseparable-sets.md), suppose a [computable set](../../../../../computable-set.md) $D$ contains $U$ and avoids $V$. Its [indicator function](../../../../../indicator-function.md) has some index $k$. If $\varphi_k(k)=0$, then $k\in U\subseteq D$, contradicting that output. If $\varphi_k(k)=1$, then $k\in V$, contradicting $D\cap V=\varnothing$. Thus neither output is possible.

Let $M\models\mathrm{PA}$ be a [nonstandard model of Peano arithmetic](../../../../../non-standard-model-of-arithmetic.md). A [recursive presentation of a structure](../../../../../recursive-presentation-of-a-structure.md) here means a presentation on $\mathbb N$ in which its arithmetic operations are [total computable functions](../../../../../total-computable-function.md); equality of presentation codes is ordinary equality. Write $\bar n$ for the element represented by the standard numeral $n$. The presentation codes of $\bar0,\bar1$ are fixed constants, so $n\mapsto\bar n$ is a [total computable function](../../../../../total-computable-function.md) obtained by repeated addition. Presentation codes and the arithmetic values they name must be kept distinct.

Use [bounded simulation of a computation](../../../../../bounded-simulation-of-a-computation.md) predicates $H_i(e,t)$ saying that machine $e$, on input $e$, has halted by time $t$ with output $i$. We can choose these as [primitive recursive](../../../../../primitive-recursive-function.md) predicates represented in [Peano arithmetic](../../../../../peano-arithmetic.md). Determinism and induction on the computation length give, provably in [Peano arithmetic](../../../../../peano-arithmetic.md), monotonicity in $t$ and

$$
\forall e\,\forall t\,\forall s\;\neg\bigl(H_0(e,t)\land H_1(e,s)\bigr).
$$

A genuine standard halting computation has a finite certificate which [Peano arithmetic](../../../../../peano-arithmetic.md) verifies. Consequently, if $e\in U$ or $e\in V$, the corresponding $H_i(\bar e,\bar t)$ holds in $M$ for some standard $t$.

Choose a nonstandard element $c$ of $M$. It exceeds every standard numeral. Let $p_e$ be the $e$th [prime number](../../../../../prime-number.md), starting with $p_0=2$. [Peano arithmetic](../../../../../peano-arithmetic.md) proves the [prime-divisibility coding of a finite set](../../../../../prime-divisibility-coding-of-a-finite-set.md) needed here: for each $c$, an element $d$ can be formed as the product of precisely those $p_e$ with $e<c$ for which $H_0(e,c)$ holds. Formally,

$$
M\models\forall e<c\;\bigl(p_e\mid d\ \longleftrightarrow\ H_0(e,c)\bigr).
$$

This is an internally finite product, not a claim that its externally observed index set is finite. Its existence follows by [mathematical induction](../../../../../mathematical-induction.md) on the cutoff: start with $1$, multiply by the next distinct [prime number](../../../../../prime-number.md) when its predicate holds, and otherwise retain the product. [Unique prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) ensures that earlier divisibility decisions are preserved. The standard prime enumeration and these finite-product constructions are provably total in [Peano arithmetic](../../../../../peano-arithmetic.md).

Define the external subset $D=\{e\in\mathbb N:M\models p_{\bar e}\mid d\}$. If $e\in U$, its standard halting time is below $c$, and monotonicity gives $H_0(\bar e,c)$, so $e\in D$. If $e\in V$, its output-one certificate and the provable incompatibility above exclude $H_0(\bar e,c)$, so $e\notin D$. Hence $D$ separates $U$ and $V$.

Finally $D$ is a [computable set](../../../../../computable-set.md). Given standard $e$, compute the ordinary integer $p_e$ and its numeral in the presentation. Enumerate all presentation codes $q$, and for each test the finitely many standard remainders $0\le r<p_e$ for

$$
 d=\bar p_e\cdot q+\bar r.
$$

Each test is decidable using the assumed [total computable functions](../../../../../total-computable-function.md). The division theorem of [Peano arithmetic](../../../../../peano-arithmetic.md) guarantees a quotient and a remainder below the standard numeral $\bar p_e$. Every element below that numeral is one of $\bar0,\ldots,\overline{p_e-1}$, so the search terminates; the remainder is unique. Return yes exactly when $r=0$. This makes $D$ a [computable set](../../../../../computable-set.md), contradicting the [recursively inseparable sets](../../../../../recursively-inseparable-sets.md) construction. Therefore

$$
\boxed{M\models\mathrm{PA}\text{ nonstandard}\ \Longrightarrow\ M\text{ has no recursive presentation}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
