<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Apply part (a) to the compact positive operator $T^*T$. Its positive square root $B=|T|$ is defined by multiplying each [eigenvector](../../../../../../eigenvector.md) of [eigenvalue](../../../../../../eigenvalue.md) $\lambda$ by $\sqrt\lambda$ and vanishing on the kernel. The [eigenvalues](../../../../../../eigenvalue.md) tend to zero, so $B$ is compact. For every $x$, $\|Tx\|^2=\langle T^*Tx,x\rangle=\|Bx\|^2$.

Consequently $U(Bx)=Tx$ is a well-defined isometry on $\operatorname{ran}B$. Extend it to the closure of that range and set it to zero on its orthogonal complement. This gives a [partial isometry](../../../../../../partial-isometry.md) with initial space $(\ker T)^\perp$, final space $\overline{\operatorname{ran}T}$, and

$$
\boxed{T=U|T|,\qquad\ker U=\ker T.}
$$

For uniqueness, the positive factor in any such [polar decomposition of a bounded operator](../../../../../../polar-decomposition-of-a-bounded-operator.md) satisfies $B^2=T^*T$. The positive-square-root uniqueness proved in 4(b) fixes $B$. The relation $U(Bx)=Tx$ then fixes $U$ on the dense subset $\operatorname{ran}B$ of its initial space and the kernel convention fixes it elsewhere. This proves uniqueness with the canonical initial-space condition. Without that condition the word “unique” would be false: $T=0$ can be written $U\cdot0$ with many different unitary $U$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
