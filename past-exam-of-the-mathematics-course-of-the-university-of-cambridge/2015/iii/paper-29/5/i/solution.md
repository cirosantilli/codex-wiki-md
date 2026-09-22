<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $A>0$, the first time $T_A=\inf\{n\geq0:X_n<-A\}$ is a [stopping time](../../../../../../stopping-time.md). On $\{T_A\geq1\}$, the [bounded increments](../../../../../../bounded-increments.md) assumption controls the overshoot:

$$
X_{T_A}\geq-A-M.
$$

Before that time, $X_n\geq-A$. Allowing the possibility $T_A=0$, the process

$$
Y_n=X_{n\wedge T_A}+A+M+X_0^-
$$

is a nonnegative [martingale](../../../../../../martingale-split.md). Indeed, the [stopped martingale in discrete time](../../../../../../stopped-martingale-in-discrete-time.md) is a [martingale](../../../../../../martingale-split.md), and the integrable $\mathcal F_0$-[measurable](../../../../../../measurability.md) variable $X_0^-$ is a constant-in-time [martingale](../../../../../../martingale-split.md). If $T_A=0$, nonnegativity follows from $X_0+X_0^-=X_0^+$. Its [expectations](../../../../../../expected-value.md) are constant and finite, so the [martingale convergence theorem](../../../../../../martingale-convergence-theorem.md) makes $Y_n$ converge to a finite value [almost surely](../../../../../../almost-sure-convergence.md).

On $\{T_A=\infty\}$ this proves finite convergence of $X_n$. Taking the countable union over positive integer $A$, we conclude that $X_n$ converges finitely on the event $\{\inf_nX_n> -\infty\}$. Apply the same reasoning to the [martingale](../../../../../../martingale-split.md) $-X$ to obtain finite convergence on $\{\sup_nX_n<\infty\}$.

Outside the event of finite convergence, both the infimum and the supremum of the sequence must therefore be infinite in the respective directions. Removing any finite initial segment cannot change this, because each of its values is finite. Hence

$$
\boxed{\mathbb P\bigl(\{X_n\text{ converges finitely}\}\cup\{\liminf_nX_n=-\infty,\ \limsup_nX_n=+\infty\}\bigr)=1.}
$$

This is the [bounded-increment martingale convergence-or-oscillation dichotomy](../../../../../../bounded-increment-martingale-convergence-or-oscillation-dichotomy.md). The $X_0^-$ term ensures the proof also covers an unbounded integrable initial value.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
