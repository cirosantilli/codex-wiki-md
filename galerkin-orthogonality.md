# Galerkin orthogonality

↑ **Parent:** [Finite element method](finite-element-method-split.md)

Let $V_h\subset V$ be a [conforming finite element space](conforming-finite-element-space.md). Suppose the exact solution satisfies $a(u,v)=\ell(v)$ for every $v\in V$ and its [Galerkin method](galerkin-method.md) approximation satisfies $a(u_h,v_h)=\ell(v_h)$ for every $v_h\in V_h$, using the same [bilinear form](bilinear-form-split.md) and [linear functional](linear-functional.md). Subtracting the two identities gives [Galerkin orthogonality](galerkin-orthogonality.md):

$$
a(u-u_h,v_h)=0\qquad(v_h\in V_h).
$$

This identity itself does not require symmetry. Its interpretation as an [orthogonal projection](orthogonal-projection.md) in an [energy norm](energy-norm.md) does require a bounded symmetric [coercive bilinear form](coercive-bilinear-form.md): then $a$ is an [inner product](inner-product-split.md), $e=u-u_h$ is perpendicular to every available discrete correction, and

$$
\|u-v_h\|_a^2=\|u-u_h\|_a^2+\|u_h-v_h\|_a^2\qquad(v_h\in V_h).
$$

Consequently $u_h$ is the unique closest point in $V_h$ in the [energy norm](energy-norm.md). This [Pythagorean theorem](pythagorean-theorem.md) in a function space explains the beauty of the [Galerkin method](galerkin-method.md): integrated local equations compute a global best approximation. The [Céa lemma](cea-s-lemma.md) supplies the corresponding estimate in a chosen reference norm.

For the [finite element solution of the one-dimensional Poisson equation](finite-element-solution-of-the-one-dimensional-poisson-equation.md), $a(w,v)=\int_0^1w'v'\,dx$ and $\|w\|_a=\|w'\|_{L^2(0,1)}$. Testing the error against the $i$th [piecewise-linear hat function](piecewise-linear-hat-function.md) on a uniform [mesh](finite-element-mesh.md) gives

$$
\frac1h\int_{x_{i-1}}^{x_i}e'\,dx
-\frac1h\int_{x_i}^{x_{i+1}}e'\,dx=0.
$$

In this model $e$ vanishes at every node, so each of these [integrals](integral-split.md) is individually zero, although $e$ is positive inside every element. [Galerkin orthogonality](galerkin-orthogonality.md) controls the derivative-weighted balance; it does not say that the pointwise error vanishes.

The exact identity assumes conformity and exact evaluation of the continuous forms, including any [numerical integration](numerical-integration-split.md) that is used. If assembly instead uses $a_h$ and $\ell_h$, subtraction gives the consistency defect

$$
a(u-u_h,v_h)=(\ell-\ell_h)(v_h)+(a_h-a)(u_h,v_h).
$$

Thus inexact [numerical integration](numerical-integration-split.md) need not preserve the projection. In the [Petrov-Galerkin method](petrov-galerkin-method.md) the error is tested against a different test space, and for a nonsymmetric [bilinear form](bilinear-form-split.md) the displayed identity need not describe perpendicularity in any [energy norm](energy-norm.md).

**Table of contents**

- [Céa's lemma](cea-s-lemma.md)
  - [Aubin–Nitsche duality argument](aubin-nitsche-duality-argument.md)

## ↑ Ancestors (6)

1. [Finite element method](finite-element-method-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Aubin–Nitsche duality argument](aubin-nitsche-duality-argument.md)
- [Céa's lemma](cea-s-lemma.md)
- [Conforming finite element space](conforming-finite-element-space.md)
- [Finite element mesh](finite-element-mesh.md)
- [Finite element method](finite-element-method-split.md)
- [Finite element solution of the one-dimensional Poisson equation](finite-element-solution-of-the-one-dimensional-poisson-equation.md)
- [Galerkin orthogonality](galerkin-orthogonality.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/5/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-341/7/solution.md)
- [Petrov-Galerkin method](petrov-galerkin-method.md)
- [Ritz-Galerkin equivalence for a symmetric coercive form](ritz-galerkin-equivalence-for-a-symmetric-coercive-form.md)
