# Gershgorin exclusion for a matrix-pencil parameter

↑ **Parent:** [Gershgorin circle theorem](gershgorin-circle-theorem.md)

To exclude zero as an [eigenvalue](eigenvalue.md) of $A+sB$, it is enough that every row has positive real diagonal entry exceeding the sum of the absolute values of its off-diagonal entries. All [Gershgorin discs](gershgorin-disc.md) then lie strictly in the right half-plane. For

$$
A=\begin{pmatrix}2&-2&0\\-3&5&0\\1&2&3\end{pmatrix},\qquad B=\begin{pmatrix}2&0&0\\0&2&1\\0&1&2\end{pmatrix},
$$

the three diagonal-dominance margins of $A+sB$ are $2s,2+s,s$, all positive for $s>0$. Thus $A-\mu B$ is nonsingular for negative real $\mu$. Working with the pencil directly avoids computing either a [determinant](determinant.md) [polynomial](polynomial-split.md) or $B^{-1}A$.

## ↑ Ancestors (6)

1. [Gershgorin circle theorem](gershgorin-circle-theorem.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
