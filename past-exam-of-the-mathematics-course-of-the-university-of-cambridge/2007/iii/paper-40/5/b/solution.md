<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In an ideal continuous-price [English auction](../../../../../../english-auction.md), staying active until one's private valuation is optimal: dropping earlier can forgo positive surplus, while staying later risks paying more than the car is worth. The highest-valued buyer therefore wins, paying the price at which the other buyer drops out, namely $\min(V_1,V_2)$.

For $0\leq t\leq1$, independence gives $\Pr(\min(V_1,V_2)>t)=(1-t)^2$. Integrating this tail probability gives

$$
\boxed{R_b=\mathbb E\min(V_1,V_2)=\int_0^1(1-t)^2\,dt=\frac13.}
$$

“Pays his bid” in this ascending auction does not mean that the winning buyer pays his full valuation; the competing buyer's dropout determines the winning price.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
