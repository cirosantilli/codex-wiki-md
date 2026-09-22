# Seminorm

↑ **Parent:** [Locally convex space](locally-convex-space.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Seminorm)

A seminorm on a real or complex [vector space](vector-space-split.md) $E$ is a finite-valued [function](function-split.md) $p:E\to[0,\infty)$ satisfying absolute homogeneity and the [triangle inequality](triangle-inequality.md):

$$
p(\lambda x)=|\lambda|p(x),\qquad p(x+y)\leq p(x)+p(y)
\qquad(x,y\in E,\ \lambda\in\mathbb K).
$$

In particular $p(0)=0$ and $p(-x)=p(x)$. A [seminorm](seminorm.md) is a [norm](norm.md) exactly when $p(x)=0$ implies $x=0$: this is the extra [definiteness of a norm](definiteness-of-a-norm.md) axiom. The zero [function](function-split.md) is a valid [seminorm](seminorm.md). The missing definiteness is useful when a measurement deliberately ignores some directions, such as an individual coordinate or the constant term of a [function](function-split.md) whose [derivative](derivative.md) is measured.

For example, on $C^1([0,1])$ the [function](function-split.md) $p(f)=\sup_{t\in[0,1]}|f'(t)|$ is a [seminorm](seminorm.md) that vanishes on every constant [function](function-split.md). Adding the value measurement gives the [norm](norm.md) $q(f)=|f(0)|+p(f)$: if $q(f)=0$, the [fundamental theorem of calculus](fundamental-theorem-of-calculus.md) gives $f(t)=f(0)+\int_0^t f'(s)\,ds=0$. A family of such partial measurements defines a [seminorm topology](seminorm-topology.md).

**Table of contents**

- [Kernel of a seminorm](kernel-of-a-seminorm.md)
- [Coordinate seminorms](coordinate-seminorms.md)
- [Dual seminorm](dual-seminorm.md)

## ↑ Ancestors (7)

1. [Locally convex space](locally-convex-space.md)
2. [Topological vector space](topological-vector-space-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (44)

- [Bounded set in a topological vector space](bounded-set-in-a-topological-vector-space.md)
- [Continuous-dual separation theorem for Hausdorff locally convex spaces](continuous-dual-separation-theorem-for-hausdorff-locally-convex-spaces.md)
- [Coordinate seminorms](coordinate-seminorms.md)
- [Derivative seminorms on a compact interval](derivative-seminorms-on-a-compact-interval.md)
- [Dual seminorm](dual-seminorm.md)
- [Dual Thurston polytope](dual-thurston-polytope.md)
- [Fourier transform isomorphism of the Schwartz space](fourier-transform-isomorphism-of-the-schwartz-space.md)
- [Hermitian inner product](hermitian-inner-product.md)
- [Kernel of a seminorm](kernel-of-a-seminorm.md)
- [Locally convex space](locally-convex-space.md)
- [Open mapping theorem for Fréchet spaces](open-mapping-theorem-for-frechet-spaces.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-6/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-6/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-79/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-5/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-68/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-60/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-7/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-14/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-327/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-327/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-327/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-327/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-117/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327/3/b/solution.md)
- [Schwartz seminorm](schwartz-seminorm.md)
- [Seminorm](seminorm.md)
- [Seminorm topology](seminorm-topology.md)
- [Separating family of seminorms](separating-family-of-seminorms.md)
- [Separation of a point from a closed linear subspace](separation-of-a-point-from-a-closed-linear-subspace.md)
- [Sequential continuity criterion in a metrizable vector space](sequential-continuity-criterion-in-a-metrizable-vector-space.md)
- [Test-function inductive limit topology](test-function-inductive-limit-topology.md)
- [Test-function seminorm](test-function-seminorm.md)
- [Thurston norm](thurston-norm.md)
