<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $M$ be a nonstandard model of the [theory of true arithmetic](../../../../../../true-arithmetic.md) whose carrier is $\mathbb N$, and suppose for contradiction that the graphs of $+^M$ and $\times^M$ are decidable. Because these operations are total, searching their decidable graphs computes their output on any pair of carrier elements.

Choose disjoint [recursively inseparable sets](../../../../../../recursively-inseparable-sets.md) $A,B$ that are computably enumerable, with primitive recursive stage predicates $E_A(n,s)$ and $E_B(n,s)$. Let $c\in M$ be nonstandard. True arithmetic proves finite sequence coding, so inside $M$ there is an element $a$ such that, for every $i<c$,

$$
p_i^M\mid^M a
\quad\Longleftrightarrow\quad
M\models\exists s<c\,E_A(i,s),
$$

where $p_i$ is the $i$th prime. This can be obtained by taking the product of the selected primes internally; it is the same finite coding mechanism as [Gödel beta-function sequence coding](../../../../../../godel-beta-function-sequence-coding.md).

Define the external set

$$
C=\{n\in\mathbb N:M\models p_n^M\mid a\}.
$$

This set is decidable from the assumed operations. For fixed standard $n$, compute the model element $p_n^M$. The division algorithm in $M$ gives unique $q$ and a remainder among the finitely many standard residues

$$
0^M,1^M,\ldots,(p_n-1)^M
$$

such that $a=q\times^M p_n^M+r$. Dovetail the search over $q$ and these finitely many residues, using the computable model operations. It eventually finds the unique remainder, and $n\in C$ exactly when that remainder is zero.

If $n\in A$, it enters $A$ at a standard stage below the nonstandard $c$, so $n\in C$. If $n\in B$, the true arithmetical sentence asserting that the two enumerations are disjoint holds in $M$, so $n$ cannot enter the coded $A$-set below $c$; hence $n\notin C$. Thus

$$
A\subseteq C,
\qquad
B\cap C=\varnothing,
$$

contradicting recursive inseparability. The two operation graphs therefore cannot both be decidable. This is the [recursively inseparable-set proof of Tennenbaum theorem](../../../../../../recursively-inseparable-set-proof-of-tennenbaum-theorem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
