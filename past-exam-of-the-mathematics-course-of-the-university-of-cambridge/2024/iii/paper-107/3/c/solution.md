<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set

$$
v_k=\frac{u_k}{\|u_k\|_{L^2(B_1)}}.
$$

Part (b.iii), applied on each compactly contained ball, gives uniform $C^{2,\alpha}$ bounds for $v_k$. A diagonal use of the [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) therefore gives a subsequence converging in $C^2(K)$ on every compact $K\Subset B_1$ to a $C^2$ function $w$.

The same estimate applied to $u_k$ gives $Du_k\to0$ locally uniformly because $\|u_k\|_2\to0$. Dividing the minimal-surface equation by $\|u_k\|_2$ shows that

$$
\left(\delta_{ij}-\frac{D_iu_kD_ju_k}{1+|Du_k|^2}\right)D_{ij}v_k=0.
$$

The coefficients converge locally uniformly to $\delta_{ij}$. Passing to the $C^2$ limit yields

$$
\boxed{\Delta w=0.}
$$

**Thus $w$ is harmonic and the required normalized subsequence converges to it locally in $C^2$.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
