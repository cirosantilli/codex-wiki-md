<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Here the intended space must consist of **bounded** [linear operators](../../../../../linear-operator.md), namely [Hilbert-Schmidt operators](../../../../../hilbert-schmidt-operator.md). The printed restriction to “all linear mappings” is insufficient. To see this, choose $v\in X$ outside the algebraic [linear span](../../../../../linear-span.md) of $(e_k)$, for example $v=\sum_{k\geq1}2^{-k}e_k$. Extend the linearly independent family $\{e_k:k\geq1\}\cup\{v\}$ to a [Hamel basis](../../../../../basis.md). Define a [linear functional](../../../../../linear-functional.md) $\phi$ on this [Hamel basis](../../../../../basis.md) by $\phi(v)=1$ and zero on every other basis vector, and extend it linearly. Then the everywhere-defined [linear operator](../../../../../linear-operator.md) $Rx=\phi(x)e_1$ satisfies

$$
Re_k=0\quad(k\geq1),\qquad Rv=e_1\ne0.
$$

Its printed column sum is zero although $R\ne0$. More explicitly, $v_N=\sum_{k=1}^N2^{-k}e_k\to v$ but $R(v-v_N)=e_1$ for every $N$. Thus $R$ is discontinuous; it has no everywhere-defined [adjoint operator](../../../../../adjoint-operator.md) of the bounded kind used in the question. This proves [finite column sum does not imply boundedness](../../../../../finite-column-sum-does-not-imply-boundedness.md). We use $T\in\mathcal B(X)$ in the intended argument below.

By the [Parseval identity for a Hilbertian basis](../../../../../parseval-identity-for-a-hilbertian-basis.md) for $(e_j)$, followed by the [adjoint operator](../../../../../adjoint-operator.md) identity and then the [Parseval identity for a Hilbertian basis](../../../../../parseval-identity-for-a-hilbertian-basis.md) for $(h_k)$,

$$
\begin{aligned}
\sum_k\|Th_k\|^2
&=\sum_k\sum_j|\langle Th_k,e_j\rangle|^2\\
&=\sum_j\sum_k|\langle h_k,T^*e_j\rangle|^2\\
&=\sum_j\|T^*e_j\|^2.
\end{aligned}
$$

The interchange is valid by [Tonelli's theorem](../../../../../tonelli-theorem.md) for nonnegative double [series](../../../../../series-mathematics.md), even before finiteness is known. Repeating with $h_k=e_k$ shows that the right side also equals $\sum_k\|Te_k\|^2$. Hence

$$
\boxed{\sum_k\|Th_k\|^2=\sum_j\|T^*e_j\|^2=\sum_k\|Te_k\|^2.}
$$

In particular the [Hilbert-Schmidt norm](../../../../../hilbert-schmidt-norm.md) is independent of the [Hilbertian basis](../../../../../hilbertian-basis.md), and $\|T^*\|_2=\|T\|_2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analysis II course of the University of Oxford](../../../../split.md)
6. [Functional analysis II course of the University of Oxford](../../../../../functional-analysis-ii-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
