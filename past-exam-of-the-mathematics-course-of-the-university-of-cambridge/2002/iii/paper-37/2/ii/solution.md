<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The probability of a first event of type $A$ in $(u,u+du)$ is the probability $S(u)$ of still being at risk times $h_A(u)du$. Thus its [cumulative incidence function](../../../../../../cumulative-incidence-function.md) is

$$
\boxed{F_A(t)=\int_0^t h_A(u)\exp\{-H_A(u)-H_B(u)\}\,du.}
$$

Similarly $F_B(t)=\int_0^t h_B(u)S(u)\,du$. In general $F_A(t)\ne1-e^{-H_A(t)}$: that latter expression ignores the competing removal caused by $B$ and instead describes a [net survival](../../../../../../net-survival.md) complement.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
