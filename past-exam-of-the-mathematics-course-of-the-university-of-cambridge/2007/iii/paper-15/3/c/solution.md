<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [covariant exterior derivative](../../../../../../exterior-covariant-derivative.md) on the [endomorphism bundle](../../../../../../endomorphism-bundle.md) and remember that $F$ has degree two. The [Bianchi identity](../../../../../../bianchi-identity.md) is $d_AF=dF+A\wedge F-F\wedge A=0$. The local formula from part (b) gives

$$
\begin{aligned}
dF&=d(dA+A\wedge A)=dA\wedge A-A\wedge dA,\\
A\wedge F-F\wedge A
&=A\wedge dA+A\wedge A\wedge A-dA\wedge A-A\wedge A\wedge A\\
&=A\wedge dA-dA\wedge A.
\end{aligned}
$$

The two lines cancel, establishing

$$
\boxed{d_AF=0.}
$$

Because this is an [endomorphism](../../../../../../endomorphism.md)-valued equation and the operators transform covariantly under a change of [local frame](../../../../../../frame-of-a-vector-bundle.md), this local calculation proves the global identity.

For a [line bundle](../../../../../../line-bundle.md) over $k=\mathbb R$ or $\mathbb C$, every fibre [endomorphism](../../../../../../endomorphism.md) is multiplication by a scalar. Thus $\operatorname{End}E$ is canonically the trivial scalar bundle, even when $E$ itself is nontrivial. In a [local frame](../../../../../../frame-of-a-vector-bundle.md) $A$ is a scalar one-form, so $A\wedge A=0$ and $F=dA$ locally. Also $A\wedge F=F\wedge A$, since their degrees are one and two. The [Bianchi identity](../../../../../../bianchi-identity.md) therefore reduces to the ordinary closedness condition

$$
\boxed{dF=0.}
$$

This does not assert that the local scalar one-forms $A$ combine into a global one-form.

For two [connections on a vector bundle](../../../../../../connection-vector-bundle.md) $\nabla,\nabla'$, the difference is $C^\infty(M)$-linear in the section: the two $df\otimes s$ terms cancel. It is consequently a global [endomorphism](../../../../../../endomorphism.md)-valued one-form $a$. In rank one, $a$ is a global ordinary scalar one-form. Locally $A'=A+a$, and the scalar cross terms and $a\wedge a$ vanish, giving

$$
F_{A'}-F_A=d(A+a)-dA=da.
$$

This is a global equality, so the two [closed differential forms](../../../../../../closed-differential-form.md) differ by an [exact differential form](../../../../../../exact-differential-form.md). It proves the [connection-independent curvature class of a line bundle](../../../../../../connection-independent-curvature-class-of-a-line-bundle.md):

$$
\boxed{[F_{A'}]=[F_A]\in H^2_{\mathrm{dR}}(M;k).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
