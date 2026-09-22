# Radial Schwartz approximation of tempered distributions

↑ **Parent:** [Radial tempered distribution](radial-tempered-distribution.md)

Choose a radial [mollifier](mollifier.md) $\rho\in C_c^\infty$ with integral one and support in the unit ball, and a radial [cutoff function](cutoff-function.md) $\chi\in C_c^\infty$ equal to one there. For a [radial tempered distribution](radial-tempered-distribution.md) $T$, the functions

$$
f_j(x)=\chi(x/j)(T*\rho_{1/j})(x),\qquad \rho_\varepsilon(x)=\varepsilon^{-n}\rho(x/\varepsilon),
$$

are radial [Schwartz functions](schwartz-function.md). Smoothness comes from [convolution of a tempered distribution with a Schwartz function](convolution-of-a-tempered-distribution-with-a-schwartz-function.md), and compact support comes from the cutoff. Pairing with $\varphi$ gives $\langle f_j,\varphi\rangle=\langle T,\check\rho_{1/j}*(\chi(\cdot/j)\varphi)\rangle$. With $q_m(\varphi)=\max_{|\beta|\leq m}\sup_x(1+|x|)^m|\partial^\beta\varphi(x)|$, the cutoff tail and the [mean value theorem](mean-value-theorem.md) give

$$
q_m\!\left(\check\rho_{1/j}*(\chi(\cdot/j)\varphi)-\varphi\right)\leq C_mj^{-1}q_{m+1}(\varphi).
$$

The continuity estimate for $T$ therefore proves $f_j\to T$ even in the [strong dual topology](strong-dual-topology.md). Inserting a cutoff is essential because convolution alone need not give rapid decay.

## ↑ Ancestors (8)

1. [Radial tempered distribution](radial-tempered-distribution.md)
2. [Tempered distribution](tempered-distribution.md)
3. [Schwartz space](schwartz-space.md)
4. [Fourier analysis](fourier-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-327/2/ii/solution.md)
