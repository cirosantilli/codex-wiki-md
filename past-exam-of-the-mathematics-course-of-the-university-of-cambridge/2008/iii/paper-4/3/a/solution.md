<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $q=p^n$ and choose a generator $h$ of $H$. In characteristic $p$, $(h-1)^q=h^q-1=0$, so

$$
kH\cong k[t]/(t^q),\qquad t=h-1.
$$

A [module](../../../../../../module-mathematics.md) is a vector space with a [nilpotent operator](../../../../../../nilpotent-linear-map.md) $t$ whose nilpotence index is at most $q$. The nilpotent [Jordan normal form](../../../../../../jordan-normal-form.md), valid over every [field](../../../../../../field.md), splits it into Jordan blocks. One block of size $i$ is

$$
\boxed{V_i=k[t]/(t^i),\qquad1\le i\le q.}
$$

It is indecomposable: its [endomorphism ring](../../../../../../endomorphism-ring.md) is $k[t]/(t^i)$, a [local ring](../../../../../../local-ring.md) with no nontrivial [idempotents](../../../../../../idempotent.md). Distinct $i$ have distinct dimensions. Conversely a [direct sum](../../../../../../direct-sum.md) of at least two Jordan blocks is decomposable. Thus there are exactly $q$ indecomposable isomorphism classes.

A homomorphism $V_i\to V_j$ is determined by the image of $1$, which can be any element of $V_j$ annihilated by $t^i$. If $i\ge j$ this is all of $V_j$, of dimension $j$; if $i<j$ it is the span of $t^{j-i},\ldots,t^{j-1}$, of dimension $i$. Hence

$$
\boxed{\dim_k\operatorname{Hom}_{kH}(V_i,V_j)=\min(i,j).}
$$

This realizes the [indecomposable modules for a cyclic p-group](../../../../../../indecomposable-modules-for-a-cyclic-p-group.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
