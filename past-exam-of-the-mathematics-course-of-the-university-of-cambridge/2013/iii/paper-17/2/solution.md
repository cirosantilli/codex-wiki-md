<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [connection on a vector bundle](../../../../../connection-vector-bundle.md) is a complex-linear map from smooth sections to vector-bundle-valued one-forms satisfying

$$
D(fs)=df\otimes s+fDs.
$$

Choose a locally finite trivializing cover, its componentwise flat [connections on a vector bundle](../../../../../connection-vector-bundle.md) $D_i$, and a subordinate smooth [partition of unity](../../../../../partition-of-unity.md) $\rho_i$. The formula $D=\sum_i\rho_iD_i$ is globally meaningful: each weighted term extends by zero outside its chart. Its [Leibniz rule](../../../../../leibniz-rule.md) follows from $\sum_i\rho_i=1$, proving **every smooth complex vector bundle admits a connection**.

Extend the [connection on a vector bundle](../../../../../connection-vector-bundle.md) to bundle-valued [differential forms](../../../../../differential-form-split.md) by

$$
D(\beta\otimes s)=d\beta\otimes s+(-1)^{\deg\beta}\beta\wedge Ds.
$$

The [curvature form of a connection](../../../../../curvature-form.md) is $\Theta_D=D^2$. Applying this twice to $fs$ shows that the $df$ terms cancel, so $D^2$ is tensorial and defines an $\operatorname{End}(E)$-valued two-form. With column coordinates for sections and [connection one-form](../../../../../connection-one-form.md) $A$, the local expression is $D=d+A\wedge$. Direct expansion on an arbitrary bundle-valued form gives

$$
(d+A\wedge)^2=dA\wedge+A\wedge A\wedge.
$$

The terms containing a derivative of the argument cancel by the graded [Leibniz rule](../../../../../leibniz-rule.md). Thus [Cartan curvature matrix equation](../../../../../cartan-curvature-matrix-equation.md) is

$$
\boxed{\Theta=dA+A\wedge A.}
$$

Here multiplication includes matrix multiplication and the [exterior product](../../../../../exterior-product.md) of form entries. For a frame change $e'=eg$, the [connection one-form](../../../../../connection-one-form.md) and [curvature form of a connection](../../../../../curvature-form.md) transform as

$$
A'=g^{-1}Ag+g^{-1}dg,\qquad
\Theta'=g^{-1}\Theta g.
$$

The [trace](../../../../../matrix-trace.md) is consequently frame independent. Also

$$
\operatorname{Tr}(A\wedge A)=\sum_{i,j}A_{ij}\wedge A_{ji}=0:
$$

the diagonal terms vanish and the off-diagonal terms cancel in pairs. Locally $\operatorname{Tr}\Theta=d\operatorname{Tr}A$, and hence $d\operatorname{Tr}\Theta=0$. The local primitives need not agree, but the two-form does. We obtain **a global closed two-form** $\operatorname{Tr}\Theta_D$.

The [determinant connection](../../../../../determinant-connection.md) on $\det E=\bigwedge^rE$ is defined intrinsically by

$$
D^{(r)}(s_1\wedge\cdots\wedge s_r)
=\sum_{j=1}^r s_1\wedge\cdots\wedge Ds_j\wedge\cdots\wedge s_r,
$$

where the differential-form coefficient of $Ds_j$ is placed first. In a local frame, only the diagonal components contribute to the derivative of $e_1\wedge\cdots\wedge e_r$, so its [connection one-form](../../../../../connection-one-form.md) is $\operatorname{Tr}A$. A line-bundle connection has curvature $d\operatorname{Tr}A$, because a scalar one-form wedges with itself to zero. Therefore

$$
\boxed{\Theta_{D^{(r)}}=\operatorname{Tr}\Theta_D.}
$$

To see independence of the [de Rham cohomology](../../../../../de-rham-cohomology.md) class, write $D_1-D_0=a$, a globally defined endomorphism-valued one-form. The [curvature difference formula](../../../../../curvature-difference-formula.md) and the same trace cancellations give the [trace curvature transgression](../../../../../trace-curvature-transgression.md)

$$
\operatorname{Tr}\Theta_{D_1}-\operatorname{Tr}\Theta_{D_0}
=d\operatorname{Tr}a.
$$

Their difference is globally an [exact differential form](../../../../../exact-differential-form.md), so their [de Rham cohomology](../../../../../de-rham-cohomology.md) classes coincide.

For the [Hermitian metric on a holomorphic vector bundle](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md), use the displayed ordering of the local matrices and put $B=(\partial h)h^{-1}$. The identity $\bar\partial h^{-1}=-h^{-1}(\bar\partial h)h^{-1}$ gives

$$
\bar\partial B
=(\bar\partial\partial h)h^{-1}
+(\partial h)h^{-1}\wedge(\bar\partial h)h^{-1}.
$$

The plus sign comes from applying the graded [Leibniz rule](../../../../../leibniz-rule.md) to the one-form $\partial h$. By the derivative formula for a [determinant](../../../../../determinant.md),

$$
\operatorname{Tr}B=\partial\log\det h.
$$

The [Hermitian positive-definite matrix](../../../../../hermitian-positive-definite-matrix.md) $h$ has positive real determinant, so this logarithm is an ordinary smooth real function. The [trace of Chern curvature](../../../../../trace-of-chern-curvature.md) in these conventions is therefore

$$
\boxed{\alpha=\bar\partial\partial\log\det h
=d(\partial\log\det h)=-\partial\bar\partial\log\det h.}
$$

It is locally an [exact differential form](../../../../../exact-differential-form.md) and in particular closed.

A [holomorphic local frame](../../../../../holomorphic-local-trivialization.md) change multiplies $\det h$ by $|\det g|^2$. A nowhere-zero [holomorphic function](../../../../../holomorphic-function.md) has a local [holomorphic logarithm](../../../../../holomorphic-logarithm.md), so $\bar\partial\partial\log|\det g|^2=0$. Thus the preceding expression for $\alpha$ is independent of the frame and glues globally. For two [Hermitian metrics on a holomorphic vector bundle](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md), the function

$$
f=\log\frac{\det h_1}{\det h_0}
$$

is globally defined because the frame-change factors cancel. Their two-forms differ by $d(\partial f)$. Hence **the class of $\alpha$ is independent of the metric**. The two-form is generally imaginary-valued; the metric independence statement is in complex [de Rham cohomology](../../../../../de-rham-cohomology.md), or equivalently for the real form $i\alpha$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
