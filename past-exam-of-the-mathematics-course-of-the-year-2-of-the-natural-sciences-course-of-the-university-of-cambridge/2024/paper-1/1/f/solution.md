<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Choose the symmetric [tensor field](../../../../../tensor-field.md)

$$
\Sigma_{kj}=(\partial_k\psi)(\partial_j\psi)-\frac12\delta_{kj}|\nabla\psi|^2.
$$

The [product rule](../../../../../product-rule.md) and equality of mixed [partial derivatives](../../../../../partial-derivative.md) give

$$
\begin{aligned}
\partial_k\Sigma_{kj}
&=(\nabla^2\psi)\partial_j\psi+(\partial_k\psi)\partial_k\partial_j\psi-\frac12\partial_j|\nabla\psi|^2\\
&=(\nabla^2\psi)\partial_j\psi.
\end{aligned}
$$

This is the [Euclidean scalar-gradient stress identity](../../../../../euclidean-scalar-gradient-stress-identity.md). Substitute it into part (e), and use $\Sigma_{ki}\hat n_k=(\partial_n\psi)\partial_i\psi-\tfrac12|\nabla\psi|^2\hat n_i$, where $\partial_n\psi=\hat{\mathbf n}\cdot\nabla\psi$. Reassembling the components gives the required pure [surface integral](../../../../../surface-integral.md):

$$
\boxed{\int_V\mathbf r\,\nabla\cdot[(\nabla^2\psi)\nabla\psi]\,dV=\int_S\left[\mathbf r(\nabla^2\psi)\partial_n\psi-(\partial_n\psi)\nabla\psi+\frac12|\nabla\psi|^2\hat{\mathbf n}\right]dS.}
$$

Sufficient smoothness of $\psi$ is understood for the displayed [derivatives](../../../../../derivative.md) and applications of the [divergence theorem](../../../../../divergence-theorem.md).

## ↑ Ancestors (13)

1. [F](../f.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
