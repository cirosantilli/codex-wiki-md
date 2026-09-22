# Rayleigh quotient

↑ **Parent:** [Operator theory](linear-operator-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Rayleigh_quotient)

The [Rayleigh quotient](rayleigh-quotient.md) measures the [quadratic form](quadratic-form.md) of a [self-adjoint operator](self-adjoint-operator.md) per unit squared [norm](norm.md). For a nonzero [vector](vector.md) $x$ and a finite-dimensional [Hermitian matrix](hermitian-operator.md) $A$,

$$
R_A(x)=\frac{x^*Ax}{x^*x}.
$$

For a real [symmetric matrix](symmetric-matrix.md), replace the [conjugate transpose](conjugate-transpose.md) $x^*$ by $x^T$. More generally, for a [self-adjoint operator](self-adjoint-operator.md) $H$ on a [Hilbert space](hilbert-space-split.md), use $R_H(\psi)=\langle\psi,H\psi\rangle/\langle\psi,\psi\rangle$ for nonzero $\psi$ in its [operator domain](operator-domain.md). On an [eigenvector](eigenvector.md) it returns the exact [eigenvalue](eigenvalue.md). Multiplying the [vector](vector.md) by any nonzero [scalar](scalar.md) leaves the quotient unchanged, so it measures a direction rather than a chosen length.

For the [symmetric matrix](symmetric-matrix.md) $A=\begin{pmatrix}2&1\\1&2\end{pmatrix}$ from the [finite-dimensional spectral theorem](finite-dimensional-spectral-theorem.md) example,

$$
R_A(1,0)=2,\qquad R_A(1,1)=3,\qquad R_A(-1,1)=1.
$$

The first value is not an [eigenvalue](eigenvalue.md): it is an average of the two directional responses. To see every direction, write the unit [vector](vector.md) $q(\theta)=\cos\theta\,e_++\sin\theta\,e_-$ in the [orthonormal eigenbasis](orthonormal-eigenbasis.md). Then

$$
R_A(q(\theta))=3\cos^2\theta+\sin^2\theta=1+2\cos^2\theta.
$$

The largest value is $3$ along $e_+$; the smallest is $1$ along $e_-$. A direction halfway between them has quotient $2$. In the left panel, the color on the [unit circle](complex-unit-circle.md) represents the quotient; in the right panel, the same values are plotted against the [angle](angle.md) measured from $e_+$.

<a id="image-the-rayleigh-quotient-varies-continuously-between-two-eigenvalues-as-a-unit-vector-turns"></a>
![](rayleigh-quotient-direction.png)

