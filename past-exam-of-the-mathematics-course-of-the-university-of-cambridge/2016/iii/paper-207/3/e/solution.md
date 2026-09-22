<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

At time zero the [chain-binomial epidemic model](../../../../../../chain-binomial-epidemic-model.md) has $B(0)\sim\operatorname{Bin}(N,\beta)$ and $C(0)\sim\operatorname{Bin}(1,1-e^{-\gamma})$, independently. The update gives $I(1)=1+B(0)-C(0)$. Since $B(0)\ge0$ and $C(0)\le1$, extinction at day one is equivalent to $B(0)=0$ and $C(0)=1$. Hence **the one-day extinction probability** is

$$
\boxed{\mathbb P(I(1)=0)=(1-\beta)^N(1-e^{-\gamma}).}
$$

This is the exact probability for the printed discrete-time approximation, which requires $\beta I(t)\delta t\in[0,1]$ wherever used. It should not be substituted for the distinct continuous-time extinction calculation.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
