# Initial-data decomposition into two normal modes

↑ **Parent:** [Normal mode](normal-mode.md)

Suppose a two-coordinate linear oscillator has independent [normal modes](normal-mode.md) $v_1,v_2$ as displayed, with positive angular frequencies $\omega_1,\omega_2$. For initial displacement $d=(d_1,d_2)^T$ and velocity $w=(w_1,w_2)^T$, its solution is

$$
x(t)=\sum_{j=1}^2v_j\left[c_j\cos(\omega_jt)+\frac{b_j}{\omega_j}\sin(\omega_jt)\right],
$$

where

$$
c_1=\frac{d_2-r_2d_1}{r_1-r_2},\quad c_2=\frac{r_1d_1-d_2}{r_1-r_2},\qquad b_1=\frac{w_2-r_2w_1}{r_1-r_2},\quad b_2=\frac{r_1w_1-w_2}{r_1-r_2}.
$$

These formulas follow by inverting the two-by-two matrix with columns $v_1,v_2$. Each coefficient evolves by its own scalar harmonic-oscillator equation, and substituting $t=0$ recovers both prescribed vectors. Euclidean orthogonality of the mode shapes is unnecessary; with unequal masses, the natural orthogonality is in the mass inner product of the [generalized eigenvalue problem for small oscillations](generalized-eigenvalue-problem-for-small-oscillations.md).

## ↑ Ancestors (7)

1. [Normal mode](normal-mode.md)
2. [Wave equation](wave-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-2/7/ii/solution.md)
