<h1 id="25k/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For independent random variables $X_1,X_2,\ldots$, let $\mathcal F_n=\sigma(X_1,\ldots,X_n)$, $\mathcal F=\sigma(X_1,X_2,\ldots)$, and let the [tail sigma-algebra](../../../../../../tail-sigma-algebra.md) be $\mathcal T=\bigcap_n\sigma(X_{n+1},X_{n+2},\ldots)$. [Kolmogorov zero-one law](../../../../../../kolmogorov-s-zero-one-law.md) states that every $A\in\mathcal T$ has probability zero or one.

Such an event is independent of each $\mathcal F_n$ by independence of the variables. The collection of events $B\in\mathcal F$ satisfying $\mathbb P(A\cap B)=\mathbb P(A)\mathbb P(B)$ is a [Dynkin system](../../../../../../dynkin-system.md): it contains the whole space and is closed under complements and disjoint countable unions. It contains the [pi-system](../../../../../../pi-system.md) $\bigcup_n\mathcal F_n$, which generates $\mathcal F$. The [pi-lambda theorem](../../../../../../pi-lambda-theorem.md) therefore makes $A$ independent of all of $\mathcal F$. Since $A$ itself belongs to $\mathcal F$,

$$
\mathbb P(A)=\mathbb P(A\cap A)=\mathbb P(A)^2,\qquad\boxed{\mathbb P(A)\in\{0,1\}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [25K](../../25k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
