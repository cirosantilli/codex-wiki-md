<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Promote the [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md) coefficients to [annihilation operators](../../../../annihilation-operator.md) and [creation operators](../../../../creation-operator.md), replacing $a^*$ by $a^\dagger$. The [canonical commutation relations](../../../../canonical-commutation-relation.md) are

$$
\boxed{[a_{\mathbf p},a_{\mathbf q}^\dagger]=(2\pi)^3\delta^3(\mathbf p-\mathbf q),\qquad
[a_{\mathbf p},a_{\mathbf q}]=[a_{\mathbf p}^\dagger,a_{\mathbf q}^\dagger]=0.}
$$

Together with the normalization in part a, they give $[\phi(t,\mathbf x),\pi(t,\mathbf y)]=i\delta^3(\mathbf x-\mathbf y)$ and vanishing equal-time [commutators](../../../../commutator.md) between two [fields](../../../../field.md) or two [conjugate momenta](../../../../canonical-momentum.md).

Insert the [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md) in the [Hamiltonian](../../../../hamiltonian.md). The spatial integral produces $(2\pi)^3\delta^3(\mathbf p\pm\mathbf q)$. The $aa$ and $a^\dagger a^\dagger$ coefficients cancel because $\omega_{\mathbf p}^2=\mathbf p^2+m^2$. The remaining terms give

$$
H=\frac12\int\frac{d^3p}{(2\pi)^3}\omega_{\mathbf p}
\left(a_{\mathbf p}^\dagger a_{\mathbf p}+a_{\mathbf p}a_{\mathbf p}^\dagger\right)
=\int\frac{d^3p}{(2\pi)^3}\omega_{\mathbf p}a_{\mathbf p}^\dagger a_{\mathbf p}
+\frac{(2\pi)^3\delta^3(0)}2\int\frac{d^3p}{(2\pi)^3}\omega_{\mathbf p}.
$$

This is a continuum of [quantum harmonic oscillators](../../../../quantum-harmonic-oscillator-split.md). In a finite periodic volume $V$, $(2\pi)^3\delta^3(0)=V$. The [Fock vacuum](../../../../fock-vacuum.md) satisfies $a_{\mathbf p}|0\rangle=0$, so its [vacuum energy density](../../../../vacuum-energy-density.md) is

$$
\boxed{\mathcal E=\frac{\langle0|H|0\rangle}{V}=\frac12\int\frac{d^3p}{(2\pi)^3}\sqrt{\mathbf p^2+m^2}.}
$$

[Normal ordering](../../../../normal-ordering.md) would subtract this constant; here it must be retained because it is the quantity being calculated.[Section 2, canonical quantization of the real scalar field and its zero-point Hamiltonian](../../../../quantum-field-theory-by-david-tong.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
