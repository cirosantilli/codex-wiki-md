<h1 id="15d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

In a region with no current, the [Ampère-Maxwell equation](../../../../../../ampere-s-circuital-law.md) and [Faraday's law](../../../../../../faraday-s-law-of-induction.md) are

$$
\nabla\times\mathbf B=\mu_0\epsilon_0\frac{\partial\mathbf E}{\partial t},
\qquad
\nabla\times\mathbf E=-\frac{\partial\mathbf B}{\partial t}.
$$

Therefore

$$
\begin{aligned}
\frac{\partial w}{\partial t}
&=\epsilon_0\mathbf E\mathbin{\cdot}\partial_t\mathbf E
+\frac1{\mu_0}\mathbf B\mathbin{\cdot}\partial_t\mathbf B\\
&=\frac1{\mu_0}\left[
\mathbf E\mathbin{\cdot}(\nabla\times\mathbf B)
-\mathbf B\mathbin{\cdot}(\nabla\times\mathbf E)\right]\\
&=-\frac1{\mu_0}\nabla\mathbin{\cdot}(\mathbf E\times\mathbf B),
\end{aligned}
$$

where the last line uses the [divergence and curl of a cross product](../../../../../../divergence-and-curl-of-a-cross-product.md). Thus [Poynting's theorem](../../../../../../poynting-theorem.md) takes the form

$$
\boxed{\frac{\partial w}{\partial t}+\nabla\mathbin{\cdot}\mathbf S=0},
\qquad
\boxed{\mathbf S=\frac1{\mu_0}\mathbf E\times\mathbf B}.
$$

The vector $\mathbf S$ is the [Poynting vector](../../../../../../poynting-vector.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [15D](../../15d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
