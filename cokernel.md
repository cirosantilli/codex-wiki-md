# Cokernel

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Cokernel)

The [cokernel](cokernel.md) records output information that a [linear map](linear-map.md) cannot produce. For $T:V\to W$, it is the [quotient vector space](quotient-vector-space.md)

$$
\operatorname{coker}T=W/\operatorname{im}T.
$$

Its elements are [cosets](coset.md) $[b]=b+\operatorname{im}T$. Two [vectors](vector.md) $b,c\in W$ represent the same class exactly when $b-c$ is in the [image of a linear map](image-of-a-linear-map.md). The zero class is the whole [image of a linear map](image-of-a-linear-map.md), so

$$
\boxed{T(x)=b\text{ is solvable}\iff[b]=0\text{ in }\operatorname{coker}T.}
$$

Changing $b$ by an attainable output does not change its obstruction. This is useful because one can test compatibility before trying to find an input. The [quotient vector space](quotient-vector-space.md) construction is described in Axler's §3E. [Sheldon Axler, Linear Algebra Done Right, fourth edition, §3E: quotient spaces](linear-algebra-done-right-by-sheldon-axler-4th-edition.md)

For the [linear map](linear-map.md) $T:\mathbb R^2\to\mathbb R^2$ given by $T(x,y)=(x+2y,0)$, the [image of a linear map](image-of-a-linear-map.md) is the horizontal line. All outputs $(b_1,b_2)$ with the same second coordinate have the same [cokernel](cokernel.md) class, because their difference is horizontal. Thus this [cokernel](cokernel.md) is [isomorphic](isomorphism.md) to $\mathbb R$ via $[(b_1,b_2)]\mapsto b_2$. In particular, $(3,0)$ has zero class and is attainable, while $(3,1)$ has nonzero class and is unattainable.

<a id="image-the-second-output-coordinate-is-a-cokernel-obstruction-to-solving-t-x-y-b"></a>
![](cokernel-solvability-obstruction.png)

**[Figure 25](#image-the-second-output-coordinate-is-a-cokernel-obstruction-to-solving-t-x-y-b). The second output coordinate is a cokernel obstruction to solving $T(x,y)=b$**. The horizontal axis is the [image of a linear map](image-of-a-linear-map.md) $T(x,y)=(x+2y,0)$. The class of $b=(3,1)$ is the parallel line $b+\operatorname{im}T$, which never meets the image. The projection $(3,0)$ is attainable but has a different [cokernel](cokernel.md) class.

If $W$ is finite-dimensional, the dimension rule for a [quotient vector space](quotient-vector-space.md) gives

$$
\dim W=\operatorname{rank}T+\dim\operatorname{coker}T.
$$

Compare this with the [rank-nullity theorem](rank-nullity-theorem.md), $\dim V=\operatorname{rank}T+\dim\ker T$. The [kernel](kernel-of-a-linear-map.md) counts invisible inputs; the [cokernel](cokernel.md) counts missing output directions. They need not have the same [dimension](dimension-vector-space.md): $B(x,y,z)=(x+2y,0)$ has a two-dimensional [kernel](kernel-of-a-linear-map.md) and a one-dimensional [cokernel](cokernel.md). A [linear map](linear-map.md) is [surjective](surjective-function.md) exactly when its [cokernel](cokernel.md) is zero.

The [cokernel](cokernel.md) is a quotient, rather than a chosen perpendicular [vector subspace](vector-subspace.md). With a finite-dimensional [inner product space](inner-product-space.md) as output, one may represent each class by its unique component in the [orthogonal complement](orthogonal-complement.md) of the [image of a linear map](image-of-a-linear-map.md). That representation depends on the chosen [inner product](inner-product.md). For [matrices](matrix.md) over the [complex numbers](complex-number.md), this complement is $\ker A^*$, leading to the [cokernel compatibility equations](cokernel-compatibility-equations.md).

The same quotient definition applies to a [group homomorphism](group-homomorphism.md) of [abelian groups](abelian-group.md). For $T:\mathbb Z\to\mathbb Z$ given by $T(n)=2n$, the [cokernel](cokernel.md) is $\mathbb Z/2\mathbb Z$. The equation $2n=b$ is solvable exactly when $b$ is an [even integer](even-number.md); the two [cosets](coset.md) record [integer parity](parity-mathematics.md). A quotient captures the obstruction here just as it captures a missing output coordinate for a [linear map](linear-map.md).

**Table of contents**

- [Cokernel compatibility equations](cokernel-compatibility-equations.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (32)

- [Cokernel](cokernel.md)
- [Cokernel compatibility equations](cokernel-compatibility-equations.md)
- [Compact perturbation invariance of Fredholm operators](compact-perturbation-invariance-of-fredholm-operators.md)
- [Finitely generated abelian group](finitely-generated-abelian-group.md)
- [Fredholm index](fredholm-index.md)
- [Generic transversality for simple holomorphic spheres](generic-transversality-for-simple-holomorphic-spheres.md)
- [Godement resolution](godement-resolution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-13/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-1/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-14/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-26/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-17/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-16/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-17/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-2/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-16/1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7/3/f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-3/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-16/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-16/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-3/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-3/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-101/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-127/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-128/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/11g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-4/21f/b/solution.md)
- [Rank-nullity theorem](rank-nullity-theorem.md)
