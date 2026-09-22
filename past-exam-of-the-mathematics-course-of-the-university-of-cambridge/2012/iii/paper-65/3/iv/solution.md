<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Put $u=\varepsilon/2$. The state is well defined for $0\leq\varepsilon\leq2$, with eigenvalues $1-u,u$. The first state is pure and has zero [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md), so the exact difference is

$$
\boxed{|S(\rho)-S(\sigma)|=h_2(\varepsilon/2),\qquad
h_2(u)=-u\log_2u-(1-u)\log_2(1-u).}
$$

This is the [entropy of a binary diagonal qubit mixture](../../../../../../entropy-of-a-binary-diagonal-qubit-mixture.md). Its [trace distance](../../../../../../trace-distance.md) from the [pure state](../../../../../../pure-state.md) is $u$, not $\varepsilon$. An explicit elementary upper bound follows from $-(1-u)\ln(1-u)\leq u$:

$$
\boxed{|S(\rho)-S(\sigma)|\leq
\min\left\{1,\frac{\varepsilon}{2}\log_2\frac{2e}{\varepsilon}\right\}
\quad(0<\varepsilon\leq2).}
$$

At zero the limit is zero. For small $\varepsilon$, the sharp exact answer behaves as $(\varepsilon/2)\log_2(2/\varepsilon)+\varepsilon/(2\ln2)+O(\varepsilon^2)$, displaying the logarithmic continuity of entropy near a [pure state](../../../../../../pure-state.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
