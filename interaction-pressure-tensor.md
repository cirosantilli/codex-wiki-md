# Interaction pressure tensor

↑ **Parent:** [Pressure tensor](pressure-tensor.md)

For a central differentiable [pair potential](pair-potential.md), an exact local representation of the interaction [momentum flux](momentum-flux.md) is

$$
P^\phi_{ij}(\mathbf x)=-\frac12\int d^3R\,\frac{R_iR_j}{R}\phi'(R)\int_0^1n_2(\mathbf x+(s-1)\mathbf R,\mathbf x+s\mathbf R)\,ds.
$$

Here $n_2$ is the [two-particle number density](two-particle-number-density.md). The line integral assigns each pair's exchanged [momentum](momentum-split.md) along the segment joining the particles. Translating both endpoints gives $\partial_s n_2=\mathbf R\cdot\nabla_{\mathbf x}n_2$. Integrating over $s$ and using pair-exchange symmetry proves that $-\nabla\cdot\mathbf P^\phi$ is the interaction [force density](force-density.md). Its homogeneous isotropic specialization gives the interaction part of the [virial pressure from pair correlations](virial-pressure-from-pair-correlations.md). The kinetic [pressure tensor](pressure-tensor.md) accounts separately for random particle motion.

## ↑ Ancestors (7)

1. [Pressure tensor](pressure-tensor.md)
2. [Pressure](pressure-split.md)
3. [Thermodynamics](thermodynamics-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-kinetic-theory-course-of-the-university-of-oxford/2024/1/c/solution.md)