**[Figure 6](#image-the-rayleigh-quotient-varies-continuously-between-two-eigenvalues-as-a-unit-vector-turns). The Rayleigh quotient varies continuously between two eigenvalues as a unit vector turns**.

The [Hermitian Rayleigh quotient range](hermitian-rayleigh-quotient-range.md) explains why this is useful: evaluating one trial [vector](vector.md) gives an upper bound on the smallest [eigenvalue](eigenvalue.md) and a lower bound on the largest one, without solving a [characteristic polynomial](characteristic-polynomial.md). At an extreme [eigenvector](eigenvector.md), a small angular error changes the quotient only quadratically. Near $e_+$ in this example, $3-R_A(q(\theta))=2\sin^2\theta=2\theta^2+O(\theta^4)$. This is the geometric reason for [quadratic Rayleigh-quotient improvement for the power method](quadratic-rayleigh-quotient-improvement-for-the-power-method.md) and motivates the [Rayleigh-Ritz method](rayleigh-ritz-method.md).

There is a concrete historical link with [normal modes](normal-mode.md). In _The Theory of Sound_ (1877), Volume I, Sections 88–89, Lord Rayleigh studies the period of a constrained trial vibration. He shows that the period has a [stationary point](stationary-point.md) at a [normal mode](normal-mode.md) and that a trial type bounds the longest natural period. These [energy](energy.md) ratios are a mechanical setting for the modern [Rayleigh quotient](rayleigh-quotient.md) and [generalized Rayleigh quotient](generalized-rayleigh-quotient.md); the book describes the result through vibration periods, rather than today's matrix notation.[Rayleigh, The Theory of Sound, Volume I, 1877, Sections 88–89, printed pp. 84–87](https://archive.org/details/theorysound06raylgoog)

**Table of contents**

- [Rayleigh quotient with one Neumann endpoint](rayleigh-quotient-with-one-neumann-endpoint.md)
- [Hermitian Rayleigh quotient range](hermitian-rayleigh-quotient-range.md)
- [Stationary directions of the Rayleigh quotient](stationary-directions-of-the-rayleigh-quotient.md)
- [Odd variational trial gives an excited oscillator bound](odd-variational-trial-gives-an-excited-oscillator-bound.md)
- [Generalized Rayleigh quotient](generalized-rayleigh-quotient.md)
- [Rayleigh quotient iteration](rayleigh-quotient-iteration.md)
  - [Local cubic convergence of Rayleigh quotient iteration](local-cubic-convergence-of-rayleigh-quotient-iteration.md)
- [Rayleigh-Ritz variational principle](rayleigh-ritz-variational-principle.md)
  - [Odd-state variational principle for an even potential](odd-state-variational-principle-for-an-even-potential.md)
  - [Gaussian variational bound for an attractive Gaussian well](gaussian-variational-bound-for-an-attractive-gaussian-well.md)
  - [Finite-subspace variational method](finite-subspace-variational-method.md)
    - [Two-mode variational bound for a linearly tilted square well](two-mode-variational-bound-for-a-linearly-tilted-square-well.md)

## ↑ Ancestors (6)

1. [Operator theory](linear-operator-theory-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (71)

- [Canonical discriminant directions](canonical-discriminant-directions.md)
- [Completely positive optimization](completely-positive-optimization.md)
- [Copositive optimization](copositive-optimization.md)
- [Cowling energy principle for a rotating barotropic star](cowling-energy-principle-for-a-rotating-barotropic-star.md)
- [Elastic normal-mode energy identity](elastic-normal-mode-energy-identity.md)
- [Exact two-dimensional power iteration](exact-two-dimensional-power-iteration.md)
- [Exact variational solution in a two-level system](exact-variational-solution-in-a-two-level-system.md)
- [Global variational form of the Michael criterion](global-variational-form-of-the-michael-criterion.md)
- [Hermitian quadratic form](hermitian-quadratic-form.md)
- [Hermitian Rayleigh quotient range](hermitian-rayleigh-quotient-range.md)
- [Largest-eigenvalue interlacing for a principal submatrix](largest-eigenvalue-interlacing-for-a-principal-submatrix.md)
- [Local cubic convergence of Rayleigh quotient iteration](local-cubic-convergence-of-rayleigh-quotient-iteration.md)
- [Magnetic buoyancy energy criterion](magnetic-buoyancy-energy-criterion.md)
- [Magnetohydrodynamic energy principle](magnetohydrodynamic-energy-principle.md)
- [Odd variational trial gives an excited oscillator bound](odd-variational-trial-gives-an-excited-oscillator-bound.md)
- [Optimal energy amplification of a linear system](optimal-energy-amplification-of-a-linear-system.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-54/2/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-43/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-72/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-72/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-76/5/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ii/paper-2/33b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-71/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-46/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-47/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-3/15d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-69/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ia/paper-1/7a/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/34d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-59/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-67/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-36/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-54/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-63/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ii/paper-1/32a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-58/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-1/6b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-107/6/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/16d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-314/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-339/1/h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ia/paper-1/7b/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-331/4/a/v/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-2/34b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/41e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-205/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ii/paper-3/40c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-2/36d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/40c/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-216/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218/6/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-218/6/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-333/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-333/3/f/solution.md)
- [Power iteration eigenpair diagnostics](power-iteration-eigenpair-diagnostics.md)
- [Power iteration failure cases](power-iteration-failure-cases.md)
- [Quadratic Rayleigh-quotient improvement for the power method](quadratic-rayleigh-quotient-improvement-for-the-power-method.md)
- [Quantum variational principle](quantum-variational-principle.md)
- [Radial stellar pulsation equation](radial-stellar-pulsation-equation.md)
- [Rank-one eigenprojector perturbation bound](rank-one-eigenprojector-perturbation-bound.md)
- [Rayleigh quotient](rayleigh-quotient.md)
- [Stellar displacement energy identity](stellar-displacement-energy-identity.md)
- [Sturm-Liouville operator](sturm-liouville-operator.md)
- [Transverse energy instability of nonconstant temperature rolls](transverse-energy-instability-of-nonconstant-temperature-rolls.md)
- [Variational method](variational-method.md)
- [Witness acceptance operator](witness-acceptance-operator.md)
