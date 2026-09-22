<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $|\psi\rangle=\alpha|0\rangle+\beta|1\rangle$ and $t=e^{i\theta}$. Before measurement, the three [controlled-NOT gates](../../../../../../controlled-not-gate.md) map a computational-basis component $|x,y,0\rangle$ to

$$
|x,y\mathbin\oplus x,y\mathbin\oplus x\rangle.
$$

The measured bit is therefore $b=y\mathbin\oplus x$. For $b=0$, the unnormalized state of the first qubit is

$$
\frac1{\sqrt2}(\alpha|0\rangle+t\beta|1\rangle)
=\frac1{\sqrt2}P(\theta)|\psi\rangle.
$$

For $b=1$, it is

$$
\frac1{\sqrt2}(t\alpha|0\rangle+\beta|1\rangle)
=\frac t{\sqrt2}P(-\theta)|\psi\rangle.
$$

Each branch has probability $1/2$; after normalization and removal of the irrelevant global phase $t$, the two outputs are

$$
\boxed{P(\theta)|\psi\rangle\quad\text{and}\quad
P(-\theta)|\psi\rangle}
$$

with equal probability. This is [probabilistic phase-gate injection](../../../../../../probabilistic-phase-gate-injection.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
