<h1 id="6e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [inclusion-exclusion principle](../../../../../../inclusion-exclusion-principle.md) says that the size of a finite union is the alternating sum of the sizes of all nonempty intersections of its constituent sets.

For each [prime number](../../../../../../prime-number.md) $p\mid n$, let $A_p$ consist of the tuples for which $p$ divides every $x_i$. Exactly $(n/p)^r$ tuples lie in $A_p$, and for distinct primes $p_1,\ldots,p_j\mid n$, exactly $(n/(p_1\cdots p_j))^r$ lie in their intersection. A tuple has greatest common divisor greater than one with $n$ exactly when it belongs to some $A_p$. Inclusion-exclusion therefore gives the [Jordan totient function](../../../../../../jordan-s-totient-function.md)

$$
\phi_r(n)
=n^r\sum_{S\subseteq\{p:p\mid n\}}(-1)^{|S|}\prod_{p\in S}p^{-r}
=\boxed{n^r\prod_{p\mid n}(1-p^{-r})}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
