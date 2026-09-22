<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

A [connection on a vector bundle](../../../../../connection-vector-bundle.md) $E\to M$ is a linear map $D:\Gamma(E)\to\Omega^1(M;E)$ with $D(fs)=df\otimes s+fDs$. Write a [local frame](../../../../../frame-of-a-vector-bundle.md) as a row $e=(e_1,\ldots,e_r)$, and a section as $s=eu$ with a coefficient column $u$. If the [connection one-form](../../../../../connection-one-form.md) is the [matrix](../../../../../matrix.md) $A=\sum_iA_i\,dx^i$, then

$$
\boxed{D(eu)=e(du+Au),\qquad
(D_is)^a=\partial_i u^a+\sum_b(A_i)^a{}_bu^b.}
$$

This fixes the [matrix](../../../../../matrix.md) convention for all subsequent signs.

For an $E$-valued [differential form](../../../../../differential-form-split.md) of degree $k$, represented locally by a column $\alpha$ of ordinary forms, its [covariant exterior derivative](../../../../../exterior-covariant-derivative.md) is

$$
\boxed{d_A\alpha=d\alpha+A\wedge\alpha.}
$$

The defining [graded Leibniz rule](../../../../../graded-leibniz-rule.md) with a scalar form $\omega$ of degree $j$ is

$$
d_A(\omega\wedge\alpha)=d\omega\wedge\alpha+(-1)^j\omega\wedge d_A\alpha.
$$

It follows by moving the one-form $A$ past $\omega$, which introduces $(-1)^j$. It uniquely extends the connection on sections.

The induced [endomorphism bundle connection](../../../../../endomorphism-bundle-connection.md) is characterized on an endomorphism section $T$ by $(D^{\rm End}T)s=D(Ts)-T(Ds)$. For a matrix-valued form $\beta$ of degree $k$, the extension is

$$
\boxed{d_A^{\rm End}\beta=d\beta+A\wedge\beta-(-1)^k\beta\wedge A.}
$$

Indeed it is exactly the formula that makes

$$
d_A(\beta\wedge\alpha)=(d_A^{\rm End}\beta)\wedge\alpha+(-1)^k\beta\wedge d_A\alpha.
$$

The [endomorphism-valued exterior product](../../../../../endomorphism-valued-exterior-product.md) uses [matrix](../../../../../matrix.md) composition as well as the ordinary [exterior product](../../../../../exterior-product.md), so factors cannot in general be interchanged.

Define the [curvature form of a connection](../../../../../curvature-form.md) by $D^2$ acting on sections, or equivalently by

$$
F(X,Y)s=D_XD_Ys-D_YD_Xs-D_{[X,Y]}s.
$$

It is tensorial in both vector arguments and in $s$: the derivatives of multiplying functions cancel by the connection rule. For example $D^2(fs)=D(df\,s+fDs)=fD^2s$, since the two $df\wedge Ds$ terms cancel and $d^2f=0$. Thus curvature is a two-form with values in the [endomorphism bundle](../../../../../endomorphism-bundle.md). Locally, applying the graded rule gives

$$
(d+A\wedge)^2\alpha=(dA+A\wedge A)\wedge\alpha,
$$

so

$$
\boxed{F(A)=dA+A\wedge A,\qquad
F_{ij}=\partial_iA_j-\partial_jA_i+[A_i,A_j].}
$$

For a [change of frame of a vector-bundle connection](../../../../../change-of-frame-of-a-vector-bundle-connection.md) $e'=eg$, the coefficients satisfy $u'=g^{-1}u$, and differentiation gives

$$
A'=g^{-1}Ag+g^{-1}dg,\qquad d_{A'}=g^{-1}d_Ag.
$$

Squaring yields $F'=g^{-1}Fg$, precisely the transformation rule of an endomorphism-valued two-form. This independently proves that the local expressions define one global [curvature form of a connection](../../../../../curvature-form.md).

For the [Bianchi identity](../../../../../bianchi-identity.md), use the endomorphism formula with degree two:

$$
\begin{aligned}
d_A^{\rm End}F
&=dF+A\wedge F-F\wedge A\\
&=(dA\wedge A-A\wedge dA)
 +(A\wedge dA+A\wedge A\wedge A)\\
&\hspace{1em}-(dA\wedge A+A\wedge A\wedge A)=0.
\end{aligned}
$$

Every term cancels with its indicated sign. Therefore

$$
\boxed{d_A F(A)=0,}
$$

where $d_A$ here means the induced derivative on the [endomorphism bundle](../../../../../endomorphism-bundle.md).

For a [line bundle](../../../../../line-bundle.md), the [endomorphism bundle](../../../../../endomorphism-bundle.md) is canonically the trivial scalar bundle: every fibre endomorphism is a scalar times the identity. Scalar multiplication commutes, so $A\wedge A=0$ and the endomorphism covariant derivative on scalar-valued forms reduces to $d$. The [Bianchi identity](../../../../../bianchi-identity.md) consequently says $dF=0$.

If $D'$ is another connection, their difference is $C^\infty$-linear in sections because the Leibniz terms cancel. Hence $D'-D=\eta$ is a global endomorphism-valued one-form; for a [line bundle](../../../../../line-bundle.md) it is an ordinary global scalar one-form. Locally $A'=A+\eta$, so

$$
F(D')-F(D)=d\eta.
$$

Thus the two closed curvatures differ by an exact form, proving the [connection-independent curvature class of a line bundle](../../../../../connection-independent-curvature-class-of-a-line-bundle.md):

$$
\boxed{[F(D')]=[F(D)]\in H^2_{\rm dR}(M;\mathbb K).}
$$

No global trivialization of the [line bundle](../../../../../line-bundle.md) itself was assumed; it is its [endomorphism bundle](../../../../../endomorphism-bundle.md) that has the canonical scalar identification.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
