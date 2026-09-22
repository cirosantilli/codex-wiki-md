<h1 id="12f/solution">Solution</h1>

↑ **Parent:** [12F](../12f.md)

Interpret random choice of coin as equal prior probabilities, and the tosses as [independent](../../../../../independent-random-variables.md) conditional on the chosen coin. Let $H_2$ denote two heads. The conditional probabilities are $P(H_2\mid A)=1/16$ and $P(H_2\mid B)=9/16$. For [posterior coin selection from repeated tosses](../../../../../posterior-coin-selection-from-repeated-tosses.md), [Bayes' theorem](../../../../../bayes-theorem.md) gives

$$
\boxed{P(B\mid H_2)=\frac{(1/2)(9/16)}{(1/2)(1/16)+(1/2)(9/16)}=\frac9{10}.}
$$

The tosses need not be unconditionally [independent](../../../../../independent-random-variables.md), because the same hidden coin is used twice. If the coin-choice prior were instead $P(B)=\pi$, the answer would be $9\pi/(1+8\pi)$; equal choice gives the stated $9/10$.

For [nondecreasing uniform samples](../../../../../nondecreasing-uniform-samples.md) in the lottery, all $n^r$ ordered samples have equal probability by the [discrete uniform distribution](../../../../../discrete-uniform-distribution.md) and [independence](../../../../../independent-random-variables.md). A nondecreasing sample is uniquely specified by its multiplicities $k_1,\ldots,k_n\geq0$, with $k_1+\cdots+k_n=r$. The [stars and bars](../../../../../stars-and-bars-combinatorics.md) argument places $n-1$ separators among $r$ identical markers, giving $\binom{r+n-1}{n-1}$ multiplicity vectors. There is exactly one nondecreasing ordered sample for each such vector, so **the probability is**

$$
\boxed{\frac{\binom{r+n-1}{n-1}}{n^r}=\frac{\binom{r+n-1}{r}}{n^r}.}
$$

This counts samples with ties correctly; multiplying a single strictly increasing count by $r!$ would not handle the repeated values.

## ↑ Ancestors (10)

1. [12F](../12f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
