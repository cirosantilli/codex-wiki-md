<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For fixed $t$, put $M_t=\sup_{0\leq s\leq t}\|f(s)\|_2$. A [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) in time strengthens the organization of the estimate in (c):

$$
\|\tau g(t)\|_2^2
\leq C^2t\int_0^t\|g(s)\|_2^2\,ds.
$$

Start with $\|\tau f(t)\|_2^2\leq C^2t^2M_t^2$. If the printed bound holds for $n-1$, then

$$
\|\tau^nf(t)\|_2^2
\leq C^2t\int_0^t
\frac{C^{2n-2}s^{2n-2}}{1\cdot3\cdots(2n-3)}M_t^2\,ds
=\frac{C^{2n}t^{2n}}{1\cdot3\cdots(2n-1)}M_t^2.
$$

Taking square roots proves **the [iterated Cauchy-Schwarz bound for a Volterra operator](../../../../../../iterated-cauchy-schwarz-bound-for-a-volterra-operator.md)**:

$$
\boxed{\|\tau^nf(t)\|_2
\leq\frac{C^nt^n}{\sqrt{1\cdot3\cdots(2n-1)}}M_t.}
$$

There is also a [factorial bound for a Volterra iterate](../../../../../../factorial-bound-for-a-volterra-iterate.md), obtained by iterating the unsquared integral estimate in (c):

$$
\boxed{\|\tau^nf(t)\|_2\leq\frac{C^nt^n}{n!}M_t.}
$$

Its factor $t^n/n!$ is the volume of the time-ordered simplex $0<s_n<\cdots<s_1<t$. It is stronger than the printed estimate because $\prod_{j=1}^n j^2\geq\prod_{j=1}^n(2j-1)$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
