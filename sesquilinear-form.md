# Sesquilinear form

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Sesquilinear_form)

A [sesquilinear form](sesquilinear-form.md) on a [complex vector space](complex-vector-space.md) $V$ is a map $B:V\times V\to\mathbb C$ which, with the convention used throughout this article, is a [linear map](linear-map.md) in its first argument and a [conjugate-linear map](antilinear-map.md) in its second. For [vectors](vector.md) $u,v,w$ and [complex numbers](complex-number.md) $\alpha,\beta$, the defining identities are

$$
B(\alpha u+\beta v,w)=\alpha B(u,w)+\beta B(v,w),\qquad
B(u,\alpha v+\beta w)=\overline\alpha B(u,v)+\overline\beta B(u,w).
$$

The bars denote [complex conjugation](complex-conjugation.md). No symmetry or positivity is required. Some authors choose the opposite convention; every formula here keeps the first argument linear.[David Bindel, CS 6210: Matrix Computations, Introduction, sesquilinear forms](https://www.cs.cornell.edu/courses/cs6210/2025fa/lec/2025-08-25.html)

For a [basis](basis.md) $e_1,\ldots,e_n$ of a [finite-dimensional vector space](finite-dimensional-vector-space.md), write $u=\sum_i x_i e_i$, $v=\sum_j y_j e_j$, and $A_{ij}=B(e_i,e_j)$. Expanding by the two identities gives

$$
B(u,v)=\sum_{i,j}x_i A_{ij}\overline{y_j}=x^T A\overline y.
$$

Every complex [matrix](matrix.md) $A$ gives a [sesquilinear form](sesquilinear-form.md) this way. The superscript $T$ means [transpose](transpose.md), not [conjugate transpose](conjugate-transpose.md). Equivalently, the scalar is $y^*A^T x$, where $y^*=\overline y^{\,T}$. This is the convention used for the [matrix of a Hermitian form](matrix-of-a-hermitian-form.md) when symmetry is imposed. The coordinate formula follows directly by expanding the [basis](basis.md) coefficients.[Burke, Linear Analysis, Lecture 4, coordinate expansion for sesquilinear forms](https://sites.math.washington.edu/~burke/crs/554/lectures/b-lecture4.pdf)

For a concrete example on $\mathbb C^2$, let $B(z,w)=z_1\overline{w_2}$. Its [matrix](matrix.md) is $\begin{pmatrix}0&1\\0&0\end{pmatrix}$: $B(e_1,e_2)=1$ but $B(e_2,e_1)=0$, so it is not a [Hermitian form](hermitian-form.md). Also $B((1,i),(1,i))=-i$, so even real diagonal values cannot be assumed for an arbitrary [sesquilinear form](sesquilinear-form.md). By comparison, the [bilinear form](bilinear-form.md) $F(z,w)=z_1w_1+z_2w_2$ satisfies $F(iz,w)=F(z,iw)=iF(z,w)$ and has $F((i,0),(i,0))=-1$; it cannot supply positive squared lengths on this [complex vector space](complex-vector-space.md).

The effect of changing the [complex argument](argument-complex-analysis.md) of a multiplier is particularly revealing. For [real numbers](real-number.md) $\theta,\phi$, [sesquilinear forms](sesquilinear-form.md) satisfy

$$
B(e^{i\theta}u,e^{i\phi}v)=e^{i(\theta-\phi)}B(u,v),\qquad B(\alpha u,\alpha u)=|\alpha|^2B(u,u).
$$

Thus a common change of [complex argument](argument-complex-analysis.md) cancels from the diagonal, whereas the two arguments rotate the output in opposite directions. Conjugating one argument is what replaces the $\alpha^2$ scaling of a [bilinear form](bilinear-form.md) by the nonnegative $|\alpha|^2$ scaling needed for a [Hermitian inner product](hermitian-inner-product.md). This mechanism also works in [function spaces](function-space.md): for complex [continuous functions](continuous-function.md) on $[0,1]$, $B(f,g)=\int_0^1 f(t)\overline{g(t)}\,dt$ obeys the same identities, letting [integration](integral.md) measure overlap rather than merely multiply coefficients.

**Table of contents**

- [Orthogonal complement for a sesquilinear form](orthogonal-complement-for-a-sesquilinear-form.md)
- [Hermitian form](hermitian-form.md)
  - [Hermitian inner product](hermitian-inner-product.md)
  - [Hermitian form over a quadratic finite field](hermitian-form-over-a-quadratic-finite-field.md)
    - [Hermitian hyperbolic plane over a finite field](hermitian-hyperbolic-plane-over-a-finite-field.md)
    - [Orthonormalization of a finite-field Hermitian form](orthonormalization-of-a-finite-field-hermitian-form.md)
  - [Monomial orthonormal basis on the unit torus](monomial-orthonormal-basis-on-the-unit-torus.md)
  - [Radical of a Hermitian form](radical-of-a-hermitian-form.md)
  - [Positive semidefinite Hermitian form](positive-semidefinite-hermitian-form.md)
  - [Indefinite Hermitian form](indefinite-hermitian-form.md)
  - [Matrix of a Hermitian form](matrix-of-a-hermitian-form.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Bilinear form](bilinear-form.md)
- [Coercive bilinear form](coercive-bilinear-form.md)
- [Hermitian form](hermitian-form.md)
- [Hermitian form over a quadratic finite field](hermitian-form-over-a-quadratic-finite-field.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-2/8f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-69/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-5/1/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-4/8e/a/solution.md)
- [Sesquilinear form](sesquilinear-form.md)
- [Trace-class duality](trace-class-duality.md)
