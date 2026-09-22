<h1 id="26i/solution">Solution</h1>

↑ **Parent:** [26I](../26i.md)

A [smooth manifold](../../../../../smooth-manifold.md) of dimension $k$ is a Hausdorff, second-countable space with an atlas of smoothly compatible charts to open subsets of $\mathbb R^k$. A value $y\in Y$ is a [regular value](../../../../../regular-value.md) of a smooth map $f:X\to Y$ when every $x\in f^{-1}(y)$ has surjective derivative $df_x$.

The [inverse function theorem](../../../../../inverse-function-theorem.md) says that a smooth map between equal-dimensional manifolds whose derivative is invertible at a point is a diffeomorphism between neighbourhoods of that point and its image. If $y$ is a regular value of a map from an $m$-manifold to an $n$-manifold, choose coordinates corresponding to an invertible $n$ by $n$ minor of $df$. Applying the inverse theorem to $f$ together with the remaining $m-n$ coordinates makes $f$ the coordinate projection onto the first $n$ coordinates. Its level set is therefore locally $\mathbb R^{m-n}$. This proves the [preimage theorem](../../../../../preimage-theorem.md).

The critical-point set is closed because failure of full rank is the simultaneous vanishing of all maximal minors of $df$. If $X$ is compact, this set is compact, so its image under $f$ is compact and hence closed in the manifold $Y$. Its complement, the set of regular values, is open.

For the printed equations put

$$
F_1=x+y-z^2-w^2,\qquad
F_2=x^2+y^2-\frac{z^4}{2}.
$$

A rank calculation shows that $(a,0)$ is a regular value when $a>0$: if  
$\nabla F_2=\lambda\nabla F_1$, then

$$
x=y=\lambda/2,\qquad z(z^2-\lambda)=0,\qquad
\lambda w=0,\qquad \lambda^2=z^4.
$$

At a point of the level set these relations force $a\leq0$. Hence for $a>0$, the preimage theorem makes $X_a$ a two-dimensional manifold.

As printed, however, the assertion for every $a\ne0$ is false. If $a<0$, the points

$$
(0,0,0,\pm\sqrt{-a})
$$

belong to $X_a$. Near either point the first equation solves smoothly for $w$, while the second equation is

$$
x^2+y^2=z^4/2.
$$

Its positive-$z$ and negative-$z$ sheets meet only at the origin, so deleting the meeting point disconnects every sufficiently small neighbourhood. A punctured neighbourhood in a two-manifold is connected. Thus $X_a$ is not a manifold there.

For $a=0$, Cauchy--Schwarz gives

$$
x+y\leq\sqrt{2(x^2+y^2)}=z^2.
$$

The first equation requires $w^2=x+y-z^2\geq0$, so equality must hold. Therefore

$$
X_0=\{(z^2/2,z^2/2,z,0):z\in\mathbb R\}.
$$

This is the image of a smooth embedding with nonzero derivative, and hence  
$\boxed{X_0\text{ is a one-dimensional manifold}}$.

## ↑ Ancestors (10)

1. [26I](../26i.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
