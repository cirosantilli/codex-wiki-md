<h1 id="38c/solution">Solution</h1>

↑ **Parent:** [38C](../38c.md)

The interface is the material level set $F=r-R(\theta,t)=0$. The condition $DF/Dt=0$ gives

$$
-R_t+u-\frac vrR_\theta=0,
$$

which is the stated equation.

Let the perturbation potentials inside and outside be

$$
\phi_i=A r^k e^{ik\theta+\sigma t},
\qquad
\phi_o=B r^{-k}e^{ik\theta+\sigma t}.
$$

Linearizing the kinematic condition at $r=a$ gives

$$
(\sigma+ik\omega)\eta=kAa^{k-1},
\qquad
\sigma\eta=-kBa^{-k-1}.
$$

The linearized interior Euler equations give

$$
p_i'=-\rho[\sigma+i(k-2)\omega]\phi_i,
$$

whereas the stationary exterior gives $p_o'=-\rho\sigma\phi_o$. Since the basic interior [pressure](../../../../../pressure.md) has $dp_i/dr=\rho\omega^2r$, [pressure](../../../../../pressure.md) continuity on the displaced boundary is

$$
p_i'(a)+\rho\omega^2a\eta=p_o'(a).
$$

Eliminating $A$ and $B$ gives the [circular vortex-sheet mode](../../../../../circular-vortex-sheet-mode.md) relation

$$
\sigma^2+i\omega(k-1)\sigma
-\frac12\omega^2k(k-1)=0,
$$

so

$$
\boxed{\displaystyle
\sigma=\frac\omega2\left[-i(k-1)\pm\sqrt{k^2-1}\right]}.
$$

The $k=1$ mode is a neutral displacement. Every $k>1$ mode has one exponentially growing branch, so the circular interface rolls up through a Kelvin--Helmholtz instability. Its pattern angular [velocity](../../../../../velocity.md) is $\omega(k-1)/(2k)$, in the direction of the gyre but slower than the solid-body motion; the disturbances therefore propagate upstream relative to the rotating water.

## ↑ Ancestors (10)

1. [38C](../38c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
