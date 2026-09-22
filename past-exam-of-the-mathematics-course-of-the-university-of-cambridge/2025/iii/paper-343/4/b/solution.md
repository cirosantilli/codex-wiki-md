<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the $X$ eigenbasis $|s_i\rangle_X$, $s_i\in\mathbb Z_2$, and put a dual qubit on every edge with $t_i=s_i+s_{i+1}\pmod2$. The [Kramers--Wannier intertwiner](../../../../../../kramers-wannier-intertwiner.md) is

$$
D=\sum_{s_1,\ldots,s_L}|s_1+s_2,\ldots,s_L+s_1\rangle_Z\langle s_1,\ldots,s_L|_X.
$$

An explicit [matrix product operator](../../../../../../matrix-product-operator.md) tensor is

$$
\boxed{A^{t,s}_{\alpha\beta}=\delta_{\alpha,s}\,\delta_{t,\alpha+\beta\ ({\rm mod}\ 2)}}.
$$

Contracting neighboring virtual indices $\beta_i=\alpha_{i+1}$ around the ring is the graphical MPO: each tensor copies its input bit to the left virtual leg and outputs the XOR of its two virtual legs.

Directly from the domain-wall definition,

$$
D(X_iX_{i+1})=\widetilde Z_{i+1/2}D,
\qquad
DZ_i=(\widetilde X_{i-1/2}\widetilde X_{i+1/2})D.
$$

Therefore $DH(\lambda)=\widetilde H(\lambda)D$, where

$$
\widetilde H(\lambda)=-\sum_i\widetilde Z_{i+1/2}+\lambda\sum_i\widetilde X_{i-1/2}\widetilde X_{i+1/2}.
$$

After exchanging $X$ and $Z$ and rescaling, this is the same Ising family at reciprocal coupling, so corresponding symmetry sectors have the same spectrum and $H(\lambda)$ is dual to $|\lambda|H(1/\lambda)$ up to the elementary sign conventions. In particular the Ising spectrum is self-dual at $|\lambda|=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 343](../../../paper-343-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
