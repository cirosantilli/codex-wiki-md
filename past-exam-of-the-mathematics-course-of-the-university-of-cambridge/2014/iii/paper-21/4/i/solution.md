<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Yes. There is a [computable isomorphism](../../../../../../computable-isomorphism.md), obtained by an [effective back-and-forth construction](../../../../../../effective-back-and-forth-construction.md).** Decidability of the two orders makes the usual existence argument into an algorithm.

Maintain a finite [order-preserving](../../../../../../order-preserving-function.md) [partial isomorphism of structures](../../../../../../partial-embedding.md) $f_s$ from $(\mathbb N,<_A)$ to $(\mathbb N,<_B)$, starting with the empty map. At a forth step, take the least ordinary natural number $a$ outside its domain. Look at the finitely many mapped elements below and above $a$ in $<_A$. Their images impose an [open interval](../../../../../../open-interval.md) in $<_B$: it lies above all the lower images and below all the upper images, with a missing bound interpreted as an unbounded side.

This interval contains a fresh element. If both bounds exist they are ordered correctly by the induction hypothesis; density supplies an element strictly between them. If there is just one bound, the absence of endpoints supplies an element beyond it; if there are no bounds, choose any element. Density and the absence of endpoints moreover give infinitely many points in every such [open interval](../../../../../../open-interval.md), so finitely many already used images can always be avoided.

Enumerate $b=0,1,2,\ldots$ in the ordinary presentation order, test whether $b$ is unused and satisfies every required $<_B$ inequality, and choose the first successful candidate. All tests are decidable, and the existence argument proves termination. Extend $f_s$ by $a\mapsto b$.

At a back step, take the least natural number outside the range, interchange the roles of $A$ and $B$, and carry out exactly the same search for a fresh preimage. Alternate forth and back steps. Every stage is an effective terminating finite computation, and every stage remains an [order-preserving](../../../../../../order-preserving-function.md) [partial isomorphism of structures](../../../../../../partial-embedding.md).

Let $f=\bigcup_s f_s$. The least-unused scheduling puts every element of $A$ into the domain and every element of $B$ into the range. For example, after $n+1$ forth steps, all ordinary presentation numbers at most $n$ have been included, since each step removes the least missing one. Thus $f$ is a [bijection](../../../../../../bijection.md) preserving and reflecting the orders. To compute $f(n)$, simulate the construction until $n$ appears in its domain; this terminates. The corresponding range search computes its inverse. Hence

$$
\boxed{f:(\mathbb N,<_A)\cong(\mathbb N,<_B),\qquad f,f^{-1}\text{ are computable}.}
$$

The searches use the decidable presentations, rather than a possibly ineffective choice of points in an abstract [dense linear order without endpoints](../../../../../../dense-linear-order-without-endpoints.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
