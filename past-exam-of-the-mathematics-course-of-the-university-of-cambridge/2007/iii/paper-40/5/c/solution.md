<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

With [reserve price](../../../../../../reserve-price.md) $r\in[0,1]$, an [English auction](../../../../../../english-auction.md) makes no sale if both valuations are below $r$. If exactly one exceeds it, the price is $r$; if both exceed it, the price is their minimum. Thus

$$
\begin{aligned}
R_c(r)
&=r\,[2r(1-r)]+\int_r^1 2t(1-t)\,dt\\
&=\frac13+r^2-\frac43r^3.
\end{aligned}
$$

The first term accounts for one qualifying buyer, and the integral uses the density $2(1-t)$ of the smaller valuation. Differentiation gives $R_c'(r)=2r(1-2r)$. It increases up to $r=1/2$ and decreases afterwards, while the endpoints give $1/3$ and zero. Therefore

$$
\boxed{r_*=\frac12,\qquad R_c^*=\frac5{12}.}
$$

The strict sale condition at the reserve changes only a probability-zero event.

## ↑ Ancestors (11)

1. [C](../c.md)
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
