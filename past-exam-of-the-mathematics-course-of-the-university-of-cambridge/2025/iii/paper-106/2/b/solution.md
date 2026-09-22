<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

By definition of the [weak topology](../../../../../../weak-topology-split.md), $x_n\rightharpoonup x$ exactly when $f(x_n)\to f(x)$ for every $f\in X^*$.

Let $(x_n)$ be bounded and choose a norm-dense sequence $(f_j)$ in $X^*$. Successive subsequences make $f_1(x_n),f_2(x_n),\ldots$ converge, and the [diagonal argument](../../../../../../diagonal-argument.md) produces a single subsequence $(y_n)$ on which every $f_j$ converges. Uniform boundedness of $(y_n)$ and norm approximation of an arbitrary $f$ by the $f_j$ show that $f(y_n)$ is Cauchy for every $f\in X^*$. Thus $(y_n)$ is [weakly Cauchy](../../../../../../weakly-cauchy-sequence.md), and

$$
f(y_{2n}-y_{2n-1})\longrightarrow0
$$

for every $f$, so its difference sequence is [weakly null](../../../../../../weakly-null-sequence.md).

For the countable family $(y_{m,n})_n$, use the weak metric from part a. Delete a finite initial segment from the $m$th sequence so that every remaining term has weak distance less than $1/m$ from zero, and relabel that tail. Enumerate all these tails while preserving the order within each one. For every weak neighbourhood of zero, all terms from sufficiently large $m$ lie inside it, and only finitely many terms from each of the finitely many remaining sequences lie outside it. The resulting enumeration $(z_n)$ is weakly null and contains the relabelled $m$th sequence as a subsequence for every $m$. Equivalently, without relabelling, it contains a tail-subsequence of every original sequence, which is the form used below.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 106](../../../paper-106-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
