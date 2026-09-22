# Minkowski inequality for finite vectors

↑ **Parent:** [Minkowski inequality](minkowski-inequality.md)

For [vectors](vector.md) $u,v\in\mathbb R^n$ or $\mathbb C^n$, [counting measure](counting-measure.md) turns the [Minkowski inequality](minkowski-inequality.md) into

$$
\left(\sum_{i=1}^n|u_i+v_i|^p\right)^{1/p}
\leq\left(\sum_{i=1}^n|u_i|^p\right)^{1/p}
+\left(\sum_{i=1}^n|v_i|^p\right)^{1/p},\qquad 1\leq p<\infty.
$$

For $p=\infty$, replace each displayed [norm](norm.md) by the maximum of its coordinate [absolute values](absolute-value.md). Take $u=(1,0)$ and $v=(0,1)$. Both [vectors](vector.md) have [Lp norm](lp-norm.md) one for every $p\geq1$, but their sum has [L1 norm](l1-norm.md) $2$, [Euclidean norm](euclidean-norm.md) $\sqrt2$, and [L-infinity norm](l-infinity-norm.md) $1$. Thus the same [vector addition](vector-addition.md) gives equality $2=1+1$ at $p=1$, strict inequality $\sqrt2<1+1$ at $p=2$, and strict inequality $1<1+1$ at $p=\infty$.

By contrast, $u=(1,1)$ and $v=2u=(2,2)$ give equality for every $p\geq1$: [absolute homogeneity of a norm](absolute-homogeneity-of-a-norm.md) yields $\lVert u+v\rVert_p=3\lVert u\rVert_p=\lVert u\rVert_p+\lVert v\rVert_p$. At $p=2$, the three sizes are $\sqrt2$, $2\sqrt2$, and $3\sqrt2$. Opposite [vectors](vector.md) behave very differently: $u+(-u)=0$, so the inequality is strict whenever $u$ is nonzero. Cancellation is allowed; the bound describes the largest possible total size.

<a id="image-strict-minkowski-inequality-equality-for-positive-multiples-and-quasi-norm-failure"></a>
![](minkowski-vector-equality-and-quasinorm-failure.png)

**[Figure 19](#image-strict-minkowski-inequality-equality-for-positive-multiples-and-quasi-norm-failure). Strict Minkowski inequality, equality for positive multiples, and quasi-norm failure**. Arrows show $u$, the translated step $v$, and their sum. Left: perpendicular unit [vectors](vector.md) give $\sqrt2<2$ for the [Euclidean norm](euclidean-norm.md). Middle: $u=(1,1)$ and $v=(2,2)$ give $3\sqrt2=\sqrt2+2\sqrt2$. Right: $u=(1,0)$ and $v=(0,1)$ give $4>2$ for the [Lq quasi-norm](lq-quasi-norm.md) at $q=1/2$. Pale curves show the corresponding unit level sets.

## ↑ Ancestors (7)

1. [Minkowski inequality](minkowski-inequality.md)
2. [Lp norm](lp-norm.md)
3. [Real analysis](real-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
