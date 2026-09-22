<h1 id="22f/solution">Solution</h1>

↑ **Parent:** [22F](../22f.md)

If a [linear map](../../../../../linear-map.md) satisfies $\|Tx\|\le M\|x\|$, then $\|Tx-Tx'\|\le M\|x-x'\|$, so it is [continuous](../../../../../continuous-function.md). Conversely [continuity](../../../../../continuous-function.md) at zero gives $\delta>0$ such that $\|x\|<\delta$ implies $\|Tx\|<1$. Apply this to $\delta x/(2\|x\|)$ for $x\ne0$ to obtain $\|Tx\|\le2\|x\|/\delta$. Hence **a [linear map](../../../../../linear-map.md) is [continuous](../../../../../continuous-function.md) exactly when it is bounded**.

For the separately [continuous](../../../../../continuous-function.md) [bilinear map](../../../../../bilinear-map.md), put $T_x(y)=F(x,y)$ for $\|x\|\le1$. Every $T_x:Y\to Z$ is a bounded [linear map](../../../../../linear-map.md) by the first result. For each fixed $y$, [continuity](../../../../../continuous-function.md) in the other variable gives $\|F(x,y)\|\le C_y\|x\|$, so $\sup_{\|x\|\le1}\|T_xy\|<\infty$. The [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) therefore gives $\sup_{\|x\|\le1}\|T_x\|=M<\infty$, and bilinearity then yields

$$
\boxed{\|F(x,y)\|\le M\|x\|\|y\|}.
$$

To spell out the uniform-boundedness step, define the closed subsets $E_m=\{y:\sup_{\|x\|\le1}\|T_xy\|\le m\}$ of the [Banach space](../../../../../banach-space-split.md) $Y$. They cover $Y$. The [Baire category theorem](../../../../../baire-category-theorem.md) gives an $E_m$ containing a ball $B(y_0,r)$. For $\|h\|<r$, both $y_0+h$ and $y_0$ lie in $E_m$, so $\sup_x\|T_xh\|\le2m$. Scaling $h=(r/2)y$ for $\|y\|\le1$ bounds all the operator [norms](../../../../../norm.md) by $4m/r$. This proves the claimed uniform estimate without presuming joint [continuity](../../../../../continuous-function.md).

## ↑ Ancestors (10)

1. [22F](../22f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
