# ADHM factorization identity

↑ **Parent:** [ADHM construction](adhm-construction.md)

With $z_1=x^1+ix^2$, $z_2=x^3+ix^4$, form

$$
\mathcal D_z=\begin{pmatrix}B_2-z_2&B_1-z_1&I\\-B_1^\dagger+\bar z_1&B_2^\dagger-\bar z_2&J^\dagger\end{pmatrix}.
$$

The two [ADHM construction](adhm-construction.md) constraints say that $\mathcal D_z\mathcal D_z^\dagger$ has zero off-diagonal blocks and equal diagonal blocks, so it equals $1_2\otimes f^{-1}$. Assume it is invertible everywhere. Choose an orthonormal kernel [bundle frame](frame-of-a-vector-bundle.md) $\Psi$, so $\mathcal D_z\Psi=0$ and $\Psi^\dagger\Psi=1_N$, and set $A=\Psi^\dagger d\Psi$. The orthogonal complement projector is $1-\Psi\Psi^\dagger=\mathcal D_z^\dagger(1_2\otimes f)\mathcal D_z$. Differentiating the kernel equation gives

$$
F=\Psi^\dagger d\mathcal D_z^\dagger(1_2\otimes f)\wedge d\mathcal D_z\Psi.
$$

Its space-time [differential two-form](2-form.md) entries are combinations of $dz_1\wedge d\bar z_1-dz_2\wedge d\bar z_2$, $dz_1\wedge d\bar z_2$, and $d\bar z_1\wedge dz_2$, all anti-self-dual. Thus the constructed [gauge curvature](gauge-field-strength.md) satisfies the [Anti-self-dual Yang-Mills equations](anti-self-dual-yang-mills-equations.md).

## ↑ Ancestors (8)

1. [ADHM construction](adhm-construction.md)
2. [Yang-Mills instanton](yang-mills-instanton.md)
3. [Gauge-theory soliton](gauge-theory-soliton.md)
4. [Classical field-theory soliton](classical-field-theory-soliton-split.md)
5. [Quantum field theory](quantum-field-theory-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [ADHM construction](adhm-construction.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-56/3/solution.md)
