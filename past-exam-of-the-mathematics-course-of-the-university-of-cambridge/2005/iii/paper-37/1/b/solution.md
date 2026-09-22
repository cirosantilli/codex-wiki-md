<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let a [density operator](../../../../../../density-matrix.md) on a [Hilbert space](../../../../../../hilbert-space-split.md) $\mathcal H_S$ have the [spectral decomposition](../../../../../../spectral-decomposition.md)

$$
\rho_S=\sum_{j=1}^r\lambda_j|j\rangle_S\langle j|,
\qquad\lambda_j>0,\qquad\sum_j\lambda_j=1.
$$

Introduce an auxiliary [Hilbert space](../../../../../../hilbert-space-split.md) $\mathcal H_R$ with an [orthonormal basis](../../../../../../orthonormal-basis.md) containing $r$ vectors $|j\rangle_R$, and set

$$
|\Omega\rangle_{SR}=\sum_{j=1}^r\sqrt{\lambda_j}|j\rangle_S|j\rangle_R.
$$

This vector has norm one. Its [partial trace](../../../../../../partial-trace.md) is

$$
\operatorname{Tr}_R|\Omega\rangle\langle\Omega|
=\sum_{j,k}\sqrt{\lambda_j\lambda_k}|j\rangle_S\langle k|\langle k|j\rangle_R
=\rho_S.
$$

This explicitly constructs a [purification of a density operator](../../../../../../purification-of-a-density-operator.md). The same construction works for an arbitrary trace-class [density operator](../../../../../../density-matrix.md): its nonzero [eigenvalues](../../../../../../eigenvalue.md) form a finite or countable summable family, and the displayed vector converges in the [Hilbert space](../../../../../../hilbert-space-split.md) norm. The entropy inequality below is understood with finite [Von Neumann entropies](../../../../../../von-neumann-entropy-split.md), avoiding undefined differences of infinities.

Apply this construction with $S=AB$ to obtain a joint [pure state](../../../../../../pure-state.md) on $ABC$. The [Schmidt decomposition](../../../../../../schmidt-decomposition.md) across $AB:C$, $A:BC$ and $B:AC$ respectively gives

$$
S(AB)=S(C),\qquad S(A)=S(BC),\qquad S(B)=S(AC).
$$

Now apply [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md) to the [reduced density matrices](../../../../../../reduced-density-matrix.md) on $BC$ and $AC$:

$$
S(A)=S(BC)\leq S(B)+S(C),\qquad
S(B)=S(AC)\leq S(A)+S(C).
$$

These inequalities say $S(A)-S(B)\leq S(C)$ and $S(B)-S(A)\leq S(C)$. Replacing $S(C)$ by $S(AB)$ proves the [Araki–Lieb inequality](../../../../../../araki-lieb-inequality.md):

$$
\boxed{|S(A)-S(B)|\leq S(A,B).}
$$

The subadditivity used here concerns the actual reduced [density operators](../../../../../../density-matrix.md), rather than statistical independence. In particular it follows from [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md), since

$$
D(\rho_{BC}\Vert\rho_B\otimes\rho_C)
=S(\rho_B)+S(\rho_C)-S(\rho_{BC})\geq0,
$$

and similarly for $AC$. Thus no independence assumption on the [purification of a density operator](../../../../../../purification-of-a-density-operator.md) is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
