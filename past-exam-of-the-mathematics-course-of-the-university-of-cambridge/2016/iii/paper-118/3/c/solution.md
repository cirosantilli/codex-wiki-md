<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [orthogonal projection](../../../../../../orthogonal-projection.md) $\pi_S$ is a smooth bundle map, since the [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) and the subbundle vary smoothly. The map

$$
E/S\longrightarrow S^\perp,\qquad [v]\longmapsto(I-\pi_S)v
$$

is independent of the representative, bijective on each fibre, and smooth with smooth inverse supplied by the quotient map on $S^\perp$. Hence it is a natural isomorphism of smooth [vector bundles](../../../../../../vector-bundle.md). It need not be holomorphic. The [quotient Hermitian metric](../../../../../../quotient-hermitian-metric.md) is

$$
\boxed{h_Q([v],[w])=h_E((I-\pi_S)v,(I-\pi_S)w).}
$$

It is well-defined and positive definite because $S^\perp$ represents each quotient class uniquely.

On sections of $S$, set $D'=\pi_S D_E$. The [Leibniz rule](../../../../../../leibniz-rule.md) makes $D'$ a [connection on a vector bundle](../../../../../../connection-vector-bundle.md). For $s,t\in\Gamma(S)$, the orthogonal terms vanish in the metric pairing, so

$$
dh_S(s,t)=h_S(D's,t)+h_S(s,D't).
$$

Thus $D'$ has [metric compatibility](../../../../../../metric-compatibility.md). Because $S$ is a holomorphic subbundle, the $(0,1)$ part of $D_E$ preserves $S$ and restricts to $\bar\partial_S$. Therefore $(D')^{0,1}=\bar\partial_S$. The uniqueness of the [Chern connection](../../../../../../chern-connection.md) in part (b) gives the [projected Chern connection](../../../../../../projected-chern-connection.md) formula

$$
\boxed{D_S=\pi_S D_E.}
$$

It follows that $A(s)=(I-\pi_S)D_Es$ is a quotient-valued one-form. **The printed target $T_M\otimes Q$ is missing a dual:** the [cotangent bundle](../../../../../../cotangent-bundle.md) is the correct factor,

$$
\boxed{A(s)\in\Gamma(T_M^*\otimes Q).}
$$

Complex-valued forms use the complexified cotangent bundle here. In fact the $(0,1)$ part cancels, so $A$ is the [second fundamental form of a holomorphic subbundle](../../../../../../second-fundamental-form-of-a-holomorphic-subbundle.md), an element of $\mathcal A^{1,0}(\operatorname{Hom}(S,Q))$. Finally the two connection [Leibniz rules](../../../../../../leibniz-rule.md) give

$$
A(fs)=df\otimes s+fD_Es-df\otimes s-fD_Ss
=\boxed{fA(s)}.
$$

This proves its [tensoriality](../../../../../../tensoriality.md) and all the asserted quotient and projection properties.

## ↑ Ancestors (11)

1. [C](../c.md)
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
