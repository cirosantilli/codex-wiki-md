<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

The [Fermat little theorem](../../../../../fermat-little-theorem.md) states that if $p$ is a [prime number](../../../../../prime-number.md), then $a^p\equiv a\pmod p$ for every [integer](../../../../../integer.md) $a$. Equivalently, for $p\nmid a$, $a^{p-1}\equiv1\pmod p$.

To prove it when $p\nmid a$, multiplication by $a$ permutes the nonzero residues $1,\ldots,p-1$. Indeed, $ai\equiv aj\pmod p$ implies $p\mid a(i-j)$, and the [Euclid lemma](../../../../../euclid-lemma.md) implies $i=j$ in this range. Multiplying all these residues gives

$$
a^{p-1}(p-1)!\equiv(p-1)!\pmod p.
$$

None of the factors of $(p-1)!$ is divisible by $p$, so the [factorial](../../../../../factorial.md) has a [modular inverse](../../../../../modular-multiplicative-inverse.md). Cancelling it proves $a^{p-1}\equiv1$, hence $a^p\equiv a$. When $p\mid a$, the latter identity has both sides zero, completing the proof.

For an odd [prime number](../../../../../prime-number.md) $p\ne5$, the numbers $10,p$ are coprime. The [Fermat little theorem](../../../../../fermat-little-theorem.md) gives $10^{p-1}\equiv1\pmod p$, and consequently

$$
\boxed{p\mid10^{j(p-1)}-1\quad\text{for every }j\ge1.}
$$

These exponents are distinct, so infinitely many are obtained.

Write the [repdigit](../../../../../repdigit.md) with $n$ copies of $5$ as

$$
R_n=5\sum_{j=0}^{n-1}10^j=\frac{5(10^n-1)}9.
$$

If $p\ne3,5$, choose $n$ to be any positive multiple of $p-1$. Then $9$ has a [modular inverse](../../../../../modular-multiplicative-inverse.md) modulo $p$, so $p\mid R_n$. Division by $9$ cannot be used modulo $3$; instead $10\equiv1\pmod3$ gives $R_n\equiv5n\pmod3$, so $3\mid R_{3j}$ for every $j\ge1$. If $p=5$, every $R_n$ is divisible by $5$. Thus

$$
\boxed{\text{Every odd prime divides infinitely many of }5,55,555,\ldots.}
$$

The separate treatment of $3$ accounts for the prime factor of the geometric-sum denominator.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
