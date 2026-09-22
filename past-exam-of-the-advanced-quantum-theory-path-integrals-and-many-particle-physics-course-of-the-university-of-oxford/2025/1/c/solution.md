<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take the [thermodynamic limit](../../../../thermodynamic-limit.md) $N\to\infty$ at fixed separation $n$ and fixed finite $K=\beta J>0$. Since $|t|=\tanh K<1$, the terms $t^{N-n}$ and $t^N$ in the [finite-ring antiferromagnetic Ising correlation](../../../../finite-ring-antiferromagnetic-ising-correlation.md) vanish, through either even or odd $N$. Therefore

$$
C_n\longrightarrow t^n=(-1)^n(\tanh K)^n
=(-1)^n\exp\bigl[n\log(\tanh K)\bigr].
$$

Matching the decaying [exponential function](../../../../exponential-function.md) gives the [correlation length](../../../../correlation-length.md), in units of the site spacing:

$$
\boxed{\langle S_1S_{n+1}\rangle=(-1)^ne^{-n/\xi},\qquad
\xi=-\frac1{\log\tanh(\beta J)}
=\frac1{\log\coth(\beta J)}.}
$$

If the physical spacing is $a$, the physical [correlation length](../../../../correlation-length.md) is $a\xi$. The alternating sign records the preferred opposite orientation of neighboring [Ising spins](../../../../ising-spin-variable.md); the finite [correlation length](../../../../correlation-length.md) shows that this preference does not maintain long-range [Néel order](../../../../neel-state.md) at positive [temperature](../../../../temperature-split.md).

For large $K$, $\tanh K=1-2e^{-2K}+O(e^{-4K})$, so $\xi\sim e^{2K}/2$: the [correlation length](../../../../correlation-length.md) becomes large on cooling, but diverges only at zero [temperature](../../../../temperature-split.md). At infinite [temperature](../../../../temperature-split.md), $K\to0^+$ and $\xi\to0$; the separate equal-site [two-point correlation function](../../../../two-point-correlation-function.md) remains $C_0=1$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
