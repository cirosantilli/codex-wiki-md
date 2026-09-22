<h1 id="34d/solution">Solution</h1>

↑ **Parent:** [34D](../34d.md)

At zero temperature, fill all momentum states inside the Fermi sphere, with two [spin](../../../../../spin.md) states per momentum. Phase-space counting gives

$$
N=2\frac V{(2\pi\hbar)^3}\frac{4\pi p_F^3}{3},\qquad
\boxed{p_F=\hbar(3\pi^2N/V)^{1/3}.}
$$

For dispersion $E=cp$, the ratio of energy to particle-number integrals is

$$
\frac{E_{tot}}N=c\frac{\int_0^{p_F}p^3dp}{\int_0^{p_F}p^2dp}
=\boxed{\frac34cp_F.}
$$

Let $\varepsilon$ be the common [chemical potential](../../../../../chemical-potential.md) in the weak field, and let $+$ denote the lower Zeeman-energy branch $cp-\mu B$. Its populations are

$$
N_\pm=\frac V{6\pi^2\hbar^3c^3}(\varepsilon\pm\mu B)^3.
$$

Keeping $N_++N_-=N$ changes $\varepsilon$ only at order $B^2$, so to first order it equals $\varepsilon_F=cp_F$. Subtracting the two populations gives

$$
N_+-N_-=\frac{3N\mu B}{\varepsilon_F}+O(B^3).
$$

Each excess lower-energy [spin](../../../../../spin.md) contributes moment $\mu$ along the field. Hence the [Pauli moment of a massless electron gas](../../../../../pauli-moment-of-a-massless-electron-gas.md) is

$$
\boxed{\mathcal M=\frac{3N\mu^2B}{cp_F}+O(B^3).}
$$

This includes the [spin](../../../../../spin.md) contribution specified in the problem. The field is weak enough that both [spin](../../../../../spin.md) branches remain occupied, and orbital magnetic effects are not part of the assumed energy model.

## ↑ Ancestors (10)

1. [34D](../34d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
