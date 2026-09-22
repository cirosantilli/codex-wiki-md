<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $L_n=\operatorname{span}\{e_1,\ldots,e_n\}$ and let $P_n$ be its [orthogonal projection](../../../../../../orthogonal-projection.md). For $z\in\mathbb C$, define

$$
\gamma_n(z)^2
=\lambda_{\min}\!\left(
(1+|z|^2)I_n-\bar z\,P_nAP_n-z\,P_nA^*P_n
\right).
$$

Because $A$ is [unitary](../../../../../../unitary-operator.md),

$$
\gamma_n(z)
=\inf_{\substack{x\in L_n\\\|x\|=1}}\|(A-zI)x\|.
$$

The displayed finite [Hermitian matrix](../../../../../../hermitian-operator.md) uses only finitely many matrix entries of $A$, and its least eigenvalue can be approximated by an [arithmetic algorithm in the SCI hierarchy](../../../../../../arithmetic-algorithm-in-the-sci-hierarchy.md).

As $L_n$ increases densely,

$$
\gamma_n(z)\downarrow
\inf_{\|x\|=1}\|(A-zI)x\|.
$$

A [unitary operator](../../../../../../unitary-operator.md) is [normal](../../../../../../normal-operator.md), so the [spectral theorem for normal operators on a separable Hilbert space](../../../../../../spectral-theorem-for-normal-operators-on-a-separable-hilbert-space.md) identifies the limit as

$$
\operatorname{dist}(z,\operatorname{Sp}(A)).
$$

The functions $\gamma_n$ are continuous and decrease to a continuous function on the compact unit circle. The [Dini theorem](../../../../../../dini-s-theorem.md) therefore gives uniform convergence there.

Take successively finer rational meshes $G_n$ around $\mathbb T$. From the finitely computed values of $\gamma_n$, retain the mesh minima in the comparison neighborhoods whose radii are $\gamma_n(z)$; equivalently, use the standard local-minimum construction for a decreasing approximation to a distance function. Call the resulting finite set $\Gamma_n(A)$. Uniform convergence and the shrinking mesh imply

$$
\boxed{\Gamma_n(A)\longrightarrow\operatorname{Sp}(A)}
$$

in [Hausdorff distance](../../../../../../hausdorff-distance.md). Every operation at stage $n$ is finite and arithmetic, so $(\Gamma_n)$ is the required one-limit sequence.

There is no finite-stage certificate that the whole output has the correct Hausdorff error: the convergence of $\gamma_n$ has no uniform computable rate over all unitary operators, and unseen matrix entries can still reveal a missing spectral component. A small computed residual can certify that an individual output point lies near the spectrum, but it cannot verify that $\Gamma_n(A)$ covers all of $\operatorname{Sp}(A)$. Thus the full finite-stage output is not verifiable without additional information.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 358](../../../paper-358-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
