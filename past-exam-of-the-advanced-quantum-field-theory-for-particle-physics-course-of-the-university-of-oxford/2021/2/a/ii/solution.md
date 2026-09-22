<h1 id="2/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\Sigma=m_e^2+m_t^2$, $Q_e=-1$, $Q_t=2/3$ and $N_c=3$. The single [tree-level Feynman diagram](../../../../../tree-level-feynman-diagram.md) is annihilation through a [virtual photon](../../../../../virtual-photon.md). Up to an irrelevant common phase, its [scattering amplitude](../../../../../scattering-amplitude.md) is

$$
\mathcal M_\gamma=\frac{e^2Q_eQ_t}{s}\,[\bar v(p_2)\gamma^\mu u(p_1)]\,[\bar u(p_3)\gamma_\mu v(p_4)]\,\delta_{cd}.
$$

There are two initial [spin angular momentum](../../../../../spin.md) states for each particle, so the [spin average](../../../../../spin-average.md) is $1/4$. The final [color charge](../../../../../color-charge.md) sum gives $\sum_{c,d}|\delta_{cd}|^2=N_c$. There is no additional [photon polarization](../../../../../photon-polarization.md) average for a [virtual photon](../../../../../virtual-photon.md) and no separate polarization label beyond the [Dirac spinor](../../../../../dirac-spinor.md) [spin sums](../../../../../spin-sum.md).

The [spin sums](../../../../../spin-sum.md) and the [gamma-matrix trace](../../../../../gamma-matrix-trace.md) identities give

$$
\begin{aligned}
L^{\mu\nu}&=\operatorname{tr}[(\not p_2-m_e)\gamma^\mu(\not p_1+m_e)\gamma^\nu]\\
&=4[p_2^\mu p_1^\nu+p_2^\nu p_1^\mu-\tfrac{s}{2}g^{\mu\nu}],\\
H_{\mu\nu}&=\operatorname{tr}[(\not p_3+m_t)\gamma_\mu(\not p_4-m_t)\gamma_\nu]\\
&=4[p_{3\mu}p_{4\nu}+p_{3\nu}p_{4\mu}-\tfrac{s}{2}g_{\mu\nu}].
\end{aligned}
$$

Here $p_1\cdot p_2+m_e^2=p_3\cdot p_4+m_t^2=s/2$. Contracting gives

$$
\frac14L^{\mu\nu}H_{\mu\nu}
=8[(p_1\cdot p_3)(p_2\cdot p_4)+(p_1\cdot p_4)(p_2\cdot p_3)]+4s\Sigma.
$$

Since $2p_1\cdot p_3=2p_2\cdot p_4=\Sigma-t$ and $2p_1\cdot p_4=2p_2\cdot p_3=\Sigma-u$, this is the [massive vector-current annihilation kernel](../../../../../massive-vector-current-annihilation-kernel.md)

$$
2[(\Sigma-t)^2+(\Sigma-u)^2+2s\Sigma]
=2[t^2+u^2+4s\Sigma-2\Sigma^2].
$$

Thus the absolutely normalized result is

$$
\boxed{\overline{|\mathcal M_\gamma|^2}
=\frac{2N_ce^4Q_e^2Q_t^2}{s^2}[t^2+u^2+4s\Sigma-2\Sigma^2]
=\frac{8e^4}{3s^2}[t^2+u^2+4s\Sigma-2\Sigma^2].}
$$

After taking out the displayed prefactor, $\boxed{A=1,\ B=4,\ C=-2}$. Because the source uses a proportionality sign, only their ratio is fixed until that prefactor is specified. Equivalently, after taking out just $e^4/s^2$, their values are $8/3,32/3,-16/3$. No mass has been neglected. At $m_e=0$ and $s=4m_t^2$, the bracket yields the finite isotropic threshold value of the [scattering amplitude](../../../../../scattering-amplitude.md); the vanishing threshold [scattering cross-section](../../../../../scattering-cross-section.md) comes from [relativistic two-body phase space](../../../../../relativistic-two-body-phase-space.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
