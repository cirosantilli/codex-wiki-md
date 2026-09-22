<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A two-dimensional [Lie algebra representation](../../../../../../lie-algebra-representation.md) already provides a counterexample. In the basis $e_1,e_2$ of $V=\mathbb C^2$, define

$$
\rho(x)=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad
\rho(y)=\rho(z)=0.
$$

The commutator $[\rho(x),\rho(y)]$ is zero, agreeing with $\rho(z)$; the other defining [Lie brackets](../../../../../../lie-bracket.md) also map to zero. Thus $\rho$ is a [Lie algebra homomorphism](../../../../../../lie-algebra-homomorphism.md), although it is not a [Faithful Lie algebra representation](../../../../../../faithful-lie-algebra-representation.md).

The line $L=\mathbb Ce_1$ is an [invariant subspace](../../../../../../invariant-subspace.md). Any complementary line has the form $\mathbb C(e_2+a e_1)$ for some $a\in\mathbb C$. But

$$
\rho(x)(e_2+a e_1)=e_1\notin\mathbb C(e_2+a e_1),
$$

so no complementary line is an [invariant subspace](../../../../../../invariant-subspace.md). Equivalently, every invariant line is killed by $\rho(x)$: its restriction to a line is a scalar, and its square is zero, forcing that scalar to be zero. A decomposition into two invariant lines would then force $\rho(x)=0$, a contradiction. This representation is therefore not a [semisimple representation](../../../../../../semisimple-representation.md). Thus

$$
\boxed{\text{Not every finite-dimensional representation of }\mathfrak h\text{ is completely reducible}.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
