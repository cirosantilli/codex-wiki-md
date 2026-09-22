<h1 id="19g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [linear map](../../../../../../linear-map.md) $T:X\to Y$ between normed spaces is a [bounded linear operator](../../../../../../continuous-linear-operator.md) if $\|Tx\|\leq C\|x\|$ for one finite $C$ and every $x$. This implies $\|Tx-Ty\|\leq C\|x-y\|$, hence continuity. Conversely, continuity at zero supplies $\delta>0$ such that $\|x\|<\delta$ implies $\|Tx\|<1$. Apply this to $\delta x/(2\|x\|)$ to obtain $\|Tx\|\leq2\|x\|/\delta$ for nonzero $x$. Thus **boundedness and continuity are equivalent for [linear maps](../../../../../../linear-map.md)**.

The [operator norm](../../../../../../operator-norm.md) is $\|T\|=\sup_{\|x\|\leq1}\|Tx\|$, equivalently $\sup_{x\ne0}\|Tx\|/\|x\|$. The bounded operators form a [vector space](../../../../../../vector-space-split.md), since $\|(S+T)x\|\leq(\|S\|+\|T\|)\|x\|$ and scalar multiples remain bounded. Taking suprema proves the [triangle inequality](../../../../../../triangle-inequality.md) and absolute homogeneity for the [operator norm](../../../../../../operator-norm.md); $\|T\|=0$ forces $Tx=0$ for every $x$. Thus $B(X,Y)$ is a normed space, whether or not $X,Y$ are complete.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19G](../../19g.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
