<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the uniform proposal on $[1,7]$, with density $g=1/6$. The [triangular distribution](../../../../../../../triangular-distribution.md) peaks at $x=3$ with height $1/3$, so the optimal constant for this proposal is $M=2$. At each attempt take two fresh pseudo-random uniforms $U,V$, and propose $Y=1+6U$. The [rejection method](../../../../../../../rejection-sampling.md) accepts according to

$$
\boxed{V\le\begin{cases}(Y-1)/2,&1\le Y\le3,\\(7-Y)/4,&3<Y\le7.\end{cases}}
$$

Indeed these bounds are $f(Y)/(2g(Y))=3f(Y)$. Part (a) proves that the accepted value has the required density. Acceptance probability is $1/2$, so the method needs two proposal attempts on average, and hence four uniforms on average if each attempt uses two. The validity of the ideal algorithm presumes independent uniform draws; merely belonging to $[0,1]$ does not by itself make a pseudo-random sequence uniform or independent.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
