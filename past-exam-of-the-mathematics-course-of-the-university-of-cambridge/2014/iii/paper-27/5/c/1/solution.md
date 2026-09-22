<h1 id="5/c/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Let $S$ denote this maximum and put $\tau=\tau(-b)$. [Brownian motion](../../../../../../../brownian-motion-split.md) reaches $-b$ almost surely: the [Brownian reflection principle](../../../../../../../reflection-principle-wiener-process.md) gives crossing probability $2\mathbb P(W_t<-b)\to1$. Continuity gives $W_\tau=-b$, with the strict-crossing infimum interpreted as in part (b). The process

$$
M_t=\frac{W_{t\wedge\tau}+b}{b}
$$

is a continuous nonnegative [local martingale](../../../../../../../local-martingale.md) starting at one and tending to zero. Its maximum is $1+S/b$. Apply part (b) at $a=1+x/b$, for $x>0$:

$$
\mathbb P(S>x)=\frac b{b+x},\qquad\mathbb P(S\leq x)=\frac x{b+x}.
$$

Differentiating gives the [maximum before a lower Brownian barrier](../../../../../../../maximum-before-a-lower-brownian-barrier.md) density

$$
\boxed{f_S(x)=\frac b{(b+x)^2}\mathbf1_{\{x>0\}}.}
$$

The tail tends to one as $x\downarrow0$, so there is no atom at zero. The density integrates to one.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [C](../../c.md)
3. [5](../../../5.md)
4. [Paper 27](../../../../paper-27-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
