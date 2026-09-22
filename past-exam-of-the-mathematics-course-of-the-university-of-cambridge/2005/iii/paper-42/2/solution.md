<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [transformation model](../../../../../transformation-model.md) consists of a [group](../../../../../group-split.md) $G$ acting measurably and invertibly on the sample space, an induced [group action](../../../../../group-action.md) on the parameter space, and a family $\{P_\theta\}$ satisfying $Y\sim P_\theta\Rightarrow gY\sim P_{g\theta}$. In a generated, transitive model, every $P_\theta$ is the image of a reference distribution under some transformation. In the density formulation, the transformed density includes the appropriate sample-space [Jacobian determinant](../../../../../jacobian-determinant.md); the model is a statement about whole [probability laws](../../../../../probability-distribution.md), not merely about changing parameter names.

A [maximal invariant](../../../../../maximal-invariant.md) $A$ has two properties: $A(gy)=A(y)$ for every $g$, and $A(y)=A(z)$ implies $z=gy$ for some $g$. It is therefore a coordinate for the [group orbits](../../../../../orbit-of-a-group-action.md), retaining exactly the information unaffected by the transformations. An [equivariant estimator](../../../../../equivariant-estimator.md) obeys $T(gy)=gT(y)$, where the right action is the induced parameter action.

For the normalization construction, suppose the estimator determines a [group](../../../../../group-split.md) element $t(y)\in G$ with $t(gy)=gt(y)$. Define $A(y)=t(y)^{-1}y$. Then

$$
A(gy)=(gt(y))^{-1}gy=t(y)^{-1}y=A(y).
$$

If $A(y)=A(z)$, rearranging gives $z=t(z)t(y)^{-1}y$. This is an actual transformation in $G$, so **the normalized sample is a [maximal invariant](../../../../../maximal-invariant.md)**. This [group](../../../../../group-split.md)-valued assumption matters: an estimator of a parameter with a nontrivial stabilizer does not necessarily determine a unique normalization. For a transitive parameter space $G/H$, choose a transformation carrying the estimated parameter to the reference value and take the resulting normalized sample modulo the remaining $H$-action. Different choices then have the same residual orbit. Under a free action $H$ is trivial and the simpler formula applies.

For a [location-scale model](../../../../../location-scale-family.md), $g_{a,b}(y_1,\ldots,y_n)=(a+by_1,\ldots,a+by_n)$, $b>0$, with composition $(a,b)(c,d)=(a+bc,bd)$. Its parameter action is $(\mu,\sigma)\mapsto(a+b\mu,b\sigma)$. Choose location and scale estimates satisfying

$$
\widehat m(a+by)=a+b\widehat m(y),\qquad \widehat s(a+by)=b\widehat s(y)>0.
$$

For instance, on nonconstant samples take the [sample mean](../../../../../sample-mean.md) and the positive square root of $n^{-1}\sum_i(y_i-\bar y)^2$. The standardized vector

$$
\boxed{A(y)=\left(\frac{y_i-\widehat m(y)}{\widehat s(y)}\right)_{i=1}^n}
$$

is invariant. Conversely, equality of these vectors gives $z_i=c+dy_i$ for all $i$, with $d=\widehat s(z)/\widehat s(y)>0$ and $c=\widehat m(z)-d\widehat m(y)$. Hence it is maximal, not just invariant. Degenerate constant samples have zero fitted scale and form a separate orbit; define a separate invariant value there. The construction is on labelled sample vectors: one must not discard their order unless permutations are also included in the transformation [group](../../../../../group-split.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
