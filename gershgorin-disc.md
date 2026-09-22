# Gershgorin disc

↑ **Parent:** [Gershgorin circle theorem](gershgorin-circle-theorem.md)

A row [Gershgorin disc](gershgorin-disc.md) of a [square matrix](square-matrix.md) $A=(a_{ij})$ is the closed [disk](disk-mathematics.md) in the [complex plane](complex-plane.md) with centre $a_{ii}$ and radius $r_i=\sum_{j\ne i}|a_{ij}|$. A zero radius gives a single point. The [Gershgorin disc theorem](gershgorin-circle-theorem.md) places every [eigenvalue](eigenvalue.md) in the union of these [disks](disk-mathematics.md). For a [Hermitian matrix](hermitian-operator.md), the real [intervals](interval-mathematics.md) cut out by the [Gershgorin discs](gershgorin-disc.md) bound the [eigenvalues](eigenvalue.md), including [energy](energy.md) levels when the [matrix](matrix.md) represents a [Hamiltonian operator](hamiltonian-quantum-mechanics.md).

Applying the [Gershgorin circle theorem](gershgorin-circle-theorem.md) to the [transpose](transpose.md) $A^T$ gives column [Gershgorin discs](gershgorin-disc.md) with the same centres and radii $c_i=\sum_{j\ne i}|a_{ji}|$. Since $A$ and $A^T$ have the same [characteristic polynomial](characteristic-polynomial.md), every [eigenvalue](eigenvalue.md) lies in the intersection of the row-disc union and the column-disc union. This is an intersection of two unions; one cannot generally replace each row radius by $\min(r_i,c_i)$. An isolated row [Gershgorin disc](gershgorin-disc.md) contains exactly one [eigenvalue](eigenvalue.md) by [Gershgorin eigenvalue counting](gershgorin-eigenvalue-counting.md).[Marshall Hampton, Introduction to Numerical Methods, Eigenstuff: Gershgorin circle theorem](https://www.d.umn.edu/~mhampton/NA/Eigenstuff/)

## ↑ Ancestors (6)

1. [Gershgorin circle theorem](gershgorin-circle-theorem.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Diagonal scaling of Gershgorin discs](diagonal-scaling-of-gershgorin-discs.md)
- [Gershgorin bounds for symmetric matrices](gershgorin-bounds-for-symmetric-matrices.md)
- [Gershgorin circle theorem](gershgorin-circle-theorem.md)
- [Gershgorin disc](gershgorin-disc.md)
- [Gershgorin eigenvalue counting](gershgorin-eigenvalue-counting.md)
- [Gershgorin gap bound for an adiabatic history path](gershgorin-gap-bound-for-an-adiabatic-history-path.md)
- [Gershgorin stability bound for a variable-coefficient diffusion stencil](gershgorin-stability-bound-for-a-variable-coefficient-diffusion-stencil.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-67/2/c/solution.md)
