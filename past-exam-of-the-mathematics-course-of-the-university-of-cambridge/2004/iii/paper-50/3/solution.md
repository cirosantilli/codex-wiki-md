<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the unheaded extended-algebra request, fix the central-charge normalization explicitly:

$$
\{Q_\alpha^A,(Q_\beta^B)^\dagger\}=2\delta^{AB}\sigma^\mu_{\alpha\dot\beta}P_\mu,
\qquad
\{Q_\alpha^A,Q_\beta^B\}=2\epsilon_{\alpha\beta}Z^{AB},
\qquad Z^{AB}=-Z^{BA}.
$$

The central charges are scalar numbers on an irreducible massive representation. A [unitary skew-diagonalization of an antisymmetric matrix](../../../../../unitary-skew-diagonalization-of-an-antisymmetric-matrix.md) puts $Z$ into two-by-two blocks $\begin{pmatrix}0&z_r\\-z_r&0\end{pmatrix}$ and, for odd $\mathcal N$, a leftover zero entry. Since this change of [supercharge](../../../../../supersymmetry-generator.md) basis is unitary, it preserves the mixed [anticommutator](../../../../../anticommutator.md). Go to the rest frame $P^\mu=(M,0,0,0)$.

For one block set $q_\alpha=Q_\alpha^1$ and $r_\alpha=\epsilon_{\alpha\gamma}(Q_\gamma^2)^\dagger$, with $\epsilon_{12}=1$. Direct use of the algebra gives

$$
\{q_\alpha,q_\beta^\dagger\}=\{r_\alpha,r_\beta^\dagger\}=2M\delta_{\alpha\beta},\qquad
\{q_\alpha,r_\beta^\dagger\}=2z\delta_{\alpha\beta}.
$$

Write $z=|z|e^{i\varphi}$ and form the combinations suggested by the hint:

$$
A_\alpha=\frac{q_\alpha+e^{i\varphi}r_\alpha}{\sqrt2},\qquad
B_\alpha=\frac{q_\alpha-e^{i\varphi}r_\alpha}{\sqrt2}.
$$

Then

$$
\{A_\alpha,A_\beta^\dagger\}=2(M+|z|)\delta_{\alpha\beta},\qquad
\{B_\alpha,B_\beta^\dagger\}=2(M-|z|)\delta_{\alpha\beta},\qquad
\{A_\alpha,B_\beta^\dagger\}=0.
$$

Each diagonal [anticommutator](../../../../../anticommutator.md) has nonnegative expectation because it is the sum of squared [norms](../../../../../norm.md) of an operator and its adjoint. Therefore $M-|z_r|\ge0$ for every block, proving

$$
\boxed{M\ge\max_r|z_r|.}
$$

If the algebra is instead written with $\{Q,Q\}=\epsilon Z$ without the factor two, the same proof gives $M\ge\tfrac12\max_r|Z_r|$. This is the normalization used by some definitions of the [BPS bound in supersymmetry](../../../../../bps-bound-in-supersymmetry.md); the physical bound is unchanged by the naming of the central charge.

A massive [BPS state](../../../../../bps-state.md) saturates at least one block bound. At saturation $\{B_\alpha,B_\alpha^\dagger\}=0$, so both $B_\alpha$ and $B_\alpha^\dagger$ annihilate every state in its multiplet. The two complex inactive oscillators are four preserved real supersymmetries per saturated block. If $r$ blocks saturate, the preserved fraction is $r/\mathcal N$ and only $2\mathcal N-2r$ complex fermionic oscillators remain active. For a spin-$j$ [Clifford vacuum](../../../../../clifford-vacuum.md),

$$
\boxed{\dim\mathcal H_{\mathrm{BPS}}=(2j+1)2^{\,2\mathcal N-2r},}
$$

compared with $(2j+1)2^{2\mathcal N}$ for a long massive multiplet. Thus [BPS states](../../../../../bps-state.md) have an exact mass-charge relation, preserve part of the [supersymmetry](../../../../../supersymmetry-split.md), and belong to shortened representations. A physical CPT-invariant spectrum may additionally require the conjugate-charge multiplet. The short representation protects the saturated mass relation while it exists; it does not prohibit a decay at a threshold where central-charge phases align and the sum of daughter masses equals the bound.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
