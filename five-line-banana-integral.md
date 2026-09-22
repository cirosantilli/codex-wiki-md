# Five-line banana integral

↑ **Parent:** [Feynman integral](feynman-integral.md)

The [two-point function](two-point-correlation-function.md) [Feynman integral](feynman-integral.md) with two [interaction vertices](interaction-vertex.md) joined by five parallel [scalar propagators](scalar-propagator.md) has four independent [loop momenta](loop-momentum.md):

$$
B_5(p)=\int\prod_{j=1}^4\frac{d^dk_j}{(2\pi)^d}
\frac1{\prod_{j=1}^4(k_j^2+m^2)\,[(p-\sum_jk_j)^2+m^2]}.
$$

This formula uses Euclidean [momenta](momentum-split.md). In three dimensions the [convolution theorem](convolution-theorem.md) and $G(x)=e^{-m|x|}/(4\pi|x|)$ give

$$
B_5(p)=\frac1{256\pi^4}\int_0^\infty\rho^{-3}e^{-5m\rho}\frac{\sin(|p|\rho)}{|p|\rho}\,d\rho,
$$

with [cutoff regularization](cutoff-regularization.md) required at $\rho=0$. With a lower radial cutoff $a$, the coefficient of $p^2$ has [ultraviolet divergence](ultraviolet-divergence.md) $-\log(1/(ma))/(1536\pi^4)$. It therefore generates a divergent [wave-function renormalization](wave-function-renormalization.md) in three-dimensional sextic [scalar field theory](scalar-field-theory-split.md). By contrast the three-line [sunset diagram](sunset-diagram.md) has only a momentum-independent logarithmic [ultraviolet divergence](ultraviolet-divergence.md) in three dimensions. This illustrates why a [superficial degree of divergence](superficial-degree-of-divergence.md) of two allows both a [mass counterterm](mass-counterterm.md) and a kinetic [counterterm](counterterm.md), while degree zero allows only the former in a [two-point function](two-point-correlation-function.md).

## ↑ Ancestors (7)

1. [Feynman integral](feynman-integral.md)
2. [Feynman diagram](feynman-diagram.md)
3. [Perturbative quantum field theory](perturbative-quantum-field-theory-split.md)
4. [Quantum field theory](quantum-field-theory-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-quantum-field-theory-course-of-the-university-of-oxford/2021/3/c/ii/solution.md)
- [Solution](past-exam-of-the-quantum-field-theory-course-of-the-university-of-oxford/2021/3/d/solution.md)
