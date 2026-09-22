<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The PDF's displayed zero-mode term has no derivative. Read literally, $d_0\cdot d_0$ vanishes for classical [Grassmann variables](../../../../../../grassmann-variable.md) and supplies no zero-mode symplectic structure. The subsequent canonical-algebra requests therefore require the standard kinetic term $\frac i2d_0\cdot\dot d_0$. We use that intended correction explicitly; the rest of the displayed action fixes the nonzero-mode normalization.

The [Ramond level operator](../../../../../../ramond-level-operator.md), with vacuum-annihilating [normal ordering](../../../../../../normal-ordering.md), is

$$
\boxed{\widehat N_R=\sum_{k=1}^\infty\left(\widehat\alpha_{-k}\cdot\widehat\alpha_k+k\widehat d_{-k}\cdot\widehat d_k\right).}
$$

The canonical oscillator relations, for transverse indices $I,J$, are

$$
\boxed{[\widehat\alpha_m^I,\widehat\alpha_n^J]=m\delta_{m+n,0}\delta^{IJ},\qquad
\{\widehat d_m^I,\widehat d_n^J\}_+=\delta_{m+n,0}\delta^{IJ},\qquad[\widehat\alpha_m^I,\widehat d_n^J]=0.}
$$

The hermiticity convention is $\alpha_k^\dagger=\alpha_{-k}$ and $d_k^\dagger=d_{-k}$. The commuting bosonic zero mode is supplied by the center-of-mass [momentum](../../../../../../momentum.md). For $k>0$, define $a_k^I=\alpha_k^I/\sqrt k$ and $f_k^I=d_k^I$. Their [bosonic occupation numbers](../../../../../../bosonic-occupation-number.md) are $0,1,2,\ldots$ and their [fermionic occupation numbers](../../../../../../fermionic-occupation-number.md) are $0,1$. Therefore, on the [Fock space](../../../../../../fock-space.md) generated from an [oscillator vacuum](../../../../../../oscillator-vacuum.md),

$$
\boxed{N=\sum_{k\geq1,I}k(n^B_{kI}+n^F_{kI})\in\mathbb Z_{\geq0}.}
$$

Equivalently, creation operators raise the level by $k$, since $[N_R,\alpha_{-k}^I]=k\alpha_{-k}^I$ and $[N_R,d_{-k}^I]=kd_{-k}^I$. The zero modes commute with $N_R$ and do not change the level. The multiplier imposes

$$
\boxed{M^2=-p^2=2\pi T N,}
$$

so the $N=0$ states are massless. In the [Ramond sector](../../../../../../ramond-sector.md) the bosonic and fermionic oscillator zero-point contributions cancel, consistently with the stated zero intercept. The massless ground states are spacetime spinors, as the [Ramond zero-mode Clifford algebra](../../../../../../ramond-zero-mode-clifford-algebra.md) now shows.

Normalize $\gamma^I=\sqrt2\widehat d_0^I$. Then

$$
\boxed{\{\gamma^I,\gamma^J\}_+=2\delta^{IJ},\qquad(\gamma^I)^\dagger=\gamma^I.}
$$

Let $v=|0\rangle\ne0$. Each positive-frequency bosonic annihilator commutes with $\gamma^I$, while each fermionic annihilator anticommutes with it. Applying either annihilator to $\gamma^Iv$ therefore gives zero. Thus all eight $\gamma^Iv$ are [oscillator vacua](../../../../../../oscillator-vacuum.md). For real $a_I$, the hermitian operator $A=\sum_Ia_I\gamma^I$ satisfies $A^2=(\sum_Ia_I^2)\mathbf1$, so

$$
\left\|\sum_Ia_I\gamma^Iv\right\|^2=\left(\sum_Ia_I^2\right)\|v\|^2.
$$

This proves the [real independence of Clifford-generated vectors](../../../../../../real-independence-of-clifford-generated-vectors.md), and hence their **linear independence over $\mathbb R$**.

The same argument applies to the nonzero vacuum $\gamma^1v$, because $(\gamma^1)^2=1$. It gives eight real-linearly independent [oscillator vacua](../../../../../../oscillator-vacuum.md) $\gamma^I\gamma^1v$. They include $v$ itself, at $I=1$. Products of two zero modes preserve vacuum annihilation just as products of one do.

For the [chirality matrix](../../../../../../chirality-matrix.md) $\gamma_9=\gamma^1\gamma^2\cdots\gamma^8$, reversing eight anticommuting factors introduces $(-1)^{8\cdot7/2}=1$. Hence

$$
\boxed{\gamma_9^\dagger=\gamma_9,\qquad\gamma_9^2=\mathbf1.}
$$

Moving any $\gamma^I$ through the other seven factors also gives $\gamma_9\gamma^I=-\gamma^I\gamma_9$. If $\gamma_9v=v$, then

$$
\boxed{\gamma_9\gamma^Iv=-\gamma^Iv,\qquad\gamma_9\gamma^I\gamma^1v=\gamma^I\gamma^1v.}
$$

The first collection has negative [chirality](../../../../../../chirality-physics.md); the second has positive [chirality](../../../../../../chirality-physics.md). If $u_+$ and $u_-$ have these respective [chiralities](../../../../../../chirality-physics.md), hermiticity gives $\langle u_+,u_-\rangle=\langle\gamma_9u_+,u_-\rangle=\langle u_+,\gamma_9u_-\rangle=-\langle u_+,u_-\rangle$, so they are orthogonal. Combining the two real-independent collections therefore gives **at least sixteen real-linearly independent [oscillator vacua](../../../../../../oscillator-vacuum.md)**, eight in each [chirality](../../../../../../chirality-physics.md).

The real qualification in the question matters: the particular eight vectors generated from an arbitrary complex $v$ need not be independent over $\mathbb C$. Nevertheless the [dimension bound from paired Clifford involutions](../../../../../../dimension-bound-from-paired-clifford-involutions.md) also follows from the full [Clifford algebra](../../../../../../clifford-algebra.md). Define four commuting hermitian involutions $J_j=i\gamma^{2j-1}\gamma^{2j}$, $j=1,\ldots,4$. Their joint spectral projections preserve the vacuum space, so it contains a nonzero common eigenvector $w$. Multiplication by $\gamma^{2j-1}$ flips the eigenvalue of $J_j$ and leaves the other three eigenvalues unchanged. The sixteen products obtained by independently choosing whether to apply these four odd-indexed [Gamma matrices](../../../../../../gamma-matrices.md) to $w$ consequently have distinct joint eigenvalue quadruples. They are nonzero, mutually orthogonal [oscillator vacua](../../../../../../oscillator-vacuum.md). Thus the unprojected vacuum space also has **complex dimension at least sixteen**, with eight states of each [chirality](../../../../../../chirality-physics.md) in the minimal representation. A further chiral projection is an additional physical restriction, not part of the oscillator-vacuum conditions here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 306](../../../paper-306-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
