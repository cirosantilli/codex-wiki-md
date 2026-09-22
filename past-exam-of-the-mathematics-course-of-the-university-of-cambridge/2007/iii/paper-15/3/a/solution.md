<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [connection on a vector bundle](../../../../../../connection-vector-bundle.md) is a linear operator $\nabla:\Gamma(E)\to\Omega^1(M;E)$ satisfying $\nabla(fs)=df\otimes s+f\nabla s$. Choose coordinates $x^i$ and a [local frame](../../../../../../frame-of-a-vector-bundle.md) $e_1,\ldots,e_m$, and define the [connection matrix](../../../../../../connection-one-form.md) by $\nabla e_b=\sum_a A^a{}_b\otimes e_a$, with $A^a{}_b=\sum_iA^a{}_{b i}dx^i$. For a section $s=\sum_a s^ae_a$, the coefficient column satisfies

$$
\boxed{d_As=ds+As,\qquad
(\nabla_i s)^a=\partial_i s^a+\sum_b A^a{}_{b i}s^b.}
$$

The symbol $d$ on the right means the ordinary [exterior derivative](../../../../../../exterior-derivative.md) of the coefficient functions.

Extend uniquely to $E$-valued [differential forms](../../../../../../differential-form-split.md) by the graded [Leibniz rule](../../../../../../leibniz-rule.md)

$$
d_A(\alpha s)=d\alpha\otimes s+(-1)^r\alpha\wedge\nabla s,
\qquad \alpha\in\Omega^r(M).
$$

In the same [local trivialization](../../../../../../local-trivialization.md), an $E$-valued form is a column $\sigma=(\sigma^a)$ and the [covariant exterior derivative](../../../../../../exterior-covariant-derivative.md) is

$$
\boxed{(d_A\sigma)^a=d\sigma^a+\sum_b A^a{}_b\wedge\sigma^b,\qquad d_A=d+A\wedge.}
$$

Moving the one-form $A$ past the scalar $r$-form produces exactly the $(-1)^r$ in the graded rule. This explains the sign rather than replacing the rule by an ungraded product formula.

The [endomorphism bundle](../../../../../../endomorphism-bundle.md) has the induced [endomorphism bundle connection](../../../../../../endomorphism-bundle-connection.md) characterized on sections by $\nabla^{\operatorname{End}}_X(T)s=\nabla_X(Ts)-T\nabla_Xs$. Its coefficient formula is $dT+AT-TA$. On an [endomorphism](../../../../../../endomorphism.md)-valued $r$-form $T$, extend as a [graded derivation](../../../../../../graded-derivation.md) of the [endomorphism-valued exterior product](../../../../../../endomorphism-valued-exterior-product.md), giving

$$
\boxed{d_A^{\operatorname{End}}T=dT+A\wedge T-(-1)^rT\wedge A.}
$$

Explicitly its $(a,b)$ entry is $dT^a{}_b+\sum_cA^a{}_c\wedge T^c{}_b-(-1)^r\sum_cT^a{}_c\wedge A^c{}_b$. This version is characterized by

$$
d_A(T\wedge\sigma)=(d_A^{\operatorname{End}}T)\wedge\sigma+(-1)^rT\wedge d_A\sigma.
$$

The [endomorphism](../../../../../../endomorphism.md)-valued version also satisfies $d_A(T\wedge S)=d_AT\wedge S+(-1)^rT\wedge d_AS$. Products here combine composition of [endomorphisms](../../../../../../endomorphism.md) with wedge products of coefficient forms; [matrix](../../../../../../matrix.md) factors must retain their order.

These local formulas are independent of the [local frame](../../../../../../frame-of-a-vector-bundle.md). For $e'=eg$, the [change of frame of a vector-bundle connection](../../../../../../change-of-frame-of-a-vector-bundle-connection.md) gives $A'=g^{-1}Ag+g^{-1}dg$, $\sigma'=g^{-1}\sigma$ and $T'=g^{-1}Tg$. Using $d(g^{-1})=-g^{-1}(dg)g^{-1}$ gives $d_{A'}\sigma'=g^{-1}d_A\sigma$ and $d_{A'}T'=g^{-1}(d_AT)g$. Thus both extended operators are globally defined.

## ↑ Ancestors (11)

1. [A](../a.md)
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
