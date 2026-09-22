# Rank-nullity theorem

↑ **Parent:** [Kernel of a linear map](kernel-of-a-linear-map-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rank-nullity_theorem)

The [rank-nullity theorem](rank-nullity-theorem.md) accounts for the input dimensions of a [linear map](linear-map.md): the number of independent invisible input directions plus the number of independent reachable output directions equals the input [dimension](dimension-vector-space.md). For $T:V\to W$ over a [field](field.md), with finite-dimensional [domain of a function](domain-of-a-function.md) $V$,

$$
\boxed{\dim V=\dim\ker T+\dim\operatorname{im}T.}
$$

Here $\dim\ker T$ is the [nullity](nullity-of-a-linear-map.md), and $\dim\operatorname{im}T$ is the [rank of a linear map](rank-of-a-linear-map.md). The [kernel](kernel-of-a-linear-map-split.md) lives in the input [vector space](vector-space-split.md), while the [image of a linear map](image-of-a-linear-map.md) lives in the output [vector space](vector-space-split.md). For an $m$-by-$n$ [matrix](matrix.md) of [matrix rank](matrix-rank.md) $r$, the formula is $n=(n-r)+r$: the number of columns counts input coordinates. [Sheldon Axler, Linear Algebra Done Right, fourth edition, §3B: fundamental theorem of linear maps](linear-algebra-done-right-by-sheldon-axler-4th-edition.md)

For a computed example over the [real numbers](real-number.md), take

$$
A=\begin{pmatrix}1&2\\0&0\end{pmatrix},\qquad
T(x,y)=A\begin{pmatrix}x\\y\end{pmatrix}=(x+2y,0).
$$

The [kernel](kernel-of-a-linear-map-split.md) is $\operatorname{span}\{(-2,1)\}$ and the [image of a linear map](image-of-a-linear-map.md) is $\operatorname{span}\{(1,0)\}$. Each has [dimension](dimension-vector-space.md) one, so the two input dimensions split as $2=1+1$. The [vector](vector.md) $(3,1)$ can be written

$$
(3,1)=(1,2)+(2,-1),\qquad
T(1,2)=(5,0),\qquad T(2,-1)=(0,0).
$$

The second summand is undetectable: $T(3,1)=T(1,2)$. The picture uses the standard [dot product](dot-product.md) to choose a visible direction perpendicular to the [kernel](kernel-of-a-linear-map-split.md); this is a convenient geometric choice, not an extra hypothesis of the [rank-nullity theorem](rank-nullity-theorem.md).

<a id="image-two-input-dimensions-split-into-one-visible-direction-and-one-kernel-direction"></a>
![](rank-nullity-domain-decomposition.png)

