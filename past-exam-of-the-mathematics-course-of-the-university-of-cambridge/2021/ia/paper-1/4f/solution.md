<h1 id="4f/solution">Solution</h1>

↑ **Parent:** [4F](../4f.md)

The [Bolzano-Weierstrass theorem](../../../../../bolzano-weierstrass-theorem.md) states that every bounded sequence of real numbers has a convergent subsequence.

For a proof, place all terms in a closed bounded interval $I_1$. Bisect it and choose a closed half $I_2$ containing infinitely many terms. Continue inductively, choosing nested closed intervals

$$
I_1\supseteq I_2\supseteq\cdots
$$

with infinitely many sequence terms and with lengths tending to zero. Choose $n_k>n_{k-1}$ such that $x_{n_k}\in I_k$. The [nested interval theorem](../../../../../nested-interval-theorem.md) gives a unique point $x$ in every $I_k$. Because both $x_{n_k}$ and $x$ lie in $I_k$,

$$
|x_{n_k}-x|\leq |I_k|\longrightarrow0.
$$

Thus $(x_{n_k})$ is a convergent subsequence.

Now suppose every convergent subsequence of the bounded sequence $(x_n)$ converges to $L$. If $x_n$ did not converge to $L$, there would be an $\epsilon>0$ and a subsequence $(x_{n_k})$ satisfying

$$
|x_{n_k}-L|\geq\epsilon
$$

for every $k$. This subsequence is bounded, so Bolzano--Weierstrass gives a convergent subsubsequence. By hypothesis its limit is $L$, contradicting the displayed inequality. Hence the [unique subsequential limit of a bounded sequence](../../../../../unique-subsequential-limit-of-a-bounded-sequence.md) principle gives

$$
\boxed{x_n\to L}.
$$

## ↑ Ancestors (10)

1. [4F](../4f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
