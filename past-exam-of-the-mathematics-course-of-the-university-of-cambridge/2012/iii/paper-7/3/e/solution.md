<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

We first prove the needed [Fredholm alternative for a compact operator](../../../../../../fredholm-alternative.md) without assuming self-adjointness. If $C$ is compact, the [finite-rank approximation theorem for compact operators on a Hilbert space](../../../../../../finite-rank-approximation-theorem-for-compact-operators-on-a-hilbert-space.md) follows directly by covering the compact closure of $C$'s unit-ball image by finitely many balls of radius $\varepsilon$, spanning their centers by a finite-dimensional space $E$, and using the [orthogonal projection](../../../../../../orthogonal-projection.md) $P_E$. Then $\|C-P_EC\|\leq\varepsilon$.

Choose a finite-rank $F$ with $\|C-F\|<1$, put $E_0=C-F$, and factor

$$
I-C=(I-E_0)(I-G),\qquad G=(I-E_0)^{-1}F.
$$

The first factor is invertible by the [Neumann series](../../../../../../neumann-series.md), and $G$ has finite rank. With $V=\operatorname{ran}G$ and $H=V\oplus V^\perp$, the second factor has the triangular form

$$
I-G=
\begin{pmatrix}I_V-G|_V&-G|_{V^\perp}\\0&I_{V^\perp}\end{pmatrix}.
$$

It is injective precisely when the finite-dimensional block $I_V-G|_V$ is injective, and onto precisely when that block is onto. These properties are equivalent in finite dimension. This proves that $I-C$ is injective if and only if it is onto; in that case its inverse is bounded.

For $\lambda\ne0$, apply this result to $C=K/\lambda$. If $\lambda$ lies in the [spectrum of a bounded operator](../../../../../../spectrum-of-a-bounded-operator.md) $K$, then $K-\lambda I$ is not invertible, hence is not injective. Therefore **every nonzero spectral point of $K$ is an eigenvalue**. On its [eigenspace](../../../../../../eigenspace.md) $E_\lambda$, the operator $K$ equals $\lambda I$. Compactness of $K$ would make the closed unit ball of $E_\lambda$ compact after dividing by $\lambda$; part (a) forces $\dim E_\lambda<\infty$.

It remains to rule out infinitely many distinct [eigenvalues](../../../../../../eigenvalue.md) away from zero. Suppose $|\lambda_n|\geq\varepsilon>0$ are distinct, with respective eigenvectors $v_n$. Distinct eigenvalues give linearly independent eigenvectors. Let $V_n=\operatorname{span}(v_1,\ldots,v_n)$ and choose a unit vector $h_n\in V_n\cap V_{n-1}^\perp$. Since $V_n$ is invariant and $(K-\lambda_nI)V_n\subset V_{n-1}$,

$$
Kh_n=\lambda_nh_n+w_n,\qquad w_n\in V_{n-1}.
$$

For $m<n$, $Kh_m\in V_{n-1}$, and [orthogonality](../../../../../../orthogonal-vectors.md) gives $\|Kh_n-Kh_m\|\geq|\lambda_n|\geq\varepsilon$. This contradicts compactness. Thus for each $\varepsilon>0$ there are only finitely many distinct spectral points with modulus at least $\varepsilon$.

Taking $\varepsilon=1/j$ shows that the nonzero [spectrum](../../../../../../spectrum-functional-analysis.md) is countable; if it is infinite, its distinct elements can be enumerated as a sequence tending to zero. Since the [spectrum](../../../../../../spectrum-functional-analysis.md) is closed, zero then also belongs to it. In an infinite-dimensional space zero belongs to the spectrum even if there are only finitely many nonzero spectral points: an invertible compact $K$ would make $I=K^{-1}K$ compact, contradicting part (a). **The only possible accumulation point is zero, and every nonzero eigenspace is finite-dimensional.** Zero need not be an eigenvalue. The argument uses invariant spans, not an orthogonal eigenbasis, which is unavailable for a general non-self-adjoint compact operator.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
