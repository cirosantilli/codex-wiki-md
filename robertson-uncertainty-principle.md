# Robertson uncertainty principle

↑ **Parent:** [Quantum theory](quantum-theory-split.md)

The [Robertson uncertainty principle](robertson-uncertainty-principle.md) bounds the product of the [standard deviations](standard-deviation.md) of two [observables](observable.md) in the same [quantum state](quantum-state.md). For a normalized [pure state](pure-state.md) $|\psi\rangle$ and [self-adjoint operators](self-adjoint-operator.md) $A,B$, write their [expectation values](expectation-value.md) and [variances](variance-split.md) as

$$
\langle A\rangle=\langle\psi|A|\psi\rangle,\qquad (\Delta A)^2=\|(A-\langle A\rangle I)\psi\|^2=\langle A^2\rangle-\langle A\rangle^2,
$$

and similarly for $B$, where $I$ is the [identity operator](identity-operator.md). The [quantum uncertainties](quantum-uncertainty.md) $\Delta A,\Delta B$ then obey

$$
\Delta A\,\Delta B\geq\frac12|\langle[A,B]\rangle|,\qquad [A,B]=AB-BA.
$$

Here $[A,B]$ is the [commutator](commutator.md), and every [expectation value](expectation-value.md) is taken in the same $|\psi\rangle$. These [standard deviations](standard-deviation.md) describe the outcome spreads when $A$ and $B$ are measured on separate ensembles prepared in that same [quantum state](quantum-state.md). They are not instrument errors or the change caused by a preceding [measurement in quantum mechanics](quantum-measurement-split.md). The definition and bound are developed in [Barton Zwiebach, Uncertainty Principle and Compatible Observables, 2013, §§1–2](https://ocw.mit.edu/courses/8-05-quantum-physics-ii-fall-2013/005979fa741c3ea2e0430456b70caf93_MIT8_05F13_Chap_05.pdf).

For [unbounded self-adjoint operators](unbounded-self-adjoint-operator.md), the [operator domains](operator-domain.md) matter. Assume $\psi\in D(A)\cap D(B)$, so that both second moments are finite; $\langle A^2\rangle$ here means the second moment of the measured [probability distribution](probability-distribution.md), equal to $\|A\psi\|^2$, even if $A^2\psi$ is undefined. To use the displayed operator [commutator](commutator.md), also assume $\psi\in D(AB)\cap D(BA)$. Without these product-domain assumptions, the always meaningful version on $D(A)\cap D(B)$ uses $|\operatorname{Im}\langle A\psi|B\psi\rangle|$ as its right-hand side. These qualifications prevent a formal [commutator](commutator.md) identity from being applied to an inadmissible [quantum state](quantum-state.md).

The brief proof is [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) applied to $u=(A-\langle A\rangle I)\psi$ and $v=(B-\langle B\rangle I)\psi$:

$$
\Delta A\,\Delta B=\|u\|\|v\|\geq|\langle u|v\rangle|\geq|\operatorname{Im}\langle u|v\rangle|=\frac12|\langle[A,B]\rangle|.
$$

The final equality uses [self-adjointness](self-adjoint-operator.md) and the product-domain assumptions. Thus a geometric statement about [inner products](inner-product.md) becomes a constraint on experimental spreads. For nonzero $\Delta A,\Delta B$, equality requires $u,v$ to be proportional with a purely imaginary proportionality factor; the [equality case of the Heisenberg uncertainty relation](equality-case-of-the-heisenberg-uncertainty-relation.md) turns this condition into a [Gaussian wave packet](gaussian-wave-packet.md).

The bound is useful because computing a single [commutator](commutator.md) and its [expectation value](expectation-value.md) can constrain two entire outcome distributions. Its right-hand side depends on the [quantum state](quantum-state.md): the [spin uncertainty state dependence](spin-uncertainty-state-dependence.md) example gives both a positive saturated bound and a zero bound for the same noncommuting [observables](observable.md). Robertson's paper, titled "The Uncertainty Principle", appeared on 1 July 1929 in Physical Review, volume 34, starting at page 163. [H. P. Robertson, The Uncertainty Principle, 1929](https://doi.org/10.1103/PhysRev.34.163).

**Table of contents**

- [Spin uncertainty state dependence](spin-uncertainty-state-dependence.md)
- [Heisenberg uncertainty relation](heisenberg-uncertainty-relation.md)
- [Quadratic-norm proof of the Heisenberg uncertainty relation](quadratic-norm-proof-of-the-heisenberg-uncertainty-relation.md)
- [Equality case of the Heisenberg uncertainty relation](equality-case-of-the-heisenberg-uncertainty-relation.md)

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Heisenberg uncertainty relation](heisenberg-uncertainty-relation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/ib/paper-1/18a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/16b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-3/16b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ib/paper-1/4a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2020/ii/paper-1/34a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ib/paper-1/14d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/ii/paper-1/34a/a/solution.md)
- [Quantum uncertainty](quantum-uncertainty.md)
- [Robertson uncertainty principle](robertson-uncertainty-principle.md)
- [Spin uncertainty state dependence](spin-uncertainty-state-dependence.md)
