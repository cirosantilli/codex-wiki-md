<h1 id="4i/solution">Solution</h1>

↑ **Parent:** [4I](../4i.md)

Fix an effective enumeration of register-machine programs. The $n$th register machine is $P_n$, and its domain

$$
W_n=\{x:P_n\text{ halts on input }x\}
$$

is the $n$th [recursively enumerable set](../../../../../recursively-enumerable-set.md). A [many-one reduction](../../../../../many-one-reduction.md) $A\leq_mB$ is a total computable function $h$ satisfying $x\in A\iff h(x)\in B$. [Rice theorem](../../../../../rice-s-theorem.md) says that every nontrivial property depending only on the computed partial function, or equivalently on an r.e. set in its extensional form, has an undecidable index set.

There is no total equality algorithm: it would decide whether $W_n$ is empty by comparing it with a fixed index for the empty set, contradicting Rice's theorem.

There is no partial algorithm that halts exactly when $W_m=W_n$ either. Given $e$, effectively construct an index $h(e)$ whose machine enumerates nothing unless $P_e(e)$ halts, after which it enumerates $0$. Then

$$
W_{h(e)}=\varnothing\iff e\notin K.
$$

A semialgorithm for equality with a fixed empty index would enumerate the complement of the [halting problem](../../../../../halting-problem.md) $K$. Since $K$ is r.e., both it and its complement would then be r.e., making $K$ recursive, a contradiction.

## ↑ Ancestors (10)

1. [4I](../4i.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
