<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [identity-by-descent sharing of inbred full siblings](../../../../../../identity-by-descent-sharing-of-inbred-full-siblings.md), with $J$ the maximum number of copies that can be paired across the children as [identical by descent](../../../../../../identity-by-descent.md). If two copies within one child have the same ancestral origin, they still count as two copies when both can be paired.

With probability $3/4$ the cousin parents share no ancestral copy. Conditional on this event, their children have ordinary [Mendelian IBD sharing of full siblings](../../../../../../mendelian-ibd-sharing-of-full-siblings.md), namely $(1/4,1/2,1/4)$. With probability $1/4$, the parental copies can be labelled $(A,B)$ and $(A,C)$, with $A,B,C$ distinct ancestral origins. Each child independently receives one of $AA,AB,AC,BC$, with probability $1/4$ each. Among the sixteen ordered child pairs, $AA$ paired with $BC$ in either order gives $J=0$; four equal genotype-origin pairs give $J=2$; the remaining ten give $J=1$. The mixture is

$$
\boxed{\begin{aligned}P(J=0)&=\frac34\frac14+\frac14\frac18=\frac7{32},\\P(J=1)&=\frac34\frac12+\frac14\frac58=\frac{17}{32},\\P(J=2)&=\frac34\frac14+\frac14\frac14=\frac14.\end{aligned}}
$$

These are inbred children, so the three sharing probabilities do not retain all within-child identities. The full [Jacquard identity coefficients](../../../../../../jacquard-identity-coefficients.md) are $(1,0,2,1,2,1,15,30,12)/64$. In particular, their [kinship coefficient](../../../../../../kinship-coefficient.md) is $9/32$; applying the outbred formula $(P(J=1)+2P(J=2))/4$ here would be incorrect.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
