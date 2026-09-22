<h1 id="28k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For expected final capital, the [Bellman equation](../../../../../../bellman-equation.md) is linear in wealth, with one-period factor $\mathbb E(1+pR)=1+p\mathbb ER$. Therefore **invest everything when the mean return is positive, nothing when it is negative, and any fraction when it is zero**. For $N=1$ this agrees with the yield objective.

For $N>1$, the root objective is concave and penalizes losses, so its optimal fraction need not be $1$ even when the mean is positive. For example, if $\mathbb P(R=-1)>0$ and $\mathbb ER>0$, the left [derivative](../../../../../../derivative.md) of $\mathbb E(1+pR)^r$ at $1$ is $-\infty$, while its right [derivative](../../../../../../derivative.md) at $0$ is positive; the optimum lies strictly between $0$ and $1$. If $\mathbb ER\leq0$, [Jensen inequality](../../../../../../jensen-s-inequality.md) gives $\mathbb E(1+pR)^r\leq(1+p\mathbb ER)^r\leq1$, so $p=0$ is optimal. Thus **the root objective can favor partial investment over the all-in policy**.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28K](../../28k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
