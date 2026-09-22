<h1 id="11f/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Only even times contribute, and at time $2k$ the walk is at zero exactly when it has made $k$ steps in each direction. By [linearity of expectation](../../../../../../linearity-of-expectation.md),

$$
\mathbb E(V_{2n})
=\sum_{j=0}^{2n}\mathbb P(S_j=0)
=\sum_{k=0}^n\frac{\binom{2k}{k}}{4^k}.
$$

The [Stirling formula](../../../../../../stirling-formula.md) implies that

$$
\frac{\binom{2k}{k}}{4^k}\sim\frac1{\sqrt{\pi k}}.
$$

Hence there is a constant $c_0>0$ such that this term is at least $c_0/\sqrt{k}$ for every $k\geq1$, after decreasing $c_0$ to cover the finitely many small values. Therefore

$$
\mathbb E(V_{2n})
\geq c_0\sum_{k=1}^n\frac1{\sqrt{k}}
\geq c_0\int_1^{n+1}x^{-1/2}\,dx.
$$

The final expression is $2c_0(\sqrt{n+1}-1)$, so, after another adjustment for small $n$, there is a constant $c>0$ with

$$
\boxed{\mathbb E(V_{2n})\geq c\sqrt n}
$$

for every $n$. This is the lower bound recorded by [expected visits to the origin by a simple random walk](../../../../../../expected-visits-to-the-origin-by-a-simple-random-walk.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
