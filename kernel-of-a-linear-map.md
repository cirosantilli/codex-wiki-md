# Kernel of a linear map

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Kernel_of_a_linear_map)

The [kernel of a linear map](kernel-of-a-linear-map.md) $T:V\to W$ is the [vector subspace](vector-subspace.md) of inputs sent to zero. [Linearity](linearity.md) makes it a [vector subspace](vector-subspace.md): if $T(v)=T(w)=0$, then $T(av+bw)=0$ for all [scalars](scalar.md) $a,b$. A [vector](vector.md) in the [kernel](kernel-of-a-linear-map.md) represents a change that the map cannot detect, since $T(x+v)=T(x)$ for every input $x$.

For $T:\mathbb R^3\to\mathbb R^2$ given by $T(x,y,z)=(x+y,z)$, the zero-output equations are $x+y=0$ and $z=0$. Thus

$$
\ker T=\operatorname{span}\{(1,-1,0)\}.
$$

Increasing the first input while decreasing the second by the same amount leaves the output unchanged. For the [linear functional](linear-functional.md) $\varphi(x,y)=2x-y$, the [kernel](kernel-of-a-linear-map.md) is the [straight line](straight-line.md) $y=2x$ shown in its diagram. A [linear map](linear-map.md) is [injective](injective-function.md) exactly when its [kernel](kernel-of-a-linear-map.md) is the zero [vector subspace](vector-subspace.md), because $T(v)=T(w)$ is equivalent to $T(v-w)=0$.

The [kernel](kernel-of-a-linear-map.md) describes invisible changes, rather than all inputs that produce a specified nonzero output. If $T(x_0)=b$, the corresponding [fiber of a function](fiber-of-a-function.md) is the [affine solution space of a linear equation](affine-solution-space-of-a-linear-equation.md) $x_0+\ker T$. The difference of two inputs in that [fiber](fiber-of-a-function.md) belongs to the [kernel](kernel-of-a-linear-map.md); an input in that [fiber](fiber-of-a-function.md) need not. In particular, for $b\ne0$ the [fiber](fiber-of-a-function.md) cannot be a [vector subspace](vector-subspace.md), since it does not contain the [zero vector](zero-vector.md).[Margalit and Rabinoff, Interactive Linear Algebra, §2.4.2, Key Observation and Remark: translate the homogeneous solution set by any particular solution](interactive-linear-algebra-by-dan-margalit-and-others/solution-sets.md)

For the [linear functional](linear-functional.md) $S:\mathbb R^2\to\mathbb R$, $S(x,y)=x+2y$, the [kernel](kernel-of-a-linear-map.md) is $\operatorname{span}\{(2,-1)\}$. Each [fiber](fiber-of-a-function.md) $S^{-1}(\{c\})$ is the parallel [straight line](straight-line.md) $(c,0)+\operatorname{span}\{(2,-1)\}$. The input [vector space](vector-space-split.md) is two-dimensional, but the output is one [scalar](scalar.md): a whole [straight line](straight-line.md) of inputs collapses to one point of the output [real line](real-line.md).

<a id="image-parallel-input-fibres-of-s-x-y-x-plus-2y-map-to-scalar-outputs"></a>
![](kernel-rank-one-parallel-fibres.png)

**[Figure 21](#image-parallel-input-fibres-of-s-x-y-x-plus-2y-map-to-scalar-outputs). Parallel input fibres of $S(x,y)=x+2y$ map to scalar outputs**. The blue input [straight line](straight-line.md) is the [kernel](kernel-of-a-linear-map.md); the other colored input [straight lines](straight-line.md) are its [translations](translation-geometry.md). The output panel is the one-dimensional [real line](real-line.md), drawn vertically for alignment. All displayed geometry is exact illustrative mathematics.

**Table of contents**

- [Null direction of a linear map](null-direction-of-a-linear-map.md)
- [Rectangular kernel and solution-fibre example](rectangular-kernel-and-solution-fibre-example.md)
- [Noninjective linear measurement](noninjective-linear-measurement.md)
- [Nullity of a linear map](nullity-of-a-linear-map.md)
- [Trivial kernel](trivial-kernel.md)
- [Rank-nullity theorem](rank-nullity-theorem.md)
  - [Equality in the rank-sum and nullity-product inequalities](equality-in-the-rank-sum-and-nullity-product-inequalities.md)
  - [Kernel jump in a parameter-dependent linear map](kernel-jump-in-a-parameter-dependent-linear-map.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (57)

- [Affine space of solutions of the Hodge Poisson equation](affine-space-of-solutions-of-the-hodge-poisson-equation.md)
- [Columns partition for finite-sums systems](columns-partition-for-finite-sums-systems.md)
- [Continuous dual space](continuous-dual-space-split.md)
- [Critical value](critical-value.md)
- [Determinant](determinant.md)
- [Even-weight subcode of a binary linear code](even-weight-subcode-of-a-binary-linear-code.md)
- [Factor base](factor-base.md)
- [Fixed-frequency nonradiating source](fixed-frequency-nonradiating-source.md)
- [Geometric Hahn-Banach theorem for radially open sets](geometric-hahn-banach-theorem-for-radially-open-sets.md)
- [Ground-state degeneracy](ground-state-degeneracy.md)
- [Homogeneous linear differential equation](homogeneous-linear-differential-equation.md)
- [Homogeneous linear system](homogeneous-linear-system.md)
- [Image criterion for a matrix factorization](image-criterion-for-a-matrix-factorization.md)
- [Inner product adapted to an idempotent linear map](inner-product-adapted-to-an-idempotent-linear-map.md)
- [Kernel (algebra)](kernel-algebra.md)
- [Kernel jump in a parameter-dependent linear map](kernel-jump-in-a-parameter-dependent-linear-map.md)
- [Kernel of a linear map](kernel-of-a-linear-map.md)
- [Linear differential equation](linear-differential-equation.md)
- [Linear functional](linear-functional.md)
- [Maximum-support vector in a finite-dimensional subspace](maximum-support-vector-in-a-finite-dimensional-subspace.md)
- [Normal matrices have equal adjoint norms](normal-matrices-have-equal-adjoint-norms.md)
- [Nullity of real N=1 supercharges](nullity-of-real-n-1-supercharges.md)
- [Orthogonal projection matrix](orthogonal-projection-matrix.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ia/paper-1/5c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-51/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-30/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ia/paper-1/6a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-3/19g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-3/11a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-85/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-3/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1/1g/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-1/7b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/6a/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/7b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/7b/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-15/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-1/6a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-2/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/6c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-1/6c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-12/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-3/3/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-76/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/8c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/8c/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-2/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ia/paper-1/8b/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/8e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-343/4/a/solution.md)
- [Projection (linear algebra)](projection-linear-algebra.md)
- [Tangent plane](tangent-plane.md)
