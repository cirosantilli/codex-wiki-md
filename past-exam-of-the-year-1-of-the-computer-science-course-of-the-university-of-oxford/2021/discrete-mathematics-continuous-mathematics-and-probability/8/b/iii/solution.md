<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose **$g(t)=e^t$**. If $W$ has an [exponential distribution](../../../../../../exponential-distribution.md) with rate $r$, then for $c<r$,

$$
\mathbb E[e^{cW}]=\int_0^\infty r e^{-(r-c)t}\,dt=\frac r{r-c},
$$

while the [integral](../../../../../../integral-split.md) diverges to $+\infty$ when $c\geq r$. Since $Z$ has rate $3$,

$$
\mathbb E[g(Z)]=\frac32,\qquad
\mathbb E[g(Z)^2]=3,\qquad
\boxed{\operatorname{Var}(g(Z))=\frac34.}
$$

For the other two rates, $\mathbb E[g(V)]=2/(2-1)=2$, whereas $\mathbb E[g(U)]=\int_0^\infty1\,dt=+\infty$. These computations establish exactly the required finite [variance](../../../../../../variance-split.md), finite [expected value](../../../../../../expected-value-split.md), and infinite [expected value](../../../../../../expected-value-split.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
