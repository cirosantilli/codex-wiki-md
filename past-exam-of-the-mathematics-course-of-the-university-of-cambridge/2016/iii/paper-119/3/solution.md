<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [terminal object](../../../../../terminal-object.md) $1$ is an [exponentiable object](../../../../../exponentiable-object.md) because $-\times1\cong1_{\mathcal C}$ has the identity as a [right adjoint](../../../../../adjoint-functors.md). If $A$ and $B$ are [exponentiable objects](../../../../../exponentiable-object.md), compose the two [adjunctions](../../../../../adjoint-functors.md) to get

$$
\begin{aligned}
\mathcal C(X\times(A\times B),Y)
&\cong\mathcal C((X\times A)\times B,Y)\\
&\cong\mathcal C(X\times A,Y^B)
\cong\mathcal C(X,(Y^B)^A).
\end{aligned}
$$

Consequently **[exponentiable objects](../../../../../exponentiable-object.md) are closed under finite [products in a category](../../../../../product-category-theory.md)**, including the empty product, and

$$
\boxed{Y^{A\times B}\cong(Y^B)^A.}
$$

Under the additional hypotheses, a [coseparator](../../../../../coseparator.md) $S$ detects unequal parallel arrows by postcomposition: for $u\ne v:X\to B$ there is $t:B\to S$ with $tu\ne tv$. Local smallness makes $I=\mathcal C(B,S)$ a set, and completeness forms the [product in a category](../../../../../product-category-theory.md) $S^I$. The evaluation arrow

$$
e_B:B\to S^I,\qquad\pi_t e_B=t
$$

is a [monomorphism](../../../../../monomorphism.md), because $e_Bu=e_Bv$ forces $tu=tv$ for every $t$, and the [coseparator](../../../../../coseparator.md) then forces $u=v$.

By hypothesis this [monomorphism](../../../../../monomorphism.md) is a [regular monomorphism](../../../../../regular-monomorphism.md), so it is an [equalizer](../../../../../equaliser.md) of some $r,s:S^I\rightrightarrows Q$. Apply the same evaluation construction to $Q$: $J=\mathcal C(Q,S)$ is a set and $e_Q:Q\to S^J$ is monic. Cancelling $e_Q$ shows that equalizing $e_Qr,e_Qs$ is equivalent to equalizing $r,s$. We have therefore proved the [equalizer presentation by powers of a coseparator](../../../../../equalizer-presentation-by-powers-of-a-coseparator.md):

$$
\boxed{B\xrightarrow{e_B}S^I\mathrel{\substack{\xrightarrow{e_Qr}\\[-2pt]\xrightarrow[e_Qs]{} }}S^J.}
$$

The notation $S^I$ here means a product indexed by a set, so its existence does not presuppose categorical exponentiation.

If $A$ is an [exponentiable object](../../../../../exponentiable-object.md), $\mathcal C(-\times A,S)\cong\mathcal C(-,S^A)$ is a [representable functor](../../../../../representable-functor.md). Conversely, suppose a representing object $E$ and a natural isomorphism

$$
\mathcal C(X,E)\cong\mathcal C(X\times A,S)
$$

are given. For any set $I$, the [product in a category](../../../../../product-category-theory.md) property gives

$$
\mathcal C(X,E^I)\cong\mathcal C(X\times A,S^I).
$$

Thus maps into all powers of $S$ have representations. For an [equalizer](../../../../../equaliser.md) presentation $B\to S^I\rightrightarrows S^J$ with arrows $r,s$, postcomposition induces [natural transformations](../../../../../natural-transformation.md) between these represented functors. The [Yoneda lemma](../../../../../yoneda-lemma.md) identifies them with arrows $r_A,s_A:E^I\rightrightarrows E^J$. Form their [equalizer](../../../../../equaliser.md) $B_A$. Then

$$
\begin{aligned}
\mathcal C(X,B_A)
&\cong\operatorname{Eq}\bigl(\mathcal C(X,E^I)\rightrightarrows\mathcal C(X,E^J)\bigr)\\
&\cong\operatorname{Eq}\bigl(\mathcal C(X\times A,S^I)\rightrightarrows\mathcal C(X\times A,S^J)\bigr)\\
&\cong\mathcal C(X\times A,B).
\end{aligned}
$$

These bijections are natural in $X$. For a morphism $B\to C$, postcomposition and the [Yoneda lemma](../../../../../yoneda-lemma.md) give the unique arrow $B_A\to C_A$ respecting them; uniqueness proves functoriality. Hence $B\mapsto B_A$ is a [right adjoint](../../../../../adjoint-functors.md) to $-\times A$. This proves the [exponentiability test using a coseparator](../../../../../exponentiability-test-using-a-coseparator.md):

$$
\boxed{A\text{ is exponentiable}\iff\mathcal C(-\times A,S)\text{ is representable}.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
