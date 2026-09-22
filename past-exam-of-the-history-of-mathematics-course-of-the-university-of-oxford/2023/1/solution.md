<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The passage belongs to the English reception of [Euclid](../../../euclid.md)'s [number theory](../../../number-theory-split.md). [Henry Billingsley](../../../henry-billingsley.md)'s [The Elements of Geometrie by Henry Billingsley](../../../the-elements-of-geometrie-by-henry-billingsley.md), published in 1570, brought the [Elements](../../../euclid-s-elements.md) into English with extensive explanatory material. The original title page advertises translation and annotations; the extract's worked examples show what explanatory prose could add to a compact [definition](../../../definition-mathematics.md). [Henry Billingsley](../../../henry-billingsley.md)'s numbering calls this Definition 23 of Book VII; the familiar modern numbering is VII, Definition 22. The difference is editorial, not a difference in the [perfect number](../../../perfect-number.md) being defined.[Title page and Book VII, Definition 23, in the Text Creation Partnership transcription](../../../the-elements-of-geometrie-by-henry-billingsley.md)[Definition and guide](../../../euclid-s-elements-by-euclid/book-vii-definition-22.md)

Here a number's parts are its positive [proper divisors](../../../proper-divisor.md), rather than arbitrary pieces of a [sum](../../../sum.md) or all smaller [integers](../../../integer-split.md). In modern notation the [definition](../../../definition-mathematics.md) is

$$
\boxed{\sum_{\substack{d\mid n\\1\leq d<n}}d=n,\qquad\text{equivalently }\sigma(n)=2n,}
$$

where $\sigma$ is the [sum-of-divisors function](../../../sum-of-divisors-function.md). Thus $12$ is not a [perfect number](../../../perfect-number.md): its positive [proper divisors](../../../proper-divisor.md) total $1+2+3+4+6=16$. It is essential to exclude $n$ itself: including it would double the required [sum](../../../sum.md). The pairing of a [divisor](../../../divisor.md) $d$ with the fraction $1/(n/d)$ of the whole explains the extract's language of halves, thirds and so on. Its examples are complete checks because they identify every positive [proper divisor](../../../proper-divisor.md), not merely some convenient decomposition.

The larger mathematical context is the construction in [Book IX, Proposition 36](../../../euclid-s-elements-by-euclid/book-ix-proposition-36.md). If $q=2^p-1$ is a [prime number](../../../prime-number-split.md), then $N=2^{p-1}q$ is a [perfect number](../../../perfect-number.md). To reconstruct the argument, [prime factorization](../../../fundamental-theorem-of-arithmetic.md) gives all its [divisors](../../../divisor.md) as $2^j$ and $q2^j$, with $0\leq j\leq p-1$. A [finite geometric series](../../../finite-geometric-series.md) therefore gives

$$
\sigma(N)=(1+q)\sum_{j=0}^{p-1}2^j
=2^p(2^p-1)=2N.
$$

The choices $p=2,3,5,7$ produce $6,28,496,8128$. The [primality](../../../primality.md) assumption matters: choosing $p=4$ produces $120$, whose [sum-of-divisors function](../../../sum-of-divisors-function.md) is $360$, not $240$. The construction gives a reason for the examples and connects [perfect numbers](../../../perfect-number.md) with [Mersenne primes](../../../mersenne-prime.md).[Statement, construction and guide](../../../euclid-s-elements-by-euclid/book-ix-proposition-36.md)

The extract itself supplies a [definition](../../../definition-mathematics.md) and examples, not a classification or a [mathematical proof](../../../mathematical-proof.md) that such numbers are rare. In particular, the converse that every even [perfect number](../../../perfect-number.md) has this form belongs to the later [Euclid-Euler theorem](../../../euclid-euler-theorem.md); it should not be read back into this passage. The historically significant feature is **the transmission of deductive arithmetic through vernacular explanation**: a book called geometry also teaches the [divisibility](../../../divisibility-split.md) theory needed for a general construction.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2023](../../2023-split.md)
3. [Past exam of the history of mathematics course of the University of Oxford](../../split.md)
4. [History of mathematics course of the University of Oxford](../../../history-of-mathematics-course-of-the-university-of-oxford.md)
5. [Year 3 of the mathematics course of the University of Oxford](../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
