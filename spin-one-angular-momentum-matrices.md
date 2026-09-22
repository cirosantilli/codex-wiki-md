# Spin-one angular momentum matrices

↑ **Parent:** [Irreducible spin representation](irreducible-spin-representation.md)

In the ordered [angular momentum eigenstate](angular-momentum-eigenstate.md) basis $(|1,1\rangle,|1,0\rangle,|1,-1\rangle)$, with positive raising coefficients,

$$
J_1=\frac\hbar{\sqrt2}\begin{pmatrix}0&1&0\\1&0&1\\0&1&0\end{pmatrix},\quad
J_2=\frac\hbar{\sqrt2}\begin{pmatrix}0&-i&0\\i&0&-i\\0&i&0\end{pmatrix},\quad
J_3=\hbar\operatorname{diag}(1,0,-1).
$$

To derive them, $[J_3,J_+]=\hbar J_+$ restricts $J_+$ to its two adjacent superdiagonal entries. Write these real entries as $A,B\geq0$. Since $J_-=J_+^\dagger$, the relation $[J_+,J_-]=2\hbar J_3$ reads $\operatorname{diag}(A^2,B^2-A^2,-B^2)=2\hbar^2\operatorname{diag}(1,0,-1)$, forcing $A=B=\sqrt2\hbar$. Adding and subtracting the [ladder operators](ladder-operator.md) gives the displayed [matrices](matrix.md). Direct multiplication verifies the [angular momentum commutation relations](angular-momentum-commutation-relations.md) and $J^2=2\hbar^2I$.

## ↑ Ancestors (7)

1. [Irreducible spin representation](irreducible-spin-representation.md)
2. [Spin](spin.md)
3. [Angular momentum operator](angular-momentum-operator-split.md)
4. [Quantum mechanics](quantum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-quantum-theory-course-of-the-university-of-oxford/2023/3/b/iii/solution.md)
- [Spin-one transverse measurement after axial precession](spin-one-transverse-measurement-after-axial-precession.md)
