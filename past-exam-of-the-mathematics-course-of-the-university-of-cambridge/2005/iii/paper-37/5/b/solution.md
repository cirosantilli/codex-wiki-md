<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $D=\mathcal C_{\mathrm{ev}}$, and write $\mathcal C_{\mathrm{odd}}=t+D$ for any odd-weight word $t\in\mathcal C_H$. The parity functional on the four-dimensional binary [linear code](../../../../../../linear-code.md) $\mathcal C_H$ is nonzero, so its kernel $D$ has dimension three and its other fibre is the coset $t+D$. For example $t=(1,\ldots,1)$ belongs to the standard length-seven [Hamming code](../../../../../../hamming-code.md) and has odd [Hamming weight](../../../../../../hamming-weight.md). Denote the two logical basis states by $|\psi_0\rangle$ and $|\psi_1\rangle$, corresponding to these two cosets. The eight computational [orthonormal basis](../../../../../../orthonormal-basis.md) vectors in each sum are distinct, so both logical states have norm one; their disjoint supports make them [orthogonal](../../../../../../orthogonal-vectors.md).

For a binary vector $w\in\mathbb F_2^7$, define the product of [Pauli Z gates](../../../../../../pauli-z-gate.md)

$$
Z(w)=\bigotimes_{j=1}^7 Z_j^{w_j},\qquad
Z(w)|x\rangle=(-1)^{w\cdot x}|x\rangle,
$$

where the dot product is computed modulo two. The key diagonal overlap, with $t_0=0$ and $t_1=t$, is

$$
\langle\psi_a|Z(w)|\psi_a\rangle
=\frac{(-1)^{w\cdot t_a}}8\sum_{x\in D}(-1)^{w\cdot x}.
$$

If $w\in D^\perp$, every summand is one. If $w\notin D^\perp$, choose $x_0\in D$ with $w\cdot x_0=1$. Translation $x\mapsto x+x_0$ permutes $D$ and negates every summand. The sum must then be zero. Thus

$$
\sum_{x\in D}(-1)^{w\cdot x}
=\begin{cases}8,&w\in D^\perp,\\0,&w\notin D^\perp.\end{cases}
$$

Off-diagonal logical overlaps vanish for every $w$:

$$
\langle\psi_0|Z(w)|\psi_1\rangle=0,
$$

because a diagonal [Pauli operator](../../../../../../pauli-operator.md) cannot move a computational basis word from one coset to the disjoint other coset.

The possible errors are $E_0=I$ and $E_j=Z(e_j)$ for $j=1,\ldots,7$. Set $e_0=0$. Each [phase flip](../../../../../../pauli-z-gate.md) is its own adjoint and inverse, so

$$
E_i^\dagger E_j=Z(e_i+e_j).
$$

If $i\ne j$, the vector $e_i+e_j$ is nonzero and has [Hamming weight](../../../../../../hamming-weight.md) one or two. By the given [dual code](../../../../../../dual-code.md) identity $D^\perp=\mathcal C_H$ and the minimum [Hamming distance](../../../../../../hamming-distance.md) three of the [Hamming code](../../../../../../hamming-code.md), it cannot belong to $D^\perp$. Hence all its diagonal logical overlaps vanish. If $i=j$, the product is the identity and its logical overlaps are $\delta_{ab}$. Combining both cases gives

$$
\boxed{\langle\psi_a|E_i^\dagger E_j|\psi_b\rangle
=\delta_{ij}\delta_{ab}\quad(a,b\in\{0,1\},\ i,j\in\{0,\ldots,7\}).}
$$

This proves the [Knill--Laflamme condition](../../../../../../knill-laflamme-condition.md) with an identity error-overlap [matrix](../../../../../../matrix.md), not merely a possibly degenerate scalar [matrix](../../../../../../matrix.md). In particular the eight two-dimensional error subspaces $E_i\mathcal X_{\mathrm{Steane}}$ are mutually [orthogonal](../../../../../../orthogonal-vectors.md). This is precisely [nondegenerate phase-flip correction in the Steane code](../../../../../../nondegenerate-phase-flip-correction-in-the-steane-code.md).

To exhibit recovery rather than only the criterion, let $P$ be the [orthogonal projector](../../../../../../orthogonal-projection.md) onto the code and $P_i=E_iPE_i^\dagger$. The [projective measurement](../../../../../../projective-measurement.md) consisting of these eight mutually [orthogonal projectors](../../../../../../orthogonal-projection.md), completed by $I-\sum_iP_i$, determines which error occurred. For an arbitrary encoded [pure state](../../../../../../pure-state.md) $|\chi\rangle=\alpha|\psi_0\rangle+\beta|\psi_1\rangle$ affected by $E_j$, outcome $j$ occurs with certainty and leaves $E_j|\chi\rangle$ unchanged. Applying $E_j$ again recovers $|\chi\rangle$. The outcome gives the [error syndrome](../../../../../../error-syndrome.md) and does not reveal $\alpha$ or $\beta$, so recovery preserves logical [quantum superpositions](../../../../../../quantum-superposition.md).

An equivalent explicit [error syndrome](../../../../../../error-syndrome.md) uses three commuting X-type [stabilizer generators](../../../../../../stabilizer-generator.md). Choose a [parity-check matrix](../../../../../../parity-check-matrix.md) for $\mathcal C_H$ with the seven different nonzero binary columns:

$$
H=\begin{pmatrix}
1&0&1&0&1&0&1\\
0&1&1&0&0&1&1\\
0&0&0&1&1&1&1
\end{pmatrix}.
$$

Its rows span $\mathcal C_H^\perp=D$. For a row $h_l$, the operator $X(h_l)=\bigotimes_jX_j^{(h_l)_j}$ permutes each of $D$ and $t+D$, and therefore has eigenvalue $+1$ on both logical states. A [phase flip](../../../../../../pauli-z-gate.md) at position $j$ changes its eigenvalue to $(-1)^{H_{lj}}$, since $X(h_l)Z_j=(-1)^{H_{lj}}Z_jX(h_l)$. Measuring the three commuting [stabilizer generators](../../../../../../stabilizer-generator.md) gives the $j$th column of $H$ as a binary [syndrome](../../../../../../syndrome.md); no error gives the zero column. All eight outcomes are different, and applying the identified $Z_j$ restores the code state. Measuring these [stabilizer generators](../../../../../../stabilizer-generator.md) never distinguishes the two logical states.

Finally, if a noise [Kraus operator](../../../../../../kraus-operator.md) is a coherent linear combination $F=\sum_jc_jE_j$, the same syndrome measurement separates its mutually [orthogonal](../../../../../../orthogonal-vectors.md) components $c_jE_j|\chi\rangle$. Conditional recovery returns $|\chi\rangle$ in every nonzero branch. Linearity then also corrects any [quantum channel](../../../../../../quantum-channel.md) whose [Kraus operators](../../../../../../kraus-operator.md) lie in this span. The argument therefore corrects arbitrary unknown single-site [phase flips](../../../../../../pauli-z-gate.md) nondegenerately, including coherent phase-error amplitudes, rather than only a known error on a basis codeword.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
