<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If a [bilinear map](../../../../../bilinear-map.md) is continuous, [continuity](../../../../../continuous-function.md) at $(0,0)$ gives $\delta>0$ such that $\|F(x,y)\|\leq1$ whenever $\|x\|,\|y\|<\delta$. For nonzero $x,y$, apply this to $\delta x/(2\|x\|)$ and $\delta y/(2\|y\|)$. Bilinearity gives

$$
\boxed{\|F(x,y)\|\leq\frac4{\delta^2}\|x\|\|y\|.}
$$

If either input is zero, the inequality follows from bilinearity directly.

Conversely, suppose the product bound holds with $C\geq0$. At a fixed point $(x,y)$,

$$
F(x+h,y+k)-F(x,y)=F(h,y)+F(x,k)+F(h,k).
$$

Its [norm](../../../../../norm.md) is at most $C(\|h\|\|y\|+\|x\|\|k\|+\|h\|\|k\|)$, which tends to zero as $(h,k)\to(0,0)$. Thus **the product bound is equivalent to joint [continuity](../../../../../continuous-function.md)**. This is [boundedness criterion for a bilinear map](../../../../../boundedness-criterion-for-a-bilinear-map.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
