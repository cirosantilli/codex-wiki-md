<h1 id="1/1/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [epigraph](../../../../../../../../epigraph.md) is

$$
\boxed{\operatorname{epi}E=\{(u,t)\in\mathcal U\times\mathbb R:E(u)\leq t\}.}
$$

Assume $E$ is $\tau$-[sequentially lower semicontinuous](../../../../../../../../sequential-lower-semicontinuity.md). If $(u_n,t_n)$ lies in the [epigraph](../../../../../../../../epigraph.md) and converges to $(u,t)$ in the [product topology](../../../../../../../../product-topology.md), then

$$
E(u)\leq\liminf E(u_n)\leq\lim t_n=t.
$$

The limit remains in the [epigraph](../../../../../../../../epigraph.md), so it is a [sequentially closed set](../../../../../../../../sequentially-closed-set.md).

Conversely, suppose the [epigraph](../../../../../../../../epigraph.md) is a [sequentially closed set](../../../../../../../../sequentially-closed-set.md) and [sequential lower semicontinuity](../../../../../../../../sequential-lower-semicontinuity.md) fails along $u_n\xrightarrow{\tau}u$. Choose a finite real number $a$ with $\liminf E(u_n)<a<E(u)$. There is a [subsequence](../../../../../../../../subsequence.md) along which $E(u_{n_j})\leq a$. Thus $(u_{n_j},a)$ lies in the [epigraph](../../../../../../../../epigraph.md) and converges to $(u,a)$, which does not lie there. This contradiction proves

$$
\boxed{E\text{ is }\tau\text{-sequentially lsc}
\ \Longleftrightarrow\ \operatorname{epi}E\text{ is sequentially closed}.}
$$

This is a sequential statement; identifying it with ordinary closedness requires an appropriate assumption on the [topology](../../../../../../../../topology-split.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [1](../../../../1.md)
5. [Paper 326](../../../../../paper-326-split.md)
6. [Iii](../../../../../split.md)
7. [2018](../../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../../split.md)
