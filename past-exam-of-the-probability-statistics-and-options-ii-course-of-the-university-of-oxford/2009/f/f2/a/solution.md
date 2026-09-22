<h1 id="f/f2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The $i$th [partial derivative](../../../../../partial-derivative.md) is the limit $\partial_if(x_0)=\lim_{t\to0}[f(x_0+te_i)-f(x_0)]/t$. For a nonzero vector $v$, use the directional convention $\partial_vf(x_0)=\lim_{t\to0}[f(x_0+tv)-f(x_0)]/t$, without normalizing $v$. [Differentiability](../../../../../differentiability.md) means $f(x_0+h)=f(x_0)+Lh+o(\|h\|)$ for a [linear map](../../../../../linear-map.md) $L=df(x_0)$.

For the given example take $v=(v_1,v_2)$. If $v_1\ne0$, then $f(tv)=t^2v_2^3/v_1$, so its directional difference quotient tends to zero. If $v_1=0$, the function vanishes along that line. Thus $\boxed{\partial_vf(0)=0\text{ for every }v\ne0}$. However along $(x,y)=(t^3,t)$ with $t\ne0$, one has $f(x,y)=1$, while $f(0,0)=0$. Hence **the function is neither [continuous](../../../../../continuous-function.md) nor [differentiable](../../../../../differentiable-function.md) at zero**. Existence of all [directional derivatives](../../../../../directional-derivative.md), even with a linear dependence on the direction, does not by itself imply total [differentiability](../../../../../differentiability.md).

## ↑ Ancestors (13)

1. [A](../a.md)
2. [F2](../../f2.md)
3. [F](../../../f.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
