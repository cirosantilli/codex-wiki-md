<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [positive holomorphic line bundle](../../../../../../positive-holomorphic-line-bundle.md) $F$ admits a [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) whose [Chern connection](../../../../../../chern-connection.md) curvature satisfies that $iF_F$ is a [positive real (1, 1)-form](../../../../../../positive-real-1-1-form.md). In a local [holomorphic local frame](../../../../../../holomorphic-local-trivialization.md) with squared length $e^{-\varphi}$, the [local formula for the Chern connection on a line bundle](../../../../../../local-formula-for-the-chern-connection-on-a-line-bundle.md) gives $F_F=\partial\bar\partial\varphi$, so positivity means $i\partial\bar\partial\varphi$ is positive definite. Its closedness makes $\omega=iF_F$ a [Kähler form](../../../../../../kahler-form.md); use this form to define the operators below.

Let $n=\dim_{\mathbb C}X>0$, choose a [Hermitian metric](../../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) on $E$, and equip $G_m=E\otimes F^{-m}$ with the tensor-product metric. The [curvature of a tensor product connection](../../../../../../curvature-of-a-tensor-product-connection.md) gives

$$
iF_{G_m}=iF_E-m\omega\operatorname{id}_E.
$$

On $G_m$-valued zero-forms, the [Lefschetz commutator](../../../../../../lefschetz-commutator.md) is $[L,\Lambda]=-n\operatorname{id}$. Thus the [Bochner-Kodaira-Nakano identity](../../../../../../bochner-kodaira-nakano-identity.md) gives

$$
\Delta''_{G_m}=\Delta'_{G_m}+R_E+mn\operatorname{id},
\qquad R_E=[iF_E,\Lambda]\big|_{\mathcal A^{0,0}(E)}.
$$

This last operator is a fixed smooth self-adjoint bundle endomorphism. Compactness supplies a finite $C$ such that $\langle R_Ev,v\rangle\geq-C\|v\|^2$ at every point. For a [holomorphic section](../../../../../../holomorphic-section.md) $s$ of $G_m$, $D''s=0$ and $D''^*s=0$ by degree, so integrating the identity gives

$$
0=\|D's\|^2+\langle R_Es,s\rangle+mn\|s\|^2
\geq(mn-C)\|s\|^2.
$$

Choose an integer $m_0$ with $m_0n>C$. Then **$\boxed{H^0(X,E\otimes F^{-m})=0\quad(m\geq m_0)}$**. The threshold depends on the fixed bundle $E$, as the curvature bound makes explicit. Positive complex dimension is necessary: on a zero-dimensional manifold positivity is vacuous and a nonzero fibre has nonzero sections for every twist.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
