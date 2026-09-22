<h1 id="2/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\delta>0$ and $M=\|f''\|_\infty>0$, differentiate the bound $F(h)=\sqrt6\delta/h+Mh/2$. Its derivative vanishes at $h_*^2=2\sqrt6\delta/M$, and $F''(h)>0$. Consequently, when $h_*<1/2$,

$$
\boxed{h_* =\left(\frac{2\sqrt6\delta}{M}\right)^{1/2},\qquad F(h_*)=\sqrt{2\sqrt6 M\delta}.}
$$

If $h_*\geq1/2$, the infimum on the open allowed interval is approached as $h\uparrow1/2$, rather than attained at an admissible endpoint. If $M=0$ and $\delta>0$, the bound decreases throughout the interval and has the same boundary behavior. At zero noise with $M>0$, its infimum is approached as $h\downarrow0$.

A practical [regularization parameter choice](../../../../../../../regularization-parameter-choice.md) independent of $M$ is

$$
\boxed{h(\delta)=\min\{1/4,\delta^\theta\},\qquad0<\theta<1.}
$$

It satisfies $h\to0$ and $\delta/h\to0$, hence gives a [convergent regularization of an inverse problem](../../../../../../../convergent-regularization-of-an-inverse-problem.md) on the domain of the [Volterra operator](../../../../../../../volterra-operator.md) inverse. This extends beyond $C^2$ exact data: if $f=Ku$ with $u\in L^2$, the differences are local averages of $u$. Extend $u$ by zero outside the interval; continuity of translations in $L^2$ makes these averages converge to $u$ on both halves. Together with $\|D_h(f^\delta-f)\|_2\leq\sqrt6\delta/h$ this proves convergence uniformly over the noise ball for every admissible exact datum.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2](../../../2.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
