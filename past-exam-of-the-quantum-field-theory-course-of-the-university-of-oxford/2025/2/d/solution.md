<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For an allowed [decay channel](../../../../decay-channel.md) in [iii](../c/iii.md), $|\mathcal M|^2=h^2$. Integrating the spatial [Dirac delta distribution](../../../../dirac-delta-function.md) in the printed [Lorentz-invariant phase-space measure](../../../../lorentz-invariant-phase-space-measure.md) sets $\mathbf p_2=-\mathbf p_1$. With $p=|\mathbf p_1|$ and $E_p=\sqrt{p^2+m^2}$, its remaining value is

$$
\begin{aligned}
I_2&=\int d\Phi_2=\frac1{4(2\pi)^2}\int\frac{d^3\mathbf p}{E_p^2}\,\delta(2E_p-M)\\
&=\frac1{4\pi}\int_0^\infty\frac{p^2\,dp}{E_p^2}\,\delta(2E_p-M).
\end{aligned}
$$

The positive root is $p_*=(M/2)\beta$, where $\beta=\sqrt{1-4m^2/M^2}$, and the [Dirac delta distribution](../../../../dirac-delta-function.md) contributes the [Jacobian determinant](../../../../jacobian-determinant.md) $E_*/(2p_*)$. Hence

$$
I_2=\frac{p_*}{8\pi E_*}=\frac{\beta}{8\pi},\qquad E_*=\frac M2.
$$

It follows that the **literal printed integral** evaluates to

$$
\boxed{\Gamma_{\rm printed}=\frac{h^2}{16\pi M}\sqrt{1-\frac{4m^2}{M^2}}.}
$$

The printed integration ranges count each final configuration twice, once as $(\mathbf p_1,\mathbf p_2)$ and once in the opposite order. For two identical final [bosons](../../../../boson.md), the physical [decay width](../../../../decay-width.md) therefore requires an additional [identical final-state symmetry factor](../../../../identical-particle-factor-in-a-final-state-phase-space-integral.md) $1/2!$:

$$
\boxed{\Gamma_{\rm phys}=\frac{h^2}{32\pi M}\sqrt{1-\frac{4m^2}{M^2}}\simeq\frac{h^2}{32\pi M}\quad(M\gg m).}
$$

There is one allowed [decay channel](../../../../decay-channel.md) per heavy [particle](../../../../particle-physics.md), not an extra factor of two from summing the two charge-conjugate heavy species. Both expressions vanish below the [two-body decay threshold](../../../../two-body-decay-threshold.md) $M=2m$, and the limiting value at threshold is zero. For the literally forbidden labels $\Phi\to\phi\phi$, the [decay width](../../../../decay-width.md) is instead zero because its [decay amplitude](../../../../decay-amplitude.md) vanishes, as explained in [iii](../c/iii.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
