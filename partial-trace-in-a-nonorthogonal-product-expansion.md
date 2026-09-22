# Partial trace in a nonorthogonal product expansion

↑ **Parent:** [Partial trace](partial-trace.md)

The vectors need not form [orthonormal bases](orthonormal-basis.md). With the [inner product](inner-product-split.md) linear in its second entry, expand the rank-one operator $|\Psi\rangle\langle\Psi|$ and take the trace on the second factor. This gives the displayed reduced positive operator. For every [observable](observable.md) $A$ on the first factor,

$$
\langle\Psi,(A\otimes I)\Psi\rangle=\operatorname{Tr}(AS_1),\qquad\operatorname{Tr}S_1=\|\Psi\|^2.
$$

Positivity also follows directly from $\langle v,S_1v\rangle=\|\sum_j\langle v,\xi_j\rangle\eta_j\|^2$. Thus the physical [density operator](density-matrix-split.md) is $S_1/\|\Psi\|^2$ when the nonzero source vector is not normalized. The [Gram matrix](gram-matrix.md) of the second-factor vectors supplies the cross coefficients; replacing those coefficients by Kronecker deltas without checking [orthonormality](orthonormal-set.md) changes the subsystem state. This formula is useful when an efficient product expansion uses nonorthogonal vectors, even though the [partial trace](partial-trace.md) itself is basis-independent.

## ↑ Ancestors (5)

1. [Partial trace](partial-trace.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
