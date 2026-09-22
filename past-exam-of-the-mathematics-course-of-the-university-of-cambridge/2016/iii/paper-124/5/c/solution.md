<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A useful [method of moments in probability](../../../../../../method-of-moments-probability-theory.md) states that if real [random variables](../../../../../../random-variable-split.md) $Z_N$ have all moments, $\mathbb E Z_N^j\to m_j$ for every integer $j\ge1$, and $(m_j)$ is the moment sequence of a [moment-determinate probability distribution](../../../../../../moment-determinacy.md), then $Z_N$ converges to that distribution in the sense of [convergence in distribution](../../../../../../convergence-in-distribution.md). In particular, convergence to the [standard normal distribution](../../../../../../standard-normal-distribution.md) follows from limiting odd moments zero and limiting even moments $(2k-1)!!$. The [moment-generating function of a standard normal variable](../../../../../../moment-generating-function-of-a-standard-normal-variable.md), finite in a neighbourhood of zero, ensures [moment determinacy](../../../../../../moment-determinacy.md).

For the classical [Erdős-Kac theorem](../../../../../../erdos-kac-theorem.md), put $L=\log\log N$ and choose, for example, $\varphi(N)=L^{1/4}$, with a harmless modification for small $N$. Truncate the [prime omega function](../../../../../../prime-omega-function.md) to [primes](../../../../../../prime-number.md) $p\le y=N^{1/\varphi(N)}$. The omitted number of distinct [prime factors](../../../../../../prime-factor.md) of any $n\le N$ is at most $\varphi(N)$, since a product of $r$ omitted [primes](../../../../../../prime-number.md) exceeds $N^{r/\varphi(N)}$. Thus this truncation changes the normalized variable by $o(1)$ uniformly. Also, the [Mertens theorem for reciprocal primes](../../../../../../mertens-second-theorem.md) gives

$$
\sum_{p\le y}\frac1p=L-\log\varphi(N)+O(1)=L+o(\sqrt L).
$$

Part (b) transfers every fixed normalized [central moment](../../../../../../central-moment.md) of the truncated [prime omega function](../../../../../../prime-omega-function.md) to the independent [Bernoulli random variables](../../../../../../bernoulli-distribution.md) model. Indeed, its unnormalized error is at most $O_j(N^{2j/\varphi(N)-1})$, using $\sum_{p\le y}1\le y$, and this tends to zero for each fixed $j$. In the independent expansion, any singleton index has zero [expectation](../../../../../../expected-value.md); the leading contributions are pairings, giving exactly the [standard normal distribution](../../../../../../standard-normal-distribution.md) moments, while blocks of size at least three are negligible after normalization. The [method of moments in probability](../../../../../../method-of-moments-probability-theory.md), followed by the uniformly negligible truncation and centering errors, proves the [Erdős-Kac theorem](../../../../../../erdos-kac-theorem.md).

The same strategy proves the bounded-prime-weight form in part (a). Choose $\varphi(N)\to\infty$ slowly enough that $\varphi(N)=o(B(N))$. The omitted weighted contribution is $O(\varphi(N))$; its mean is likewise $O(\varphi(N))$, and its independent [variance](../../../../../../variance-split.md) is $O(\log\varphi(N)+1)=o(B(N)^2)$ by the [Mertens theorem for reciprocal primes](../../../../../../mertens-second-theorem.md). Hence the truncated model has the same normalization, and part (b) again transfers each fixed [central moment](../../../../../../central-moment.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
