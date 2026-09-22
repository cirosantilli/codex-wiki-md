# Hermitian inner product

↑ **Parent:** [Hermitian form](hermitian-form.md)

A [Hermitian inner product](hermitian-inner-product.md) is a [Hermitian form](hermitian-form.md) $H$ on a [complex vector space](complex-vector-space.md) which has [positive definiteness](positive-definiteness.md): $H(v,v)>0$ for every nonzero [vector](vector.md) $v$. It is precisely a complex [inner product](inner-product-split.md). Only with this definiteness condition does

$$
\|v\|=\sqrt{H(v,v)}
$$

define a [norm](norm.md) rather than a [seminorm](seminorm.md) or an expression that may not be real. The standard [Hermitian inner product](hermitian-inner-product.md) on $\mathbb C^n$ is $H(z,w)=\sum_j z_j\overline{w_j}$; positive weights $c_j$ give $\sum_j c_jz_j\overline{w_j}$, with squared [norm](norm.md) $\sum_j c_j|z_j|^2$.[Sheldon Axler, Linear Algebra Done Right, third edition, §6.A, definitions 6.3 and 6.9 and examples 6.4](https://linear.axler.net/InnerProduct.pdf)

A [Hermitian inner product](hermitian-inner-product.md) need not have a real [matrix](matrix.md). For instance, with the linear-first coordinate convention,

$$
A=\begin{pmatrix}2&i\\-i&2\end{pmatrix},\qquad H(z,w)=z^T A\overline w,\qquad
H(z,z)=|z_1-i z_2|^2+|z_1|^2+|z_2|^2.
$$

The last expression proves [positive definiteness](positive-definiteness.md) without a lengthy calculation of [eigenvalues](eigenvalue.md). For $z=(1,i)$ it gives $6$, while for $z=(1,-i)$ it gives $2$. These unequal values expose why a silent switch to $z^*Az$ would change this particular [Hermitian inner product](hermitian-inner-product.md): with these same entries it gives $2$ at $(1,i)$. All entries must keep their roles from the [matrix of a Hermitian form](matrix-of-a-hermitian-form.md).

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) for a [Hermitian inner product](hermitian-inner-product.md) states

$$
|H(v,u)|^2\leq H(v,v)H(u,u).
$$

Equality holds exactly when $u,v$ are [linearly dependent](linear-dependence.md), including when either is zero. For a nonzero $u$, outline the proof by setting $a=H(v,u)/H(u,u)$ and $r=v-au$. Then $H(r,u)=0$, and the [Pythagorean theorem](pythagorean-theorem.md) gives

$$
H(v,v)=\frac{|H(v,u)|^2}{H(u,u)}+H(r,r).
$$

Nonnegativity proves the inequality, while [positive definiteness](positive-definiteness.md) makes equality equivalent to $r=0$. The scalar $a$ has no extra conjugate because the first argument is linear.[Axler, Linear Algebra Done Right, third edition, orthogonal decomposition 6.14 and Cauchy-Schwarz inequality 6.15](https://linear.axler.net/InnerProduct.pdf)

The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) also holds for a [positive semidefinite Hermitian form](positive-semidefinite-hermitian-form.md), but equality need not imply [linear dependence](linear-dependence.md): for $H_0(z,w)=z_1\overline{w_1}$, the independent [vectors](vector.md) $e_1$ and $e_1+e_2$ give $1=1$. Equality then describes dependence after passing to the [quotient vector space](quotient-vector-space.md) by the [radical of a Hermitian form](radical-of-a-hermitian-form.md). The [indefinite Hermitian form](indefinite-hermitian-form.md) in [Hermitian form](hermitian-form.md) shows that conjugate symmetry alone does not even guarantee the inequality.

For a worked [orthogonal projection](orthogonal-projection.md), take $H_+(z,w)=z_1\overline{w_1}+2z_2\overline{w_2}$, $u=(1,1)$ and $v=(2,0)$. Then $a=2/3$, $au=(2/3,2/3)$ and $r=(4/3,-2/3)$, with $H_+(r,u)=0$ and $4=4/3+8/3$ for the squared [norms](norm.md). The residual is perpendicular in this [Hermitian inner product](hermitian-inner-product.md) even though its ordinary real [dot product](dot-product.md) with $u$ is $2/3$. For complex $v=(1,i)$, the same [orthogonal projection](orthogonal-projection.md) uses $a=(1+2i)/3$; rotating $v$ multiplies $a$ by $e^{i\theta}$, while rotating $u$ multiplies $a$ by $e^{-i\theta}$. This combines geometric decomposition with sensitivity to the relative [complex arguments](argument-complex-analysis.md) of the multipliers.

<a id="image-analytical-illustration-weighted-orthogonal-projection-on-a-real-slice-and-opposite-changes-of-complex-argument-of-its-projection-coefficient"></a>
![](sesquilinear-hermitian-forms-projection-phase.png)

**[Figure 4](#image-analytical-illustration-weighted-orthogonal-projection-on-a-real-slice-and-opposite-changes-of-complex-argument-of-its-projection-coefficient). Analytical illustration: weighted orthogonal projection on a real slice and opposite changes of complex argument of its projection coefficient**.

A [Hermitian inner product](hermitian-inner-product.md) therefore supplies more than a positive diagonal: [orthogonality](orthogonal-vectors.md), [orthogonal projection](orthogonal-projection.md) onto a [span](linear-span.md), and the [triangle inequality](triangle-inequality.md) for its [norm](norm.md) make approximation and distance meaningful. For the [function space](function-space.md) of complex [continuous functions](continuous-function.md) on $[0,1]$, $H(f,g)=\int_0^1 f(t)\overline{g(t)}\,dt$ has [positive definiteness](positive-definiteness.md), because a nonzero [continuous function](continuous-function.md) has positive [modulus](modulus.md) on a small interval. The same construction turns overlap under [integration](integral-split.md) into lengths and best approximation in finite-dimensional [vector subspaces](vector-subspace.md).

## ↑ Ancestors (7)

1. [Hermitian form](hermitian-form.md)
2. [Sesquilinear form](sesquilinear-form.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (46)

- [Clifford multiplication](clifford-multiplication.md)
- [Cokernel compatibility equations](cokernel-compatibility-equations.md)
- [Complete reducibility of compact-group representations](complete-reducibility-of-compact-group-representations.md)
- [Conjugate-linear Hodge star](conjugate-linear-hodge-star.md)
- [Discrete L2 inner product](discrete-l2-inner-product.md)
- [Haar averaging produces invariant complements](haar-averaging-produces-invariant-complements.md)
- [Hermitian form](hermitian-form.md)
- [Hermitian inner product](hermitian-inner-product.md)
- [Inverse-adjoint representation](inverse-adjoint-representation.md)
- [Orthogonal complex line flag manifold](orthogonal-complex-line-flag-manifold.md)
- [Orthogonal projection matrix](orthogonal-projection-matrix.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-1/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-20/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-15/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ii/paper-4/19f/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-19/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/19g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-22/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-23/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-23/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-19/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-13/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-13/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-1/8b/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/ia/paper-1/8b/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-22/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-17/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-1/6a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-103/1/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-103/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-103/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-114/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-302/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-118/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-302/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-118/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-1/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2/10/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2018/paper-2/10/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2022/paper-1/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2025/paper-1/6/a/solution.md)
- [Sesquilinear form](sesquilinear-form.md)
