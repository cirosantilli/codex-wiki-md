# Discrete susceptible-infective model with recruitment

↑ **Parent:** [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)

This generation-based [compartmental model](compartmental-models-epidemiology.md) replenishes the [susceptible compartment](susceptible-compartment.md) by $B>0$ per step and transfers $\alpha S_tI_t$ individuals into the next infectious generation. Members of the current [infectious compartment](infectious-compartment.md) leave it after one step. In scaled variables $x=\alpha S$, $y=\alpha I$, $r=\alpha B$, the update is $x'=x+r-xy$, $y'=xy$.

Its only fixed point is $(S_*,I_*)=(1/\alpha,B)$. There is no finite disease-free fixed point, since susceptible recruitment continues when $I=0$. The [Jacobian matrix](jacobian-matrix.md) at the fixed point is $M=\begin{pmatrix}1-r&-1\\r&1\end{pmatrix}$, with determinant one and trace $2-r$. For $0<r<4$, its two distinct eigenvalues have modulus one, so the linearized iterates are bounded and oscillatory. At $r=4$, the repeated eigenvalue $-1$ has a nontrivial [Jordan block](jordan-block.md), making generic linearized iterates grow linearly. For $r>4$, one eigenvalue has modulus greater than one.

Thus $0<r<4$ gives neutral linear stability, not asymptotic stability. [Unit-modulus multipliers do not determine nonlinear stability](unit-modulus-multipliers-do-not-determine-nonlinear-stability.md). Recruitment can restore susceptibility above $1/\alpha$ after a wave, allowing repeated infection growth; a closed [SIR model](sir-model.md) without replenishment has a different susceptible balance.

## ↑ Ancestors (5)

1. [Compartmental models (epidemiology)](compartmental-models-epidemiology.md)
2. [Mathematical biology](mathematical-biology-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-short-options-course-of-the-university-of-oxford/2017/9/a/i/solution.md)
