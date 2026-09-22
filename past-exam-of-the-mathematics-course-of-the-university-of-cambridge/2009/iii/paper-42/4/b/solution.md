<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use mostly-minus [metric signature](../../../../../../metric-signature.md), $\eta=\operatorname{diag}(1,-1,-1,-1)$. The [Weyl sigma matrices](../../../../../../weyl-sigma-matrices.md) are $\sigma^\mu=(I,\boldsymbol\sigma)$ and $\bar\sigma^\mu=(I,-\boldsymbol\sigma)$, with the three [Pauli matrices](../../../../../../pauli-matrices.md)

$$
\sigma_1=\begin{pmatrix}0&1\\1&0\end{pmatrix},\quad \sigma_2=\begin{pmatrix}0&-i\\i&0\end{pmatrix},\quad \sigma_3=\begin{pmatrix}1&0\\0&-1\end{pmatrix}.
$$

The [Pauli matrix multiplication law](../../../../../../pauli-matrix-multiplication-law.md) $\sigma_i\sigma_j=\delta_{ij}I+i\epsilon_{ijk}\sigma_k$ immediately gives $\sigma^\mu\bar\sigma^\nu+\sigma^\nu\bar\sigma^\mu=2\eta^{\mu\nu}I$: the $00$ case is $2I$, the mixed cases cancel, and the spatial cases give $-2\delta_{ij}I$. The spinor indices of $\sigma^\mu_{\alpha\dot\beta}$ express the correspondence between a [Lorentz four-vector](../../../../../../four-vector.md) and a Hermitian $2\times2$ matrix. For $X=x^0I+x^i\sigma_i$, $\det X=(x^0)^2-|\mathbf x|^2$; $X\mapsto MXM^\dagger$ preserves this [determinant](../../../../../../determinant.md) for $M\in\mathrm{SL}(2,\mathbb C)$, yielding the [Lorentz spinor double cover](../../../../../../lorentz-spinor-double-cover.md).

In [four-dimensional N=1 supersymmetry](../../../../../../four-dimensional-n-1-supersymmetry.md), the odd [supercharges](../../../../../../supersymmetry-generator.md) $Q_\alpha$ and $\bar Q_{\dot\alpha}=Q_\alpha^\dagger$ transform as conjugate [Weyl spinors](../../../../../../weyl-spinor.md). Their [Super-Poincaré algebra](../../../../../../super-poincare-algebra.md) is

$$
\boxed{\{Q_\alpha,\bar Q_{\dot\beta}\}=2\sigma^\mu_{\alpha\dot\beta}P_\mu,\qquad \{Q_\alpha,Q_\beta\}=\{\bar Q_{\dot\alpha},\bar Q_{\dot\beta}\}=0,\qquad [P_\mu,Q_\alpha]=[P_\mu,\bar Q_{\dot\alpha}]=0.}
$$

The ordinary translation and Lorentz generators satisfy the [Poincare algebra](../../../../../../poincare-algebra.md), and the Lorentz generators act on the [supercharges](../../../../../../supersymmetry-generator.md) by the corresponding [group representations](../../../../../../group-representation.md) on [Weyl spinors](../../../../../../weyl-spinor.md). Tracing the mixed [anticommutator](../../../../../../anticommutator.md) gives $P_0=\frac14\sum_\alpha\{Q_\alpha,Q_\alpha^\dagger\}$, proving [energy positivity in global supersymmetry](../../../../../../energy-positivity-in-global-supersymmetry.md). For a massive rest-frame state, $P_\mu=(M,0,0,0)$, the rescaled charges $Q_\alpha/\sqrt{2M}$ obey the [canonical anticommutation relations](../../../../../../canonical-anticommutation-relations.md). Acting with their adjoints builds a [supermultiplet](../../../../../../supermultiplet.md) containing states of alternating [fermion parity](../../../../../../fermion-parity.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
