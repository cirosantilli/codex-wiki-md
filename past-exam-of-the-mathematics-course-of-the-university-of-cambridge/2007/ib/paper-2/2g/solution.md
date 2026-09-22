<h1 id="2g/solution">Solution</h1>

↑ **Parent:** [2G](../2g.md)

A [Euclidean domain](../../../../../euclidean-domain.md) is an [integral domain](../../../../../integral-domain.md) $R$ with a function $\delta:R\setminus\{0\}\to\mathbb Z_{\ge0}$ such that, for every $a\in R$ and nonzero $b\in R$, there are $q,r\in R$ satisfying $a=bq+r$, with either $r=0$ or $\delta(r)<\delta(b)$.

For the [integers](../../../../../integer.md), take $\delta(b)=|b|$. Given $a$ and $b\ne0$, put $m=|b|$ and choose the integer $q_0=\lfloor a/m\rfloor$. Then $a=mq_0+r$ with $0\le r<m$. Setting $q=q_0$ when $b>0$ and $q=-q_0$ when $b<0$ gives $a=bq+r$. A nonzero remainder has $\delta(r)=r<|b|=\delta(b)$, and the [integers](../../../../../integer.md) are an [integral domain](../../../../../integral-domain.md). Thus **$\mathbb Z$ is a Euclidean domain with Euclidean function $|b|$**.

## ↑ Ancestors (10)

1. [2G](../2g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
