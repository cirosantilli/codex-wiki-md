# Surface sources of a discontinuous Lighthill stress tensor

↑ **Parent:** [Lighthill stress tensor](lighthill-stress-tensor.md)

Write a piecewise smooth [Lighthill stress tensor](lighthill-stress-tensor.md) as $T_{ij}=T^-_{ij}+D_{ij}H(S)$, where $D_{ij}=T^+_{ij}-T^-_{ij}$ and the regular level surface $S=0$ is a [shock wave](shock-wave.md). The [distributional derivative of the Heaviside step function](distributional-derivative-of-the-heaviside-step-function.md) gives

$$
\partial_i\partial_jT_{ij}=H(S)\partial_i\partial_jT^+_{ij}+H(-S)\partial_i\partial_jT^-_{ij}+(D_{ij,i}S_j+D_{ij,j}S_i+D_{ij}S_{ij})\delta(S)+D_{ij}S_iS_j\delta'(S).
$$

Here repeated indices are summed, $S_i=\partial_iS$ and $S_{ij}=\partial_i\partial_jS$. Keep the coefficients as smooth extensions before multiplying distributions: prematurely replacing the coefficient of $\delta'(S)$ by its surface trace can lose a $\delta(S)$ contribution. The extra [surface delta distributions](surface-delta-distribution.md) and their derivatives are supported entirely on the discontinuity.

## ↑ Ancestors (7)

1. [Lighthill stress tensor](lighthill-stress-tensor.md)
2. [Lighthill acoustic analogy](lighthill-acoustic-analogy.md)
3. [Linear acoustics](linear-acoustics-split.md)
4. [Fluid mechanics](fluid-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-82/1/b/i/solution.md)
