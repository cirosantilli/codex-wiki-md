<h1 id="11g/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A real function on a [metric space](../../../../../../metric-space.md) is [uniformly continuous](../../../../../../uniform-continuity.md) if for every $\varepsilon>0$ there is a $\delta>0$ such that, simultaneously for all $x,y$, $d(x,y)<\delta$ implies $|f(x)-f(y)|<\varepsilon$. For a continuous function on a finite closed interval $[a,b]$, suppose this fails. Then there are $\varepsilon_0>0$ and pairs $x_n,y_n$ with $|x_n-y_n|<1/n$ but $|f(x_n)-f(y_n)|\ge\varepsilon_0$. By [compactness](../../../../../../compact-space.md), some subsequence $x_{n_j}$ converges to $x\in[a,b]$; then $y_{n_j}\to x$ too. [Continuity](../../../../../../continuous-function.md) contradicts the image separation. This proves the [Heine-Cantor theorem](../../../../../../heine-cantor-theorem.md) in this setting. Boundedness of the interval matters: $x^2$ on $[0,\infty)$ is a counterexample if “closed interval” includes unbounded intervals.

A function is [Lipschitz continuous](../../../../../../lipschitz-continuity.md) if some finite $K\ge0$ satisfies $|f(x)-f(y)|\le Kd(x,y)$ for every pair. Choosing $\delta=\varepsilon/(K+1)$ proves [uniform continuity](../../../../../../uniform-continuity.md).

The first assertion is **false**. Take $f(x)=\sin(x^2)$, which is bounded and continuous, and

$$
x_n=\sqrt{2\pi n+\pi/2},\qquad y_n=\sqrt{2\pi n+3\pi/2}.
$$

Then $f(x_n)=1$, $f(y_n)=-1$, while $y_n-x_n=\pi/(y_n+x_n)\to0$. This violates [uniform continuity](../../../../../../uniform-continuity.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11G](../../11g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
