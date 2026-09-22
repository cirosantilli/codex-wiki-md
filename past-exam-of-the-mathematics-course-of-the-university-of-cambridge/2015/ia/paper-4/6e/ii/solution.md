<h1 id="6e/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $1\le j\le p-1$, the identity for [binomial coefficients](../../../../../../binomial-coefficient.md)

$$
j\binom pj=p\binom{p-1}{j-1}
$$

shows that $p$ divides $j\binom pj$. Since $p$ is a [prime number](../../../../../../prime-number.md) and $j$ is not divisible by $p$, cancellation modulo $p$ gives

$$
\boxed{\binom pj\equiv0\pmod p\quad(0<j<p).}
$$

The [binomial theorem](../../../../../../binomial-theorem.md) consequently gives $(1+x)^p\equiv1+x^p$ as a coefficientwise polynomial [modular congruence](../../../../../../modular-congruence.md). Apply the same identity with $x$ replaced by $x^{p^r}$ and use [mathematical induction](../../../../../../mathematical-induction.md) to obtain

$$
(1+x)^{p^i}\equiv1+x^{p^i}\pmod p\qquad(i\ge1).
$$

This is an iteration of the [Frobenius endomorphism](../../../../../../frobenius-endomorphism.md) in characteristic $p$. Comparing the intermediate coefficients gives the [prime-power binomial divisibility](../../../../../../prime-power-binomial-divisibility.md) result

$$
\boxed{\binom{p^i}{j}\equiv0\pmod p\quad(0<j<p^i).}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6E](../../6e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
