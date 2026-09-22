# Hermitian conjugation

↑ **Parent:** [Adjoint operator](adjoint-operator.md)

Hermitian conjugation is the operation of taking the [adjoint operator](adjoint-operator.md), written $T^\dagger=T^*$. For a [matrix](matrix.md) in [orthonormal bases](orthonormal-basis.md), it takes the [complex conjugate](complex-conjugate.md) of each entry and exchanges rows with columns:

$$
(A^\dagger)_{jk}=\overline{A_{kj}},\qquad A^\dagger=\overline A^{\mathrm T}.
$$

For a real [matrix](matrix.md) it is the ordinary [transpose](transpose.md). For the complex [matrix](matrix.md) $T$ in the [adjoint operator](adjoint-operator.md) example, its second row $(2,1-i)$ becomes the second column $(2,1+i)^{\mathrm T}$ of $T^\dagger$. This is the same [conjugate transpose](conjugate-transpose.md) used in MIT's treatment of complex [inner products](inner-product.md) and [Hermitian matrices](hermitian-operator.md).[Strang, MIT 18.06SC, lecture 26 summary, Complex matrices, pp. 1–2, 2011](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/53f17d47bf99d26fdc472b3177c256a8_MIT18_06SCF11_Ses3.2sum.pdf)

For [bounded operators](continuous-linear-operator.md) with matching source and target [Hilbert spaces](hilbert-space-split.md), [Hermitian conjugation](hermitian-conjugation.md) satisfies

$$
(A+B)^\dagger=A^\dagger+B^\dagger,\quad (\alpha A)^\dagger=\overline\alpha A^\dagger,\quad (BA)^\dagger=A^\dagger B^\dagger,\quad (A^\dagger)^\dagger=A.
$$

The reversal of [function composition](function-composition.md) is forced by moving both [linear operators](linear-operator.md) across an [inner product](inner-product.md):

$$
\langle BAx,y\rangle=\langle Ax,B^\dagger y\rangle=\langle x,A^\dagger B^\dagger y\rangle.
$$

The calculation identifies the [adjoint operator](adjoint-operator.md) by the uniqueness theorem in Melrose's MIT notes.[Melrose, MIT 18.102, Functional Analysis, Chapter 3, §11, 2020](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/3d4cc88026d44a01f936cd6a0aa995cb_MIT18_102s20_lec_FA.pdf)

For a computed order check, let $S=\begin{pmatrix}0&1\\1&0\end{pmatrix}$ and reuse $T=\begin{pmatrix}1&i\\2&1-i\end{pmatrix}$. Then

$$
(ST)^\dagger=T^\dagger S=\begin{pmatrix}2&1\\1+i&-i\end{pmatrix},\qquad ST^\dagger=\begin{pmatrix}-i&1+i\\1&2\end{pmatrix}.
$$

Keeping the original order gives a different [matrix](matrix.md). Likewise $(iT)^\dagger=-iT^\dagger$: taking the [adjoint operator](adjoint-operator.md) is conjugate-linear as an operation on [linear operators](linear-operator.md), although each individual $T^\dagger$ is a [linear map](linear-map.md) on [vectors](vector.md).

## ↑ Ancestors (8)

1. [Adjoint operator](adjoint-operator.md)
2. [Riesz representation theorem](riesz-representation-theorem.md)
3. [Hilbert space](hilbert-space-split.md)
4. [Functional analysis](functional-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Hermitian conjugation](hermitian-conjugation.md)
- [Intrinsic charge-conjugation phase](intrinsic-charge-conjugation-phase.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-301/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-301/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-305/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-305/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-307/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-312/1/i/solution.md)
