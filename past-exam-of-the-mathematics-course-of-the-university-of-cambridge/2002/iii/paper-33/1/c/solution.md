<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the normalized three-qubit states $|G_\pm\rangle=(|000\rangle\pm|111\rangle)/\sqrt2$. The [Shor code](../../../../../../shor-code.md) has logical basis

$$
\boxed{|0_L\rangle=|G_+\rangle^{\otimes3},\qquad
|1_L\rangle=|G_-\rangle^{\otimes3}.}
$$

It encodes $\alpha|0\rangle+\beta|1\rangle$ as $\alpha|0_L\rangle+\beta|1_L\rangle$, preserving the unknown amplitudes by a [linear isometry](../../../../../../linear-isometry-of-hilbert-spaces.md). It concatenates a three-block [phase-flip repetition code](../../../../../../phase-flip-repetition-code.md) with the three-qubit [bit-flip repetition code](../../../../../../bit-flip-repetition-code.md) inside each block. Six [stabilizer generators](../../../../../../stabilizer-generator.md), $Z_1Z_2,Z_2Z_3,Z_4Z_5,Z_5Z_6,Z_7Z_8,Z_8Z_9$, test bit errors inside the blocks. The other two [stabilizer generators](../../../../../../stabilizer-generator.md) are

$$
A=X_1X_2X_3X_4X_5X_6,\qquad
B=X_4X_5X_6X_7X_8X_9.
$$

All eight commute and have eigenvalue $+1$ on both logical basis states. They define the $[[9,1,3]]$ [stabilizer code](../../../../../../stabilizer-code.md). The inner checks identify single bit flips, and the outer checks identify a block phase flip; combined they also correct a [Pauli Y gate](../../../../../../pauli-y-gate.md) error, since $Y=iXZ$.

For the requested [phase flip](../../../../../../pauli-z-gate.md), a $Z$ on any one qubit interchanges $|G_+\rangle$ and $|G_-\rangle$ in its block. It commutes with the six $Z$-pair checks. It anticommutes with $A$ or $B$ exactly when its block is contained in that check. The [Shor-code phase-flip syndrome](../../../../../../shor-code-phase-flip-syndrome.md) is therefore

$$
\begin{array}{c|c|c}
\text{error block}&(A,B)\text{ outcomes}&\text{recovery}\\\hline
\text{none}&(+1,+1)&I\\
1&(-1,+1)&Z_1\\
2&(-1,-1)&Z_4\\
3&(+1,-1)&Z_7
\end{array}
$$

A [projective measurement](../../../../../../projective-measurement.md) of the two commuting checks yields the displayed [error syndrome](../../../../../../error-syndrome.md) without learning $\alpha$ or $\beta$: both logical components have the same check eigenvalues after the error. Applying the indicated [Pauli Z gate](../../../../../../pauli-z-gate.md) restores every encoded [quantum state](../../../../../../quantum-state.md).

The correction is genuinely degenerate. For $i,j$ in the same block, $Z_iZ_j$ fixes both $|000\rangle$ and $|111\rangle$, so $Z_iZ_jP=P$ and consequently $Z_iP=Z_jP$. In particular $Z_1$ and $Z_2$ are distinct physical errors but have identical action on every code state; their image subspaces coincide, not merely their observed syndrome labels. In the [Knill--Laflamme condition](../../../../../../knill-laflamme-condition.md) for $I,Z_1,\ldots,Z_9$, the error [Gram matrix](../../../../../../gram-matrix.md) has $C_{00}=1$, $C_{0i}=C_{i0}=0$, and

$$
C_{ij}=\begin{cases}1,&i,j\text{ in the same block},\\0,&i,j\text{ in different blocks}.
\end{cases}
$$

The zero overlaps between different blocks follow because a phase flip changes a different pattern of orthogonal $G_+,G_-$ factors; cross-logical overlaps also vanish. Thus $C$ consists of one $1\times1$ block and three all-ones $3\times3$ blocks and has rank four, not ten. This both proves correctability of the entire single-phase-error span and exhibits its degeneracy. A coherent sum of phase errors in one block has the same logical action with its coefficients summed, so inability to locate the individual qubit loses no logical information. **The two block checks suffice to correct every single phase flip, even though the within-block errors are indistinguishable.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
