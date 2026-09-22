<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [holomorphic line bundle](../../../../../holomorphic-line-bundle.md) is a complex rank-one bundle locally trivialized over [holomorphic coordinate](../../../../../holomorphic-coordinate.md) opens, with nowhere-zero [holomorphic](../../../../../complex-differentiability-at-a-point.md) transition functions. A local [holomorphic section](../../../../../holomorphic-section.md) has a [holomorphic](../../../../../complex-differentiability-at-a-point.md) coefficient in a [holomorphic local frame](../../../../../holomorphic-local-trivialization.md). Let $h$ be a smooth positive [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) on its fibres. A [Chern connection](../../../../../chern-connection.md) is a connection compatible with $h$ whose $(0,1)$ part is the bundle's [Dolbeault operator](../../../../../dolbeault-operator.md).

Fix the Hermitian-product convention linear in the first variable and a nonvanishing [holomorphic local frame](../../../../../holomorphic-local-trivialization.md) $e$. Put $h_e=h(e,e)>0$ and write $\nabla e=Ae$. Compatibility with the [holomorphic](../../../../../complex-differentiability-at-a-point.md) structure forces $A^{0,1}=0$. Metric compatibility gives

$$
dh_e=(A+\bar A)h_e,
$$

so taking its $(1,0)$ part determines $A$ uniquely:

$$
\boxed{A=\partial\log h_e.}
$$

Define the connection by this formula. To check it exists globally, change frame to $e'=ge$ for a nonzero [holomorphic function](../../../../../holomorphic-function.md) $g$. Then $h_{e'}=|g|^2h_e$ and

$$
\partial\log h_{e'}=\partial\log h_e+g^{-1}dg,
$$

which is exactly the connection transformation law obtained from $\nabla(ge)=dg\,e+g\nabla e$. Hence the local connections glue. The formula and its conjugate give metric compatibility, and $A^{0,1}=0$ gives the required [holomorphic](../../../../../complex-differentiability-at-a-point.md) structure. Since either condition already forced this unique formula in every frame, existence and uniqueness are proved.

For a [line bundle](../../../../../line-bundle.md), the [curvature form of a connection](../../../../../curvature-form.md) is $F=\nabla^2=dA$, as the scalar one-form satisfies $A\wedge A=0$. The [local formula for the Chern connection on a line bundle](../../../../../local-formula-for-the-chern-connection-on-a-line-bundle.md) therefore gives

$$
\boxed{F_h=\bar\partial\partial\log h_e=-\partial\bar\partial\log h_e.}
$$

This formula uses a nowhere-zero local [holomorphic section](../../../../../holomorphic-section.md); arbitrary sections with zeros are not frames there. It has type $(1,1)$, is $d$-closed and satisfies $\bar F_h=-F_h$, so $iF_h$ is a real $(1,1)$-form. The transformation calculation makes its frame independence explicit.

For two metrics, their ratio $r=h_1(e,e)/h_2(e,e)$ is a global positive smooth function, since the common frame factors cancel. The [curvature difference of two Chern connections](../../../../../curvature-difference-of-two-chern-connections.md) is

$$
F_{h_1}-F_{h_2}=\bar\partial\partial\log r,
\qquad iF_{h_1}-iF_{h_2}=\bar\partial(i\partial\log r).
$$

Each curvature is $\bar\partial$-closed, and the difference has a global $(1,0)$ primitive for $\bar\partial$. Thus

$$
\boxed{[iF_{h_1}]=[iF_{h_2}]\ \text{in }H^{1,1}(X).}
$$

This is equality in [Dolbeault cohomology](../../../../../dolbeault-cohomology.md), rather than merely equality in [de Rham cohomology](../../../../../de-rham-cohomology.md); the displayed primitive proves precisely that distinction.

Finally let $s$ be a nowhere-zero smooth section of $\hat L$. In this global smooth trivialization write $\bar\partial_{\hat L}s=a\otimes s$ with a global $(0,1)$-form $a$. The [holomorphic](../../../../../complex-differentiability-at-a-point.md) structure has $\bar\partial_{\hat L}^2=0$. Its Leibniz rule gives

$$
0=\bar\partial_{\hat L}(a\otimes s)=(\bar\partial a-a\wedge a)\otimes s=(\bar\partial a)\otimes s,
$$

since a scalar one-form wedges with itself to zero. The hypothesis $H^{0,1}(X)=0$ makes $a=\bar\partial f$ for a global smooth complex function $f$. Then

$$
\bar\partial_{\hat L}(e^{-f}s)=e^{-f}(a-\bar\partial f)\otimes s=0.
$$

The exponential never vanishes. Therefore **$e^{-f}s$ is a nowhere-zero [holomorphic section](../../../../../holomorphic-section.md)**, proving [smoothly trivial holomorphic line bundles when H01 vanishes](../../../../../smoothly-trivial-holomorphic-line-bundles-when-h01-vanishes.md) constructively, without a [compactness](../../../../../compact-space.md) assumption.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
