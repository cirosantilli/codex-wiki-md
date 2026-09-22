<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

The equation fails for general nonnested sigma-algebras. On the four-point space $\Omega=\{1,2,3,4\}$ with uniform probability, let

$$
A=\{1,2\},\qquad B=\{1,2,3\},
\qquad \mathcal G=\sigma(A),\qquad\mathcal H=\sigma(B),
$$

and take $X=\mathbf1_A$. The intersection $\mathcal G\cap\mathcal H$ is trivial, so

$$
\mathbb E[X\mid\mathcal G\cap\mathcal H]=\frac12.
$$

But $X$ is $\mathcal G$-measurable and

$$
\mathbb E[\mathbb E[X\mid\mathcal G]\mid\mathcal H]
=\mathbb E[X\mid\mathcal H]
=\frac23\mathbf1_B,
$$

which is zero on $B^c$ and is not almost surely $1/2$. This exhibits the failure of [iterated conditional expectation over nonnested sigma-algebras](../../../../../../iterated-conditional-expectation-over-nonnested-sigma-algebras.md).

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
