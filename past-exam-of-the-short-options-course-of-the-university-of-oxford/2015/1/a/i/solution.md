<h1 id="1/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [binomial theorem](../../../../../binomial-theorem.md) isolates the only terms that can survive reduction modulo the [prime number](../../../../../prime-number-split.md) $p$:

$$
(a+b)^p=a^p+b^p+\sum_{r=1}^{p-1}\binom pr a^{p-r}b^r.
$$

For $1\le r\le p-1$, neither $r!$ nor $(p-r)!$ is divisible by $p$, whereas $p!$ is. Consequently $p\mid\binom pr$, and every intermediate term vanishes in [modular arithmetic](../../../../../modular-arithmetic-split.md). Thus

$$
\boxed{(a+b)^p\equiv a^p+b^p\pmod p.}
$$

This works for arbitrary [integers](../../../../../integer-split.md) $a,b$, including those divisible by $p$. It is the additive identity behind the [Frobenius endomorphism](../../../../../frobenius-endomorphism.md) in [characteristic](../../../../../characteristic-of-a-field.md) $p$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
