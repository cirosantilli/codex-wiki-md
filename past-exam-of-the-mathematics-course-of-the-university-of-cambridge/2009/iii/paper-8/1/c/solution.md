<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix a [Fredholm operator](../../../../../../fredholm-operator.md) $T$. Split its domain as $X\oplus N=(\ker T)^\perp\oplus\ker T$ and its target as $Y\oplus M=\operatorname{ran}T\oplus\ker T^*$. For a sufficiently small norm perturbation $R$, write

$$
T+R=\begin{pmatrix}A&B\\C&D\end{pmatrix},
$$

where $A:X\to Y$ remains invertible by the [Neumann series](../../../../../../neumann-series.md). Invertible triangular row and column operations reduce this matrix to

$$
\begin{pmatrix}A&0\\0&D-CA^{-1}B\end{pmatrix}.
$$

The second block maps the finite-dimensional space $N$ into $M$. Hence the perturbed operator has closed range, finite kernel and cokernel, and

$$
\operatorname{ind}(T+R)=\dim N-\dim M=\operatorname{ind}T,
$$

since the rank of that finite block cancels from the difference. Thus **the [Fredholm](../../../../../../fredholm-operator.md) set is open and its index is locally constant, hence norm continuous**.

If $S,T$ are [Fredholm](../../../../../../fredholm-operator.md), their product is [Fredholm](../../../../../../fredholm-operator.md) by multiplying their invertible images in the [Calkin algebra](../../../../../../calkin-algebra.md). For index additivity use the following finite-dimensional [exact sequence](../../../../../../exact-sequence.md):

$$
0\to\ker T\to\ker ST\xrightarrow{T}\ker S
\xrightarrow{q}\operatorname{coker}T\xrightarrow{S}\operatorname{coker}ST
\to\operatorname{coker}S\to0.
$$

Here $q$ is reduction modulo $\operatorname{ran}T$, the induced $S$-map sends $[x]$ to $[Sx]$, and the last map is the quotient by the larger range $\operatorname{ran}S$. These maps are well-defined. For example, $\ker q=\ker S\cap\operatorname{ran}T$ is the image of the preceding map. If $Sx\in\operatorname{ran}ST$, subtracting a suitable $Ty$ makes $x-Ty\in\ker S$, proving exactness at $\operatorname{coker}T$. The other positions follow directly from the definitions. Alternating dimensions in this exact sequence gives

$$
\boxed{\operatorname{ind}(ST)=\operatorname{ind}S+\operatorname{ind}T.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
