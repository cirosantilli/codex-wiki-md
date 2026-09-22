<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [uniform hypergraph Ramsey number](../../../../../../uniform-hypergraph-ramsey-number.md) $R^{(r)}(k)$ is the least $N$ such that every red-blue colouring of the $r$-element subsets of an $N$-element set contains a $k$-element set all of whose $r$-subsets have one colour.

Colour each triple of an $N$-element set independently and uniformly red or blue. For a fixed $k$-set, the probability of being monochromatic is

$$
2^{1-\binom k3}.
$$

The expected number of monochromatic $k$-sets is therefore

$$
\binom Nk2^{1-\binom k3}
\le2^{1+k\log_2(eN/k)-\binom k3}.
$$

Take $N=\lfloor2^{ck^2}\rfloor$ with any sufficiently small absolute $c>0$. The exponent is negative for large $k$, since its leading terms are $ck^3-k^3/6$. Thus some colouring has no monochromatic $k$-set, proving

$$
\boxed{R^{(3)}(k)\ge2^{ck^2}.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
