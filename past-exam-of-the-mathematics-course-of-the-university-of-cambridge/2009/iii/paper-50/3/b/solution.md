<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Using base-two logarithms, define the [quantum conditional entropy](../../../../../../quantum-conditional-entropy.md) by

$$
\boxed{S(A\mid B)=S(\rho_{AB})-S(\rho_B).}
$$

The [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md), $S(AB)\leq S(A)+S(B)$, immediately gives $S(A\mid B)\leq S(A)$.

For the lower bound, purify $\rho_{AB}$ by an auxiliary system $C$. Complementary subsystems of a [pure state](../../../../../../pure-state.md) have the same nonzero reduced-state [eigenvalues](../../../../../../eigenvalue.md), by the [Schmidt decomposition](../../../../../../schmidt-decomposition.md). Hence $S(BC)=S(A)$ and $S(C)=S(AB)$. Applying [Subadditivity of Von Neumann entropy](../../../../../../subadditivity-of-von-neumann-entropy.md) to $BC$ gives

$$
S(A)=S(BC)\leq S(B)+S(C)=S(B)+S(AB).
$$

Rearranging yields $S(A\mid B)\geq-S(A)$. This is the relevant side of the [Araki–Lieb inequality](../../../../../../araki-lieb-inequality.md), here derived using purification.

Finally the [maximum entropy of a quantum state](../../../../../../maximum-entropy-of-a-quantum-state.md) gives $S(A)\leq\log_2\dim\mathcal H_A$. For example, this follows directly from

$$
D\left(\rho_A\middle\|\frac{I_A}{\dim\mathcal H_A}\right)
=\log_2\dim\mathcal H_A-S(A)\geq0
$$

by [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md). Combining the two bounds proves

$$
\boxed{|S(A\mid B)|\leq\log_2\dim\mathcal H_A.}
$$

Both signs can be attained: a maximally mixed $A$ independent of $B$ has the positive extreme, while a [maximally entangled state](../../../../../../maximally-entangled-state.md) with a sufficiently large $B$ has the negative extreme.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
