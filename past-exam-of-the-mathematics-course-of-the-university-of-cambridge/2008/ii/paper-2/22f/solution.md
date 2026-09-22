<h1 id="22f/solution">Solution</h1>

↑ **Parent:** [22F](../22f.md)

The [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) states that a pointwise bounded family $\mathcal T$ of bounded [linear maps](../../../../../linear-map.md) from a [Banach space](../../../../../banach-space-split.md) $X$ to a normed space $Y$ is uniformly bounded in [operator norm](../../../../../operator-norm.md). Define closed sets $E_n=\{x:\sup_{T\in\mathcal T}\|Tx\|\le n\}$. Pointwise boundedness makes their union $X$. The [Baire category theorem](../../../../../baire-category-theorem.md) gives a ball $B(x_0,r)\subset E_n$ for some $n$. For $\|v\|<r$, both $x_0+v$ and $x_0$ lie in $E_n$, so $\|Tv\|\le2n$ for every $T$. Scaling yields $\sup_T\|T\|\le2n/r$, proving the principle.

For the separately continuous [bilinear map](../../../../../bilinear-map.md), consider $T_x(y)=F(x,y)$ with $\|x\|\le1$. Each $T_x$ is bounded and linear. For fixed $y$, continuity of the other [linear map](../../../../../linear-map.md) gives $\sup_{\|x\|\le1}\|F(x,y)\|<\infty$. Apply the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) to this family to get

$$
\boxed{\|F(x,y)\|\le M\|x\|\|y\|.}
$$

Bilinearity then gives $F(x,y)-F(x_0,y_0)=F(x-x_0,y)+F(x_0,y-y_0)$; the bound proves joint continuity.

For the trilinear map, fix $w$. The just-proved bilinear result bounds $G(\cdot,\cdot,w)$. Thus the bounded [linear maps](../../../../../linear-map.md) $T_{x,y}:w\mapsto G(x,y,w)$, for $\|x\|,\|y\|\le1$, are pointwise bounded. Apply the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) once more to obtain $\|G(x,y,w)\|\le C\|x\|\|y\|\|w\|$. Expansion of the difference in three slots proves joint continuity. **Separate continuity suffices for these multilinear maps.**

Without linearity it does not suffice. On $\mathbb R^2$ set $H(x,y)=xy/(x^2+y^2)$ away from the origin and $H(0,0)=0$. Each coordinate section is continuous, but $H(t,t)=1/2$ for $t\ne0$, so $H$ is not continuous at the origin.

## ↑ Ancestors (10)

1. [22F](../22f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
