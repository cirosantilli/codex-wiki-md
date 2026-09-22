# Exterior algebra

↑ **Parent:** [Multilinear algebra](multilinear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Exterior_algebra)

The [exterior algebra](exterior-algebra.md) of a [vector space](vector-space-split.md) $V$ combines [scalars](scalar.md), [vectors](vector.md), and higher-dimensional oriented elements in one [graded algebra](graded-algebra.md). In a finite-dimensional [vector space](vector-space-split.md) it is

$$
\Lambda^\bullet V=\bigoplus_{k=0}^{\dim V}\Lambda^kV
$$

with multiplication given by the [exterior product](exterior-product.md). Degree zero is the scalar [field](field.md), degree one is $V$, and degree two is the space of [bivectors](bivector.md). Multiplication adds degrees: combining two [vectors](vector.md) produces a [bivector](bivector.md), rather than another ordinary [vector](vector.md).[Exterior Powers, §10: exterior algebra and its grading](exterior-powers-by-keith-conrad.md)

The essential rule is **$v\wedge v=0$**. Repeating the same direction cannot produce a nonzero oriented area. [Bilinearity](bilinearity.md) then gives $u\wedge v=-v\wedge u$: expand $(u+v)\wedge(u+v)=0$ and remove the two zero self-products. The alternating rule remains part of the definition in [characteristic two](characteristic-two.md), where sign reversal alone would not force a self-product to vanish.

If $V=\mathbb R^2$ with [standard basis](standard-basis.md) $e_1,e_2$, every element of its [exterior algebra](exterior-algebra.md) has the form

$$
a+be_1+ce_2+d(e_1\wedge e_2).
$$

There are four independent [coefficients](coefficient.md): one scalar, two vector components, and one area component. In $\mathbb R^3$, the respective degree dimensions are $1,3,3,1$, giving eight components in total. More generally, the [exterior power](exterior-power.md) basis gives total [dimension](dimension-vector-space.md) $\sum_{k=0}^n\binom nk=2^n$.

This language is useful when direction and orientation matter together. [Determinants](determinant.md) measure the action on top-degree [exterior powers](exterior-power.md); [differential forms](differential-form-split.md) use exterior powers of a [dual space](dual-space-split.md) to describe quantities integrated along paths, surfaces, and higher-dimensional regions. The [Grassmann algebra](grassmann-algebra.md) viewpoint also makes the sign changes in anticommuting generators systematic. A single multiplication rule connects geometry and algebra.

**Table of contents**

- [Bivector](bivector.md)
  - [Simple bivector](simple-bivector.md)
- [Exterior product](exterior-product.md)
- [Polynomial polyvector field](polynomial-polyvector-field.md)
  - [Schouten-Nijenhuis bracket](schouten-nijenhuis-bracket.md)
- [Grassmann algebra](grassmann-algebra.md)
  - [Grassmann parity](grassmann-parity.md)
  - [Grassmann derivative](grassmann-derivative.md)
  - [Left Grassmann derivative](left-grassmann-derivative.md)
  - [Grassmann variable](grassmann-variable.md)
- [Exterior power](exterior-power.md)
  - [Exterior square](exterior-square.md)
    - [Exterior square of a direct sum](exterior-square-of-a-direct-sum.md)
    - [Symplectic contraction of an exterior square](symplectic-contraction-of-an-exterior-square.md)
      - [Primitive exterior square](primitive-exterior-square.md)

## ↑ Ancestors (6)

1. [Multilinear algebra](multilinear-algebra-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (24)

- [Cartan's magic formula](cartan-s-magic-formula.md)
- [Cohomology ring of a torus](cohomology-ring-of-a-torus.md)
- [Exterior algebra](exterior-algebra.md)
- [Exterior multiplication](exterior-multiplication.md)
- [Exterior-power Lie algebra representation](exterior-power-lie-algebra-representation.md)
- [Gerstenhaber algebra](gerstenhaber-algebra.md)
- [Getzler rescaling](getzler-rescaling.md)
- [Graded commutative algebra](graded-commutative-algebra.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-24/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-24/6/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-20/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-10/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-65/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-7/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-17/2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-15/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-19/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-127/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-313/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-313/3/b/solution.md)
- [Uniqueness of the exterior derivative from its axioms](uniqueness-of-the-exterior-derivative-from-its-axioms.md)
