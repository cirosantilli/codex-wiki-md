# Hermitian two-by-two matrix in the Pauli basis

↑ **Parent:** [Pauli matrices](pauli-matrices.md)

Every [Hermitian matrix](hermitian-operator.md) of size two can be written uniquely as $M=dI+b_x\sigma_x+b_y\sigma_y+b_z\sigma_z$ with real coefficients. For $M=\begin{pmatrix}u&w\\w^*&z\end{pmatrix}$, take $d=(u+z)/2$, $b_z=(u-z)/2$, $b_x=\operatorname{Re}w$ and $b_y=-\operatorname{Im}w$. Alternatively, $d=\operatorname{tr}M/2$ and $b_i=\operatorname{tr}(M\sigma_i)/2$ follow from the trace orthogonality of the [Pauli matrices](pauli-matrices.md) and the [identity matrix](identity-matrix.md).

The [Pauli matrix multiplication law](pauli-matrix-multiplication-law.md) gives $(\mathbf b\cdot\boldsymbol\sigma)^2=|\mathbf b|^2I$, hence the two [eigenvalues](eigenvalue.md) are $d\pm|\mathbf b|$. For $\mathbf b\ne0$, the corresponding pure-state [Bloch vectors](bloch-vector.md) are $\pm\mathbf b/|\mathbf b|$.

## ↑ Ancestors (5)

1. [Pauli matrices](pauli-matrices.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Constant matrix perturbation of a Weyl Hamiltonian](constant-matrix-perturbation-of-a-weyl-hamiltonian.md)
- [Solution](past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2018/section-b/b3/solution.md)
