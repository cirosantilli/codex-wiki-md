<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In coordinates, expanding $d\alpha$ and the [Lie bracket of vector fields](../../../../../lie-bracket-of-vector-fields.md) shows

$$
d\alpha(X,Y)=X(\alpha(Y))-Y(\alpha(X))-\alpha([X,Y]).
$$

The terms differentiating components of $X,Y$ cancel against the bracket, leaving $(\partial_i\alpha_j-\partial_j\alpha_i)X^iY^j$. This is the [exterior derivative of a one-form evaluated on vector fields](../../../../../exterior-derivative-of-a-one-form-evaluated-on-vector-fields.md).

A [connection on a vector bundle](../../../../../connection-vector-bundle.md) is a linear map $\nabla:\Gamma(E)\to\Omega^1(E)$ satisfying $\nabla(fs)=df\otimes s+f\nabla s$; evaluation on $X$ defines $\nabla_Xs$. Its [curvature form of a connection](../../../../../curvature-form.md) is $d_A^2$, locally $F_A=dA+A\wedge A$. Direct expansion, using the displayed exterior-derivative identity, gives

$$
\boxed{F_A(X,Y)s=\nabla_X\nabla_Ys-\nabla_Y\nabla_Xs-\nabla_{[X,Y]}s.}
$$

The derivative terms on a scalar multiplying $s$ cancel, and the expression is also linear over smooth functions in $X,Y$. Thus it is an alternating tensor with values in $\operatorname{End}(E)$, namely an element of $\Omega^2(\operatorname{End}(E))$.

The [dual connection](../../../../../dual-connection.md) and [tensor product connection](../../../../../tensor-product-connection.md) induce the [endomorphism bundle connection](../../../../../endomorphism-bundle-connection.md) on $E^*\otimes E$:

$$
(\widetilde\nabla_X\phi)(s)=\nabla_X(\phi s)-\phi(\nabla_Xs).
$$

Expanding twice cancels the cross terms and gives

$$
([\widetilde\nabla_X,\widetilde\nabla_Y]\phi)(s)
=[\nabla_X,\nabla_Y](\phi s)-\phi([\nabla_X,\nabla_Y]s).
$$

Here $\phi,s$ are local smooth sections; derivatives are not defined for isolated fiber elements without extensions. Subtract the corresponding $\widetilde\nabla_{[X,Y]}$ identity to get the [curvature of an endomorphism bundle connection](../../../../../curvature-of-an-endomorphism-bundle-connection.md):

$$
\boxed{F_{\operatorname{End}(A)}(X,Y)\phi=[F_A(X,Y),\phi].}
$$

This vanishes for all $\phi$ exactly when each $F_A(X,Y)$ is central in the full matrix algebra, hence scalar. For rank $r>0$, $\omega=r^{-1}\operatorname{tr}F_A$ is a smooth two-form and

$$
\boxed{F_{\operatorname{End}(A)}=0\quad\Longleftrightarrow\quad F_A=\omega\,\operatorname{id}_E.}
$$

Conversely scalar curvature commutes with every endomorphism. This is the [scalar-curvature criterion for a flat endomorphism connection](../../../../../scalar-curvature-criterion-for-a-flat-endomorphism-connection.md); it permits a nonflat connection on $E$ itself.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 115](../../paper-115-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
