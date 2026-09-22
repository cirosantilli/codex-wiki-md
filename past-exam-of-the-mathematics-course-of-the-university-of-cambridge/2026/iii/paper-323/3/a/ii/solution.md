<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\Delta=p\rho_0-(1-p)\rho_1$. The success probability of $Q$ is

$$
P_{\rm succ}(Q)
=p\operatorname{Tr}(Q\rho_0)
+(1-p)\operatorname{Tr}[(I-Q)\rho_1]
=1-p+\operatorname{Tr}(Q\Delta).
$$

Write the spectral decomposition $\Delta=\Delta_+-\Delta_-$. For every effect $0\leq Q\leq I$,

$$
\operatorname{Tr}(Q\Delta)
\leq\operatorname{Tr}\Delta_+,
$$

with equality when $Q$ projects onto the positive spectral subspace, with arbitrary action on the kernel. Since $\operatorname{Tr}\Delta=2p-1$ and $\|\Delta\|_1=\operatorname{Tr}\Delta_++\operatorname{Tr}\Delta_-$, the [Holevo–Helstrom theorem](../../../../../../../holevo-helstrom-theorem.md) follows:

$$
\boxed{P_{\rm succ}^*
=\frac12(1+\|\Delta\|_1)},
\qquad
\boxed{P_{\rm err}^*
=\frac12(1-\|\Delta\|_1)}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2026](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
