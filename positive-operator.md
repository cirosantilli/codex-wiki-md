# Positive operator

↑ **Parent:** [Hermitian operator](hermitian-operator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Positive_operator)

A bounded [Hermitian operator](hermitian-operator.md) $T$ on a [Hilbert space](hilbert-space-split.md) is positive, also called a [positive semidefinite operator](positive-operator.md), when

$$
q_T(x)=\langle Tx,x\rangle\geq0\qquad\text{for every }x\in H.
$$

The value must be real as well as nonnegative. This permits zero values on nonzero [vectors](vector.md): the zero [linear operator](linear-operator.md) is positive. For a bounded [Hermitian operator](hermitian-operator.md), positivity is equivalent to its [spectrum](spectrum-functional-analysis.md) being contained in $[0,\infty)$; in finite [dimension](dimension-vector-space.md), this is the condition that all [eigenvalues](eigenvalue.md) are nonnegative.[Rodriguez, notes by Andrew Lin, MIT 18.102, lecture 21, Corollary 225, 2021](https://ocw.mit.edu/courses/18-102-introduction-to-functional-analysis-spring-2021/345c4a5141559a4069aeb3105acd8ef3_MIT18_102s21_lec21.pdf)

The [Hermitian operator](hermitian-operator.md) diagram separates three cases. $D=\operatorname{diag}(1,-1)$ is [self-adjoint](self-adjoint-operator.md) but not positive, because $q_D((0,1)^{\mathrm T})=-1$. The [orthogonal projection](orthogonal-projection.md) $P=\operatorname{diag}(1,0)$ is positive semidefinite, with $q_P(x)=|x_1|^2$, but is not strictly positive on every nonzero [vector](vector.md). The complex [Hermitian matrix](hermitian-operator.md) $H=\begin{pmatrix}2&i\\-i&2\end{pmatrix}$ is positive definite because $q_H(ae_1+be_3)=|a|^2+3|b|^2>0$ whenever $(a,b)\ne(0,0)$. For real [symmetric matrices](symmetric-matrix.md), MIT's lecture 27 relates these tests to the geometry of [quadratic forms](quadratic-form-split.md) and their minima.[Strang, MIT 18.06SC, lecture 27 summary, Positive definite matrices and minima, pp. 1–2, 2011](https://ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/d163e012754258d3b374548504d8a18a_MIT18_06SCF11_Ses3.3sum.pdf)

A fundamental source of [positive operators](positive-operator.md) is $T^*T$ for a [bounded linear operator](continuous-linear-operator.md) $T:H\to K$:

$$
(T^*T)^*=T^*T,\qquad \langle T^*Tx,x\rangle=\langle Tx,Tx\rangle=\|Tx\|^2\geq0.
$$

For the complex [matrix](matrix.md) $T=\begin{pmatrix}1&i\\2&1-i\end{pmatrix}$ used above,

$$
T^*T=\begin{pmatrix}5&2-i\\2+i&3\end{pmatrix},\qquad q_{T^*T}(x)=|x_1+ix_2|^2+|2x_1+(1-i)x_2|^2.
$$

Its [eigenvalues](eigenvalue.md) are $4-\sqrt6$ and $4+\sqrt6$, both positive. Positivity organizes the squared error minimized by a [least-squares solution](least-squares-solution-of-a-linear-inverse-problem.md): the same $T^*T$ occurs in the [normal equation for a linear inverse problem](normal-equation-for-a-linear-inverse-problem.md). The [positive square root of an operator](positive-square-root-of-an-operator.md) gives the converse squared-length description, $q_T(x)=\|T^{1/2}x\|^2$ for every bounded [positive operator](positive-operator.md) $T$.

On a real [Hilbert space](hilbert-space-split.md), nonnegativity of $\langle Tx,x\rangle$ alone does not imply [self-adjointness](self-adjoint-operator.md), so the [Hermitian operator](hermitian-operator.md) hypothesis is part of the definition. On a complex [Hilbert space](hilbert-space-split.md), real-valuedness of all these expressions already forces [self-adjointness](self-adjoint-operator.md) by the [polarization identity](polarization-identity.md).

Strict positivity and a uniform positive lower bound also differ in infinite [dimension](dimension-vector-space.md). On the [l2 sequence space](l2-sequence-space.md), the bounded [Hermitian operator](hermitian-operator.md) $(Tx)_n=x_n/n$ satisfies

$$
q_T(x)=\sum_{n=1}^{\infty}\frac{|x_n|^2}{n}>0\quad(x\ne0),\qquad q_T(e_n)=\frac1n\longrightarrow0.
$$

Consequently no $\gamma>0$ satisfies $q_T(x)\geq\gamma\|x\|^2$ for every $x$. Compare the [positive definite symmetric operator](positive-definite-symmetric-operator.md) and [uniformly positive definite symmetric operator](uniformly-positive-definite-symmetric-operator.md) conditions.

**Table of contents**

- [Positive definite symmetric operator](positive-definite-symmetric-operator.md)
  - [Quadratic variational principle for a symmetric positive operator](quadratic-variational-principle-for-a-symmetric-positive-operator.md)
    - [Symmetric part determines a real quadratic functional](symmetric-part-determines-a-real-quadratic-functional.md)
  - [Uniformly positive definite symmetric operator](uniformly-positive-definite-symmetric-operator.md)
- [Positive contraction](positive-contraction.md)
- [Support of a positive operator](support-of-a-positive-operator.md)
- [Positive square root of an operator](positive-square-root-of-an-operator.md)

## ↑ Ancestors (9)

1. [Hermitian operator](hermitian-operator.md)
2. [Adjoint operator](adjoint-operator.md)
3. [Riesz representation theorem](riesz-representation-theorem.md)
4. [Hilbert space](hilbert-space-split.md)
5. [Functional analysis](functional-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (37)

- [Expectation value](expectation-value.md)
- [Filtering preserves existing frustration freeness](filtering-preserves-existing-frustration-freeness.md)
- [Frustration freeness](frustration-freeness.md)
- [Hermitian operator](hermitian-operator.md)
- [Kitaev geometrical lemma](kitaev-geometrical-lemma.md)
- [Modular operator](modular-operator.md)
- [Negative part of a Hermitian operator](negative-part-of-a-hermitian-operator.md)
- [Partial trace positivity from product vectors](partial-trace-positivity-from-product-vectors.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-47/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-58/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-33/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1/7/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-1/8/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-66/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-335/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326/2/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-335/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-225/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-225/1/a/iii/solution.md)
- [Positive contraction](positive-contraction.md)
- [Positive operator](positive-operator.md)
- [Positive operator-valued measure](positive-operator-valued-measure.md)
- [Positive part of a Hermitian operator](positive-part-of-a-hermitian-operator.md)
- [Positive square root of an operator](positive-square-root-of-an-operator.md)
- [Measurement in quantum mechanics](quantum-measurement-split.md)
- [Separable positive operator](separable-positive-operator.md)
- [Smallest angle between two subspaces](smallest-angle-between-two-subspaces.md)
- [Support of a positive operator](support-of-a-positive-operator.md)
- [Time reversal operator](time-reversal-operator.md)
- [Unitary invariance of trace distance and fidelity](unitary-invariance-of-trace-distance-and-fidelity.md)
- [Variational characterization of trace distance](variational-characterization-of-trace-distance.md)
