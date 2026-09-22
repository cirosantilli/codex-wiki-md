# Dual space

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Dual_space)

The [dual space](dual-space.md) of a [vector space](vector-space-split.md) $V$ over a [field](field.md) $F$ is the [vector space](vector-space-split.md) of all [linear functionals](linear-functional.md) $\varphi:V\to F$. Think of a [vector](vector.md) as an input and a [linear functional](linear-functional.md) as a scalar-valued measurement of that input. For $V=\mathbb R^2$, the rules $(x,y)\mapsto x$, $(x,y)\mapsto y$, and $(x,y)\mapsto2x-y$ are different elements of the [dual space](dual-space.md). None needs a notion of [length](length.md) or [angle](angle.md).

Its operations combine measurements pointwise:

$$
(\varphi+\psi)(v)=\varphi(v)+\psi(v),\qquad
(a\varphi)(v)=a\varphi(v).
$$

The [dual basis](dual-basis.md) explains the finite-dimensional structure: specifying a [linear functional](linear-functional.md)'s values on a [basis](basis.md) determines its value on every [vector](vector.md). Thus an $n$-dimensional [vector space](vector-space-split.md) has an $n$-dimensional [dual space](dual-space.md). The spaces have the same [dimension](dimension-vector-space.md), but their elements play different roles: an input and a rule that measures an input. [Axler, Linear Algebra Done Right, fourth edition, §3F, definitions 3.109–3.112](linear-algebra-done-right-by-sheldon-axler-4th-edition.md).

This separation is useful when changing coordinates. The [dual pairing](dual-pairing.md) $\varphi(v)$ must stay the same while the component lists for $v$ and $\varphi$ change in opposite ways. [Covector transformation under a change of basis](covector-transformation-under-a-change-of-basis.md) makes the compensation explicit. An [inner product](inner-product.md) on a finite-dimensional real [vector space](vector-space-split.md) gives one way to represent each [linear functional](linear-functional.md) by a [vector](vector.md), but that representation uses the chosen [inner product](inner-product.md); the [dual space](dual-space.md) itself does not require one.

Here [dual space](dual-space.md) means the [algebraic dual](dual-space.md): all [linear functionals](linear-functional.md). For a [topological vector space](topological-vector-space-split.md), the [continuous dual space](continuous-dual-space-split.md) keeps only the [continuous linear functionals](continuous-linear-functional.md). In infinite [dimension](dimension-vector-space.md), this can be a proper [vector subspace](vector-subspace.md); [discontinuous functional detected by vanishing sequence tails](discontinuous-functional-detected-by-vanishing-sequence-tails.md) gives an example. The distinction matters when a scalar-valued measurement must respond continuously to small input changes.

**Table of contents**

- [Dual pairing](dual-pairing.md)
- [Algebraic dual of a direct sum](algebraic-dual-of-a-direct-sum.md)
- [Bidual of a normed space](bidual-of-a-normed-space.md)
- [Perfect pairing](perfect-pairing.md)
- [Separating subspace of an algebraic dual](separating-subspace-of-an-algebraic-dual.md)
- [Bidual evaluation map](bidual-evaluation-map.md)
- [Covector](covector.md)
  - [Covector transformation under a change of basis](covector-transformation-under-a-change-of-basis.md)
- [Linear functional](linear-functional.md)
  - [Minimizing a linear functional on a sphere](minimizing-a-linear-functional-on-a-sphere.md)
  - [Discontinuous functional detected by vanishing sequence tails](discontinuous-functional-detected-by-vanishing-sequence-tails.md)
- [Dual basis](dual-basis.md)
  - [Coordinate functional](coordinate-functional.md)
  - [Factorial monomial basis for polynomial differentiation](factorial-monomial-basis-for-polynomial-differentiation.md)
- [Annihilator of a vector subspace](annihilator-of-a-vector-subspace.md)
- [Transpose of a linear map](transpose-of-a-linear-map.md)
  - [Dual image and kernel annihilator identity](dual-image-and-kernel-annihilator-identity.md)
  - [Equality of row rank and column rank](equality-of-row-rank-and-column-rank.md)
    - [Simultaneous basis exchange from a nonzero minor](simultaneous-basis-exchange-from-a-nonzero-minor.md)
  - [Duals of a subspace and its quotient](duals-of-a-subspace-and-its-quotient.md)
- [Surjectivity of independent linear functionals](surjectivity-of-independent-linear-functionals.md)
- [Polynomial moment functional](polynomial-moment-functional.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (45)

- [Algebraic contragredient representation](algebraic-contragredient-representation.md)
- [Algebraic dual of a direct sum](algebraic-dual-of-a-direct-sum.md)
- [Bidual evaluation map](bidual-evaluation-map.md)
- [Bilinear form](bilinear-form.md)
- [Category theory](category-theory-split.md)
- [Coadjoint representation](coadjoint-representation.md)
- [Continuous dual space](continuous-dual-space-split.md)
- [Covector](covector.md)
- [Differentiation weights from nodal evaluations](differentiation-weights-from-nodal-evaluations.md)
- [Dual basis](dual-basis.md)
- [Dual isomorphisms induced by a nondegenerate pairing](dual-isomorphisms-induced-by-a-nondegenerate-pairing.md)
- [Dual Lie algebra representation](dual-lie-algebra-representation.md)
- [Dual space](dual-space.md)
- [Lie-Poisson bracket](lie-poisson-bracket.md)
- [Nondegenerate bilinear form](nondegenerate-bilinear-form.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/15c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-2/8b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-4/15f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-4/15g/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-17/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-3/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-58/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-2/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-4/1g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-1/9g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-14/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-5/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ib/paper-4/10g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-122/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-309/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-313/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-326/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/21f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-217/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ii/paper-4/22f/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326/3/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326/3/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/10f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-4/1f/solution.md)
- [Perfect pairing](perfect-pairing.md)
- [Poincare duality pairing](poincare-duality-pairing.md)
- [Separating subspace of an algebraic dual](separating-subspace-of-an-algebraic-dual.md)
- [Sobolev duality](sobolev-duality.md)