**[Figure 4](#image-two-input-dimensions-split-into-one-visible-direction-and-one-kernel-direction). Two input dimensions split into one visible direction and one kernel direction**. For $T(x,y)=(x+2y,0)$, the input $(3,1)$ splits into $(1,2)$ and $(2,-1)$. Both $(3,1)$ and $(1,2)$ map to $(5,0)$, while the [kernel](kernel-of-a-linear-map-split.md) component maps to zero. The horizontal output line is the entire [image of a linear map](image-of-a-linear-map.md).

This explains a practical tradeoff in a [linear system](system-of-linear-equations.md). If $T(x_0)=b$, every other input with output $b$ is $x_0+k$ for $k\in\ker T$. The [nullity](nullity-of-a-linear-map.md) therefore counts independent freedom in an existing solution; the [rank](rank-one-quadratic-form.md) counts independent reachable output directions. In the example, $T(x,y)=(3,0)$ has all solutions $(x,y)=(3-2t,t)$, while $T(x,y)=(3,1)$ has none. The [cokernel](cokernel.md) records this failure of reachability.

For an $m$-by-$n$ [matrix](matrix.md), [injectivity](injective-function.md) requires [matrix rank](matrix-rank.md) $n$, and [surjectivity](surjective-function.md) requires [matrix rank](matrix-rank.md) $m$. When $m\ne n$, these conditions differ. For example, $B:\mathbb R^3\to\mathbb R^2$ with $B(x,y,z)=(x+2y,0)$ has [rank](rank-one-quadratic-form.md) one and [nullity](nullity-of-a-linear-map.md) two, because $\ker B=\operatorname{span}\{(-2,1,0),(0,0,1)\}$. The input accounting is $3=2+1$, although only one of two output directions is reached.

Proof outline: extend a [basis](basis.md) $k_1,\ldots,k_q$ of the [kernel](kernel-of-a-linear-map-split.md) to a [basis](basis.md) $k_1,\ldots,k_q,v_1,\ldots,v_r$ of $V$. Every output is a [linear combination](linear-combination.md) of $T(v_1),\ldots,T(v_r)$ because the $k_i$ vanish under $T$. If a [linear combination](linear-combination.md) of the $T(v_j)$ is zero, the corresponding combination of the $v_j$ lies in the [kernel](kernel-of-a-linear-map-split.md); [linear independence](linear-independence.md) of the full [basis](basis.md) forces all its coefficients to vanish. Thus the added [basis vectors](basis-vector.md) give a [basis](basis.md) of the [image of a linear map](image-of-a-linear-map.md). Counting them proves the formula.

**Table of contents**

- [Equality in the rank-sum and nullity-product inequalities](equality-in-the-rank-sum-and-nullity-product-inequalities.md)
- [Kernel jump in a parameter-dependent linear map](kernel-jump-in-a-parameter-dependent-linear-map.md)

## ↑ Ancestors (6)

1. [Kernel of a linear map](kernel-of-a-linear-map-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (87)

- [Cokernel](cokernel.md)
- [Complementarity from two directed subspace angles](complementarity-from-two-directed-subspace-angles.md)
- [Critical value](critical-value.md)
- [Dual image and kernel annihilator identity](dual-image-and-kernel-annihilator-identity.md)
- [Endomorphism](endomorphism.md)
- [Even-weight subcode of a binary linear code](even-weight-subcode-of-a-binary-linear-code.md)
- [Homogeneous linear system](homogeneous-linear-system.md)
- [Invertible matrix](invertible-matrix.md)
- [Johnson–Lindenstrauss lemma](johnson-lindenstrauss-lemma.md)
- [Kernel jump in a parameter-dependent linear map](kernel-jump-in-a-parameter-dependent-linear-map.md)
- [Matrix inverse](matrix-inverse-split.md)
- [Matrix rank](matrix-rank.md)
- [Nullity of a linear map](nullity-of-a-linear-map.md)
- [One-sided inverses of finite-dimensional endomorphisms](one-sided-inverses-of-finite-dimensional-endomorphisms.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/15c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/1a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-3/7a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/6f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2/15e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-2/6e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4/15g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-36/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-7/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ia/paper-1/5b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-1/6b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/9h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/10h/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ia/paper-1/2b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-2/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1/1g/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-50/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/6a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/7b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-1/9e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-13/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-36/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-45/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-9/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-10/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/6c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/8c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/8c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/10f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-116/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ia/paper-1/8c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-1/2a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-1/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/11g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/8f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-1/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/9e/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/1e/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/8e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/31j/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-4/8f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-115/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-1/2c/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-1/2c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ib/paper-1/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ia/paper-1/6c/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/15/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/7/solution.md)
- [Polynomial evaluation map on a finite point set](polynomial-evaluation-map-on-a-finite-point-set.md)
- [Pruning and minimal-degree polynomial argument](pruning-and-minimal-degree-polynomial-argument.md)
- [Rank cancellation in the Euler-Poincare formula](rank-cancellation-in-the-euler-poincare-formula.md)
- [Rank-nullity theorem](rank-nullity-theorem.md)
- [Reading solutions from reduced row echelon form](reading-solutions-from-reduced-row-echelon-form.md)
- [Rectangular kernel and solution-fibre example](rectangular-kernel-and-solution-fibre-example.md)
- [Separating subspace of an algebraic dual](separating-subspace-of-an-algebraic-dual.md)
- [Subgroup generator bound for a powerful finite p-group](subgroup-generator-bound-for-a-powerful-finite-p-group.md)
- [System of linear equations](system-of-linear-equations.md)
- [Trivial kernel](trivial-kernel.md)
- [Vector space](vector-space-split.md)
