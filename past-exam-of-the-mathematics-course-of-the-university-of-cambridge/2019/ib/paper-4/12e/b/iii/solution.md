<h1 id="12e/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The space is not compact because it is not [complete](../../../../../../../complete-metric-space.md). For $n\geq2$, define the continuous function

$$
f_n(t)=\begin{cases}
0,&0\leq t\leq\frac12-\frac1n,\\
\frac n2\left(t-\frac12+\frac1n\right),&\frac12-\frac1n<t<\frac12+\frac1n,\\
1,&\frac12+\frac1n\leq t\leq1.
\end{cases}
$$

These functions converge in the [L1 norm](../../../../../../../l1-norm.md) to the [step function](../../../../../../../step-function.md) $h=\boldsymbol1_{(1/2,1]}$, because $f_n-h$ is supported on an interval of length $2/n$ and bounded in [absolute value](../../../../../../../absolute-value.md) by one. They are consequently Cauchy for the metric $d$, since for sufficiently close pairs the outer minimum with $1$ does nothing.

If $(f_n)$ converged in this metric to some $f\in C[0,1]$, it would also converge to $f$ in $L^1$. Uniqueness of an $L^1$ limit would give $f=h$ almost everywhere. Continuity would then force $f=0$ on $[0,1/2)$ and $f=1$ on $(1/2,1]$, which is impossible at $1/2$. Thus this Cauchy sequence has no limit in $C[0,1]$, while every compact metric space is complete.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [12E](../../../12e.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ib](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
