<h1 id="5e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Reflexivity follows by taking the two exponents equal to $1$, and symmetry is built into the two divisibility conditions. For transitivity, suppose $m\mid n^a$, $n\mid m^b$, $n\mid \ell^c$ and $\ell\mid n^d$. Then $m\mid\ell^{ac}$ and $\ell\mid m^{bd}$, with positive exponents. Thus the relation is an [equivalence relation](../../../../../../equivalence-relation.md).

Its [equivalence classes](../../../../../../equivalence-class.md) have a useful description by [prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md). Let $S(n)$ be the finite set of [prime factors](../../../../../../prime-factor.md) of $n$, with $S(1)=\varnothing$. If $m\mid n^a$, every [prime factor](../../../../../../prime-factor.md) of $m$ divides $n$; the reverse divisibility gives $S(n)\subseteq S(m)$. Conversely, if $S(m)=S(n)$, write $m=\prod_{p\in S}p^{\alpha_p}$ and $n=\prod_{p\in S}p^{\beta_p}$, with all exponents positive. Choosing $a\ge\max_p\lceil\alpha_p/\beta_p\rceil$ and $b\ge\max_p\lceil\beta_p/\alpha_p\rceil$ gives the required divisibilities. The empty case is exactly $m=n=1$.

Therefore the [prime-support equivalence relation](../../../../../../prime-support-equivalence-relation.md) is

$$
\boxed{m\sim n\iff S(m)=S(n)\iff\operatorname{rad}(m)=\operatorname{rad}(n),}
$$

where the [radical of an integer](../../../../../../radical-of-an-integer.md) is the product of its distinct [prime factors](../../../../../../prime-factor.md). The class with empty support is $\{1\}$. For every nonempty finite support $S$, all positive exponent choices give one class, and varying just one exponent produces infinitely many different [integers](../../../../../../integer.md) in it.

There are infinitely many classes because each [prime number](../../../../../../prime-number.md) gives a different singleton support. For completeness, if there were only finitely many [prime numbers](../../../../../../prime-number.md) $p_1,\ldots,p_r$, a [prime factor](../../../../../../prime-factor.md) of $p_1\cdots p_r+1$ would differ from them all. **There are infinitely many classes; the unique finite class is $\{1\}$.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
