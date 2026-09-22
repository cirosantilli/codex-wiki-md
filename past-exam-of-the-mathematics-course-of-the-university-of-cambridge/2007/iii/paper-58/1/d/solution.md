<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For one fixed [POVM](../../../../../../positive-operator-valued-measure.md) repeated on independently prepared copies, the [Born rule](../../../../../../born-rule.md) gives $m$ outcome probabilities with one normalization constraint. An arbitrary mixed qubit [density operator](../../../../../../density-matrix.md) has three independent real parameters,

$$
\rho=\frac12(I+\mathbf r\cdot\boldsymbol\sigma),\qquad |\mathbf r|\leq1.
$$

The probability map is affine in $\mathbf r$. It can be injective on the full [Bloch ball](../../../../../../bloch-ball.md) only if $m-1\geq3$. If its rank is smaller, a nonzero undetected direction gives two nearby physical Bloch vectors with the same probabilities. Hence $m\geq4$ for an [informationally complete POVM](../../../../../../informationally-complete-povm.md).

To attain this bound, take the four directions

$$
\mathbf n_1=\frac{(1,1,1)}{\sqrt3},\quad
\mathbf n_2=\frac{(1,-1,-1)}{\sqrt3},\quad
\mathbf n_3=\frac{(-1,1,-1)}{\sqrt3},\quad
\mathbf n_4=\frac{(-1,-1,1)}{\sqrt3}.
$$

They are the vertices of a [regular tetrahedron](../../../../../../regular-tetrahedron.md). The [tetrahedral qubit POVM](../../../../../../tetrahedral-qubit-povm.md) has effects $E_i=(I+\mathbf n_i\cdot\boldsymbol\sigma)/4$, each positive and rank one, and $\sum_iE_i=I$. The observed probabilities are

$$
p_i=\operatorname{Tr}(\rho E_i)=\frac{1+\mathbf r\cdot\mathbf n_i}{4}.
$$

Since $\sum_i\mathbf n_i=0$ and $\sum_i\mathbf n_i\mathbf n_i^T=4I_3/3$, they recover the state by

$$
\boxed{\mathbf r=3\sum_{i=1}^4p_i\mathbf n_i,\qquad m_{\min}=4.}
$$

This is the minimum for a single fixed measurement family. If the wording permits changing measurement settings between groups of copies, three binary projective measurements of the three Pauli observables also suffice, each with $m=2$. That procedure is [informationally complete three-observable qubit tomography](../../../../../../informationally-complete-three-observable-qubit-tomography.md), and it does not contradict the four-outcome bound for one fixed POVM. Tomography estimates probabilities statistically from many copies; a finite sample does not determine an arbitrary continuous state exactly.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
