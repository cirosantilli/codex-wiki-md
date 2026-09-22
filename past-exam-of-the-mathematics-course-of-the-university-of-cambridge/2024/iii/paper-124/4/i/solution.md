<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A language $L$ belongs to [RP](../../../../../../rp-complexity.md) when a polynomial-time [randomized algorithm](../../../../../../randomized-algorithm.md) rejects every $x\notin L$ and accepts every $x\in L$ with probability at least $1/2$.

Amplify the algorithm on length-$n$ inputs with $n+1$ independent repetitions, accepting if any repetition accepts. Its error on each positive input is at most $2^{-(n+1)}$, while it still never accepts a negative input. Choose all random bits for all repetitions in advance. By the [union bound](../../../../../../boole-s-inequality.md), the probability that this one fixed choice fails on at least one of the at most $2^n$ positive strings is at most

$$
2^n2^{-(n+1)}=\frac12.
$$

Thus some random string works simultaneously for every input of length $n$. Hardwire that string into the polynomial-time computation and compile it into a [Boolean circuit](../../../../../../boolean-circuit.md). The resulting [polynomial-size circuit family](../../../../../../polynomial-size-circuit-family.md) decides $L$, proving

$$
\boxed{\mathbf{RP}\subseteq\mathbf P/\mathrm{poly}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
