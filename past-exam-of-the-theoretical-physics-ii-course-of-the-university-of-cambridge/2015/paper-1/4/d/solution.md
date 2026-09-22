<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

First [trace](../../../../../matrix-trace.md) the state explicitly specified in (c). [orthogonality](../../../../../orthogonal-vectors.md) in the $y$ oscillator removes terms with different occupation numbers:

$$
\boxed{\rho_x=(1-q)\sum_{n=0}^{\infty}q^n|n\rangle_x\langle n|,
\qquad q=|\lambda|^2=\tanh^2\theta.}
$$

For a thermal oscillator of [frequency](../../../../../frequency.md) $\omega$, the ratio of successive [Boltzmann weights](../../../../../boltzmann-factor.md) is $e^{-\hbar\omega/(k_BT)}$. Consequently the conditional answer for that two-mode squeezed state is

$$
\boxed{T_{\rm sq}=
\frac{\hbar\omega}{k_B\ln(1/\tanh^2\theta)}.}
$$

At $\theta=0$ this is interpreted by the limit $T_{\rm sq}=0$. The reduced state is mixed for nonzero squeezing although the joint state is pure; its effective thermal statistics arise from entanglement, not from heating by a bath.

The ground-state identification must still be qualified. For the true coordinate-coupled [ground state](../../../../../ground-state.md), direct normal-mode averages give

$$
\langle x^2\rangle=\frac{\hbar}{4m}\left(\frac1{\omega_+}+\frac1{\omega_-}\right),
\quad
\langle p_x^2\rangle=\frac{\hbar m}{4}(\omega_++\omega_-),
\quad
\langle xp_x+p_xx\rangle=0.
$$

Their ratio is $m^2\omega_+\omega_-$, rather than $m^2\omega^2$. Therefore this reduced state is not thermal with respect to the original bare [frequency](../../../../../frequency.md) $\omega$ for $k\ne0$. It does have an exact thermal [representation](../../../../../group-representation.md) for an effective oscillator of [mass](../../../../../mass.md) $m$ and [frequency](../../../../../frequency.md)

$$
\nu=\sqrt{\omega_+\omega_-},\qquad
q_{\rm true}=
\left(\frac{\sqrt{\omega_+}-\sqrt{\omega_-}}
{\sqrt{\omega_+}+\sqrt{\omega_-}}\right)^2,
\qquad
\boxed{T_{\rm true}=\frac{\hbar\nu}{k_B\ln(1/q_{\rm true})}.}
$$

The corresponding occupation basis is that of $\nu$, not that of the original $a$. This follows by matching the Gaussian [variances](../../../../../variance-split.md) to $\langle x^2\rangle=\hbar\coth[\hbar\nu/(2k_BT)]/(2m\nu)$ and its [momentum](../../../../../momentum-split.md) counterpart. A direct reduced-Gaussian [eigenfunction](../../../../../eigenfunction.md) calculation gives the same effective [frequency](../../../../../frequency.md) and geometric [eigenvalues](../../../../../eigenvalue.md).[Equations (1)–(5), printed pp. 2–3 of the preprint: two coupled oscillators, partial trace and the effective thermal oscillator frequency](../../../../../entropy-and-area-by-mark-srednicki.md)

## ↑ Ancestors (15)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the theoretical physics II course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics II course of the University of Cambridge](../../../../../theoretical-physics-ii-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
