# Noncommuting observables in two dimensions

↑ **Parent:** [Matrix mechanics](matrix-mechanics.md)

For two dimensionless [observables](observable.md) on a [two-level system](two-level-system.md), take

$$
A=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad B=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
$$

Both are [Hermitian matrices](hermitian-operator.md): $A$ has [eigenvalues](eigenvalue.md) $1,0$ and $B$ has [eigenvalues](eigenvalue.md) $1,-1$. Yet

$$
AB=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad BA=\begin{pmatrix}0&0\\1&0\end{pmatrix},\qquad [A,B]=\begin{pmatrix}0&1\\-1&0\end{pmatrix}\ne0.
$$

For instance, $AB|0\rangle=0$ whereas $BA|0\rangle=|1\rangle$. In $AB$, $B$ acts first. Neither product is [self-adjoint](self-adjoint-operator.md), so the product of two [observables](observable.md) is not automatically another [observable](observable.md). The [commutator](commutator.md) records this dependence on order. These operator products by themselves do not specify the outcomes of consecutive measurements; that additionally requires [measurement in quantum mechanics](quantum-measurement-split.md).

## ↑ Ancestors (6)

1. [Matrix mechanics](matrix-mechanics.md)
2. [Operator formalism](operator-formalism.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
