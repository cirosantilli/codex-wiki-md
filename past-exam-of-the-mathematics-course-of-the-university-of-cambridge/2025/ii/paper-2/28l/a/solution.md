<h1 id="28l/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The jump chain moves away from zero with probability $2/3$ and towards zero with probability $1/3$ on either half-line. Starting from $1$, the probability that this biased walk ever hits zero is $(1/3)/(2/3)=1/2$, and the same holds starting from $-1$. Thus the return probability to zero is $1/2<1$. The jump chain, and hence $X$, is transient.

It is also explosive. The transient jump chain visits zero only finitely often. After its last visit it stays on one half-line, and the strong law for its increments gives

$$
\frac{|Y_n|}{n}\longrightarrow\frac13
$$

almost surely. In particular, eventually $|Y_n|\geq n/6$. Conditional on the jump-chain path, the mean total remaining holding time is

$$
\sum_n\frac1{q_{Y_n}}
=\sum_n3^{-|Y_n|}<\infty.
$$

The sum of the actual nonnegative holding times is therefore finite almost surely, so infinitely many jumps occur in finite time.

Despite this, the chain has an invariant distribution in the continuous-time balance-equation sense $\pi Q=0$. Detailed balance across the edge from zero to one gives $\pi_1=\pi_0/2$, and on each half-line it gives

$$
\frac{\pi_{i+1}}{\pi_i}
=\frac{q_{i,i+1}}{q_{i+1,i}}=\frac23.
$$

By symmetry and normalization,

$$
\boxed{
\pi_0=\frac14,
\qquad
\pi_i=\pi_{-i}=\frac18\left(\frac23\right)^{i-1}quad(i\geq1).}
$$

This example also shows why, for an explosive chain, existence of an invariant distribution need not imply positive recurrence.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28L](../../28l.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
