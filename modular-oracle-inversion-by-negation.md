# Modular-oracle inversion by negation

↑ **Parent:** [Modular-addition quantum oracle](modular-addition-quantum-oracle.md)

Let $S_M|y\rangle=|-y\bmod M\rangle$. The [modular-addition quantum oracle](modular-addition-quantum-oracle.md) obeys

$$
U_h^{-1}=(I\otimes S_M)U_h(I\otimes S_M).
$$

The three steps replace $y$ by $-y$, then $-y+h(x)$, then $y-h(x)$. Thus a query to the inverse costs one forward query and two known [unitary operators](unitary-operator.md). The negation operator is a [permutation matrix](permutation-matrix.md) with $S_M^2=I$.

## ↑ Ancestors (5)

1. [Modular-addition quantum oracle](modular-addition-quantum-oracle.md)
2. [Quantum theory](quantum-theory-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/2/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-324/2/b/iii/solution.md)
- [Permutation-preimage quantum search](permutation-preimage-quantum-search.md)
