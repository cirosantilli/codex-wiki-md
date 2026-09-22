<h1 id="19h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
H_n=\mathbb E_A T_{BC}
$$

for the walk on $G_n$. Decompose $G_n$ into its three outer copies of $G_{n-1}$ and trace the walk only when it passes between distinct corner vertices of these copies. The [self-similarity](../../../../../../self-similarity.md) and reflection symmetry of the Sierpinski graph make this trace the simple random walk on $G_1$. It requires an expected five transitions to hit the two target outer corners.

Each coarse transition is an excursion across a copy of $G_{n-1}$ and has mean duration $H_{n-1}$. Applying the strong Markov property at the coarse stopping times gives

$$
H_n=5H_{n-1}.
$$

Since $H_1=5$, induction yields

$$
\boxed{\mathbb E_A T_{BC}=H_n=5^n}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
