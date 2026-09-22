<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The unread measurement is the [pinching map](../../../../../../pinching-map.md) $\mathcal P(\rho)=\rho'=\sum_iP_i\rho P_i$, a [nonselective projective measurement](../../../../../../nonselective-projective-measurement.md). Its output is block diagonal and commutes with each $P_i$, so $\log\rho'$ also commutes with the projectors on its support.

First the [quantum relative entropy](../../../../../../quantum-relative-entropy.md) $D(\rho\Vert\rho')$ is finite. If $v$ lies in the kernel of $\rho'$, positivity gives

$$
0=\langle v|\rho'|v\rangle=\sum_i\|\rho^{1/2}P_iv\|^2.
$$

Every summand is zero; summing $\rho^{1/2}P_iv=0$ gives $\rho^{1/2}v=0$. Thus $\ker\rho'\subseteq\ker\rho$, equivalently $\operatorname{supp}\rho\subseteq\operatorname{supp}\rho'$.

The block-diagonal logarithm obeys $\sum_iP_i(\log\rho')P_i=\log\rho'$ on this support. Cyclicity of the trace therefore gives

$$
\operatorname{Tr}\rho\log\rho'=\operatorname{Tr}\left(\sum_iP_i\rho P_i\right)\log\rho'=\operatorname{Tr}\rho'\log\rho'.
$$

Consequently the [relative entropy of a pinched state](../../../../../../relative-entropy-of-a-pinched-state.md) is exactly the entropy increase:

$$
D(\rho\Vert\rho')=-S(\rho)-\operatorname{Tr}\rho\log_2\rho'=S(\rho')-S(\rho).
$$

By the proved [nonnegativity of quantum relative entropy](../../../../../../nonnegativity-of-quantum-relative-entropy.md) and its equality condition,

$$
\boxed{S(\rho')\geq S(\rho),\qquad S(\rho')=S(\rho)\ \Longleftrightarrow\ \rho'=\rho.}
$$

Equivalently, equality holds exactly when all off-diagonal blocks $P_i\rho P_j$ for $i\ne j$ already vanish, or when $\rho$ commutes with every measurement projector. This argument proves the equality condition even when the projectors are degenerate and the states singular.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
