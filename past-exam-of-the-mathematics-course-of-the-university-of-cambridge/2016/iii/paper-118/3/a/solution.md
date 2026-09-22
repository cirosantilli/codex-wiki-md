<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [connection on a vector bundle](../../../../../../connection-vector-bundle.md) is a real-linear map (complex-linear for a complex bundle)

$$
D:\Gamma(E)\longrightarrow\mathcal A^1(E),\qquad
D(fs)=df\otimes s+fDs.
$$

It extends to the [covariant exterior derivative](../../../../../../exterior-covariant-derivative.md) by $D(\eta\otimes s)=d\eta\otimes s+(-1)^k\eta\wedge Ds$ when $\eta$ has degree $k$. Its square is linear over smooth functions: in $D^2(fs)$ the two $df\wedge Ds$ terms have opposite signs and $d^2f=0$. The [curvature form of a connection](../../../../../../curvature-form.md) is therefore the endomorphism-valued two-form

$$
\boxed{\Theta=D^2\in\mathcal A^2(\operatorname{End}E).}
$$

In a local frame with $D=d+\theta$, it is $\Theta=d\theta+\theta\wedge\theta$.

Define the [tensor product connection](../../../../../../tensor-product-connection.md) on decomposable sections by

$$
\boxed{D(s\otimes t)=D_1s\otimes t+s\otimes D_2t.}
$$

The [Leibniz rule](../../../../../../leibniz-rule.md) for $D_1,D_2$ makes this well-defined over smooth functions and makes it a [connection on a vector bundle](../../../../../../connection-vector-bundle.md). Applying its [covariant exterior derivative](../../../../../../exterior-covariant-derivative.md) again gives

$$
D^2(s\otimes t)=D_1^2s\otimes t-D_1s\wedge D_2t
+D_1s\wedge D_2t+s\otimes D_2^2t.
$$

The mixed terms cancel by the graded sign. Thus **curvature adds on the two tensor factors**:

$$
\boxed{\Theta=\Theta_1\otimes I+I\otimes\Theta_2.}
$$

Equivalently, the mixed terms in $(\theta_1\otimes I+I\otimes\theta_2)\wedge(\theta_1\otimes I+I\otimes\theta_2)$ cancel because operators on the different factors commute. This also proves the [curvature of a tensor product connection](../../../../../../curvature-of-a-tensor-product-connection.md) formula in local frames.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 118](../../../paper-118-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
