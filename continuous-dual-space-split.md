# Continuous dual space

↑ **Parent:** [Functional analysis](functional-analysis-split.md)

The [continuous dual space](continuous-dual-space-split.md) $X^*$ of a [topological vector space](topological-vector-space-split.md) is the [vector space](vector-space-split.md) of its [continuous linear functionals](continuous-linear-functional.md). Unlike the [algebraic dual](dual-space.md), it requires that a small change in an input produce a small change in its scalar measurement. For a [normed vector space](normed-vector-space.md), this is equivalent to a finite bound

$$
|\varphi(x)|\leq C\lVert x\rVert
$$

for all [vectors](vector.md) $x$ and some constant $C\geq0$. The least such constant is the [operator norm](operator-norm.md) of $\varphi$.

This is the continuity-restricted subspace of the algebraic [dual space](dual-space.md); in infinite dimension the two can differ.

For the [linear functional](linear-functional.md) $\varphi(x,y)=2x-y$ on $\mathbb R^2$ with its [Euclidean norm](euclidean-norm.md), the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives

$$
|\varphi(x,y)|\leq\sqrt5\sqrt{x^2+y^2}.
$$

Equality holds on the [unit vector](unit-vector.md) $(2,-1)/\sqrt5$, so its [operator norm](operator-norm.md) is exactly $\sqrt5$. The same estimate controls measurement error: $|\varphi(v+h)-\varphi(v)|\leq\sqrt5\lVert h\rVert_2$. The [linear functional](linear-functional.md) diagram shows which changes are entirely invisible to this measurement; its [kernel of a linear map](kernel-of-a-linear-map.md) consists of the changes with zero response. All [linear functionals](linear-functional.md) on a finite-dimensional real or complex [normed vector space](normed-vector-space.md) are continuous, but [discontinuous functional detected by vanishing sequence tails](discontinuous-functional-detected-by-vanishing-sequence-tails.md) shows why the restriction matters in infinite [dimension](dimension-vector-space.md).

**Table of contents**

- [Norming functional](norming-functional.md)
- [Norming subspace of a dual space](norming-subspace-of-a-dual-space.md)
  - [Vanishing sequences norm the summable sequence space](vanishing-sequences-norm-the-summable-sequence-space.md)
  - [Finite-codimensional weak-star dense dual subspace is norming](finite-codimensional-weak-star-dense-dual-subspace-is-norming.md)
- [Continuous-dual separation theorem for Hausdorff locally convex spaces](continuous-dual-separation-theorem-for-hausdorff-locally-convex-spaces.md)
- [Strong dual topology](strong-dual-topology.md)
- [Transpose of a bounded linear operator](transpose-of-a-bounded-linear-operator.md)
- [Positive linear functional](positive-linear-functional.md)
  - [Jordan decomposition of a bounded functional on C(K)](jordan-decomposition-of-a-bounded-functional-on-c-k.md)
  - [Positive extension from a unital subspace of C(K)](positive-extension-from-a-unital-subspace-of-c-k.md)
  - [Norm of a positive functional on C(K)](norm-of-a-positive-functional-on-c-k.md)
  - [Unital contraction positivity criterion](unital-contraction-positivity-criterion.md)
- [Operator norm](operator-norm.md)
  - [Riesz-Thorin theorem](riesz-thorin-theorem.md)
  - [Operator norm duality](operator-norm-duality.md)
  - [Euclidean logarithmic norm](euclidean-logarithmic-norm.md)
    - [Euclidean semigroup growth bounds](euclidean-semigroup-growth-bounds.md)
  - [Submultiplicativity of the operator norm](submultiplicativity-of-the-operator-norm.md)
  - [Telescoping bound for products of operators](telescoping-bound-for-products-of-operators.md)
    - [Unitary product telescoping](unitary-product-telescoping.md)
  - [Matrix 2-norm](matrix-2-norm.md)
- [Completeness of the dual space](completeness-of-the-dual-space.md)
- [Duality of sequence spaces](duality-of-sequence-spaces.md)
  - [Duality of l1 and l infinity](duality-of-l1-and-l-infinity.md)
    - [Schur property](schur-property.md)
      - [Gliding hump argument](gliding-hump-argument.md)
        - [Schur property of l1](schur-property-of-l1.md)
- [Duality of Lp spaces](duality-of-lp-spaces.md)
  - [Closed-hyperplane proof of Lp duality](closed-hyperplane-proof-of-lp-duality.md)
  - [Lp duality on an arbitrary measure space](lp-duality-on-an-arbitrary-measure-space.md)
    - [Support localization of an Lp functional](support-localization-of-an-lp-functional.md)
  - [Dual of L infinity is larger than L1](dual-of-l-infinity-is-larger-than-l1.md)
  - [Reflexivity of Lp spaces](reflexivity-of-lp-spaces.md)
  - [Positive functional representation on Lp](positive-functional-representation-on-lp.md)

## ↑ Ancestors (5)

1. [Functional analysis](functional-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (48)

- [Bounded bilinear form](bounded-bilinear-form.md)
- [Closed unit ball](closed-unit-ball.md)
- [Compactly supported distribution space](compactly-supported-distribution-space.md)
- [Continuous dual space](continuous-dual-space-split.md)
- [Continuous linear functional](continuous-linear-functional.md)
- [Dual space](dual-space.md)
- [Duality of Lp spaces](duality-of-lp-spaces.md)
- [Linear functional](linear-functional.md)
- [Locally convex space](locally-convex-space.md)
- [Original and weak continuity of linear maps between Fréchet spaces](original-and-weak-continuity-of-linear-maps-between-frechet-spaces.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-6/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-3/21f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/22g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-11/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-10/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-5/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-6/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-5/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-6/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-71/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326/3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-2/22f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-3/21f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-106/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/22h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-326/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/22i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/22i/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-3/22i/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-327/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327/1/a/solution.md)
- [2](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-327/2.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/22f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-1/22f/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-327/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-106/4/a/solution.md)
- [Regular Borel measure](regular-borel-measure.md)
- [Separable Banach space](separable-banach-space.md)
- [Strong dual topology](strong-dual-topology.md)
- [Weak convergence](weak-convergence.md)
- [Weakly bounded set](weakly-bounded-set.md)
- [Weakly compact set is norm bounded](weakly-compact-set-is-norm-bounded.md)
- [Weakly null sequence](weakly-null-sequence.md)
