<h1 id="2g/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Writing $x=\cos\theta$ and taking the [limit](../../../../../../limit-of-a-function.md) as $\theta\to0$ gives

$$
T_n'(1)=\lim_{\theta\to0}
\frac{n\sin(n\theta)}{\sin\theta}=n^2.
$$

Part (d), with $r=1$, shows that $T_n'$ is increasing on $[1,\infty)$, so

$$
T_n(x)-T_n(1)=\int_1^xT_n'(t)\,dt
\geq n^2(x-1).
$$

Since $T_n(1)=1$ and $n^2\geq n$,

$$
\boxed{T_n(x)\geq1+n(x-1)\quad(x\geq1)}.
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2G](../../2g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
