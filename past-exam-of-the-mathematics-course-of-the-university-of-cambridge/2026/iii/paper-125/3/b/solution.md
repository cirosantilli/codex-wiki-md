<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $h=\log H$ and set $h_x(P)=h(x(P))$ for $P\ne O$, with $h_x(O)=0$. The given degree-four morphism and part (a) imply that a constant $C$ exists with

$$
|h_x(2P)-4h_x(P)|\leq C
$$

for every $P\in E(\mathbb Q)$. Define

$$
\widehat h(P)=\frac12\lim_{r\to\infty}4^{-r}h_x(2^rP).
$$

To check the limit, put $a_r=4^{-r}h_x(2^rP)$. Then

$$
|a_{r+1}-a_r|\leq C4^{-r-1}.
$$

The geometric series converges, so $(a_r)$ is Cauchy and the limit exists. This is the [canonical height of an elliptic curve](../../../../../../canonical-height-of-an-elliptic-curve.md); shifting the sequence by one index immediately gives $\widehat h(2P)=4\widehat h(P)$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
