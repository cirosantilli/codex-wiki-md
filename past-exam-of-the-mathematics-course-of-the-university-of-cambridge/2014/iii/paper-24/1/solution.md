<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [absolute value on a field](../../../../../absolute-value-algebra.md) is a map $|\cdot|:K\to\mathbb R_{\geq0}$ satisfying

$$
|x|=0\Longleftrightarrow x=0,\qquad |xy|=|x||y|,\qquad |x+y|\leq|x|+|y|.
$$

A [Non-Archimedean absolute value](../../../../../non-archimedean-absolute-value.md) satisfies the stronger [ultrametric inequality](../../../../../ultrametric-inequality.md) $|x+y|\leq\max(|x|,|y|)$. Two [equivalent absolute values](../../../../../equivalent-absolute-values.md) induce the same [topology](../../../../../topology-split.md), or equivalently differ by a positive real power. The trivial [absolute value on a field](../../../../../absolute-value-algebra.md) takes value one on every nonzero element. The rational classification and the compactness criterion below concern nontrivial [absolute values on a field](../../../../../absolute-value-algebra.md); the trivial exceptions are given explicitly.

Here the additive [valuation](../../../../../valuation.md) has real values. For any $c>1$, the mutually inverse constructions are

$$
v(x)=-\log_c|x|,\quad v(0)=+\infty,\qquad |x|=c^{-v(x)}.
$$

Multiplicativity becomes $v(xy)=v(x)+v(y)$, and the [ultrametric inequality](../../../../../ultrametric-inequality.md) becomes $v(x+y)\geq\min(v(x),v(y))$. Equivalent real-valued [valuations](../../../../../valuation.md) differ by positive scaling, so these constructions give the required **bijection on equivalence classes**. Changing $c$ merely rescales the [valuation](../../../../../valuation.md).

To justify the topology formulation, $|a|<1$ is equivalent to $a^n\to0$. Thus two nontrivial [absolute values on a field](../../../../../absolute-value-algebra.md) with the same [topology](../../../../../topology-split.md) give the same strict positivity relation on their additive [valuations](../../../../../valuation.md). Fix $t$ with $v_1(t)>0$. Comparing the signs of $m v_j(t)-n v_j(x)=v_j(t^m x^{-n})$, for integers $m$ and positive integers $n$, shows that $v_1(x)/v_1(t)$ and $v_2(x)/v_2(t)$ have identical rational cuts. They are equal, proving $v_2=c v_1$ for $c>0$. If one allows [valuations](../../../../../valuation.md) in arbitrary ordered groups, the nontrivial classes arising this way are precisely [rank-one valuations](../../../../../rank-one-valuation.md): higher-rank ordered value groups do not embed order-preservingly in $\mathbb R$.

For a nontrivial [Non-Archimedean absolute value](../../../../../non-archimedean-absolute-value.md) on $\mathbb Q$, $|n|\leq1$ for every integer $n$, by repeatedly applying the [ultrametric inequality](../../../../../ultrametric-inequality.md) to sums of ones. Some prime $p$ must have $|p|<1$, otherwise [prime factorization](../../../../../fundamental-theorem-of-arithmetic.md) and multiplicativity would make every nonzero rational have value one. There is at most one such prime: if both $|p|,|q|<1$, a [Bezout identity](../../../../../bezout-identity.md) $a p+b q=1$ contradicts the [ultrametric inequality](../../../../../ultrametric-inequality.md). If $p\nmid m$, another [Bezout identity](../../../../../bezout-identity.md) gives $|m|=1$. Hence

$$
\boxed{|x|=|p|^{v_p(x)}=|x|_p^{\alpha},\qquad \alpha=-\frac{\log|p|}{\log p}>0.}
$$

This proves the non-Archimedean part of the [Ostrowski theorem](../../../../../ostrowski-s-theorem.md). If the trivial [absolute value on a field](../../../../../absolute-value-algebra.md) is admitted, it supplies one additional class and is not equivalent to any [p-adic absolute value](../../../../../p-adic-absolute-value.md).

The [valuation ring](../../../../../valuation-ring.md), its [maximal ideal](../../../../../maximal-ideal.md), and its [residue field](../../../../../residue-field.md) are

$$
R=\{x:|x|\leq1\},\qquad\mathfrak m=\{x:|x|<1\},\qquad k=R/\mathfrak m.
$$

Suppose the [absolute value on a field](../../../../../absolute-value-algebra.md) is nontrivial and $R$ is [compact](../../../../../compact-space.md). The ideal $\mathfrak m$ is an open additive subgroup of $R$, so $k$ is discrete; as a continuous image of a [compact](../../../../../compact-space.md) space it is finite. The subgroup $\mathfrak m$ is also closed, since all its cosets are open, and is therefore [compact](../../../../../compact-space.md). The continuous function $|\cdot|$ attains a maximum $\rho$ on $\mathfrak m$, with $0<\rho<1$. Choose $\pi$ with $|\pi|=\rho$. Then the positive values of $v=-\log|\cdot|$ have least element $-\log\rho$. Division with remainder in this additive subgroup of $\mathbb R$ proves $v(K^\times)=v(\pi)\mathbb Z$. Thus $K$ is a [discretely valued field](../../../../../discretely-valued-field.md) and $\pi$ is a [uniformizer](../../../../../uniformizer.md).

Conversely, normalize the [discrete valuation](../../../../../discrete-valuation.md) by $v(\pi)=1$. If $k$ has $q$ elements, $R/\pi^N R$ has $q^N$ elements. Each quotient therefore supplies a finite cover by balls of radius tending to zero. The ring $R$ is a closed subset of the complete metric field $K$, hence complete and [totally bounded](../../../../../totally-bounded-space.md), so it is [compact](../../../../../compact-space.md). Equivalently,

$$
\boxed{R\cong\varprojlim_N R/\pi^N R,\qquad R\text{ compact}\Longleftrightarrow v(K^\times)\text{ discrete and }|k|<\infty.}
$$

This is the [local compactness criterion for a complete non-Archimedean field](../../../../../local-compactness-criterion-for-a-complete-non-archimedean-field.md), with nontriviality understood. For the trivial [absolute value on a field](../../../../../absolute-value-algebra.md), $R=K$ has the discrete [topology](../../../../../topology-split.md) and is [compact](../../../../../compact-space.md) exactly when $K$ is a finite [field](../../../../../field.md); its value group is zero rather than a nonzero discrete cyclic group.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
