<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the ordered basis $(|1\rangle,|2\rangle)$ and $\sigma_z=\operatorname{diag}(1,-1)$, with

$$
\rho=\tfrac12(I+\mathbf R\cdot\boldsymbol\sigma),\qquad
R_z=p_1-p_2,\quad p_2=\frac{1-R_z}{2}.
$$

A pure [quantum superposition](../../../../quantum-superposition.md) $|+x\rangle=(|1\rangle+|2\rangle)/\sqrt2$ has $\mathbf R=(1,0,0)$ on the [Bloch sphere](../../../../bloch-sphere.md). In contrast, a [mixed state](../../../../mixed-state.md) $\rho=p|1\rangle\langle1|+(1-p)|2\rangle\langle2|$ has $\mathbf R=(0,0,2p-1)$, inside the sphere for $0<p<1$. At equal populations its vector is zero. Equal populations alone therefore do not distinguish a coherent superposition from a mixture; their off-diagonal [density matrix](../../../../density-matrix-split.md) elements differ.

Choose the drive [phase](../../../../phase-waves.md) so the rotating-frame [Hamiltonian](../../../../hamiltonian.md) is $H_{\rm rot}=\hbar(\Omega\sigma_x+\delta\sigma_z)/2$, where $\delta=\omega-\omega_0$ as specified. The [Rabi vector](../../../../rabi-vector.md) is the angular-velocity vector

$$
\boxed{\mathbf W=(\Omega,0,\delta),\qquad \dot{\mathbf R}=\mathbf W\times\mathbf R.}
$$

Here $\Omega$ is the on-resonance population oscillation [angular frequency](../../../../angular-frequency.md), not the unhalved coefficient of a cosine coupling. From $\mathbf R(0)=\hat z$, rotation about $\mathbf W$ at $W=\sqrt{\Omega^2+\delta^2}$ gives

$$
\mathbf R(t)=\left(\frac{\Omega\delta}{W^2}[1-\cos Wt],\,-\frac{\Omega}{W}\sin Wt,\,
\frac{\delta^2+\Omega^2\cos Wt}{W^2}\right),
$$



$$
\boxed{p_2(t)=\frac{\Omega^2}{\Omega^2+\delta^2}\sin^2\left(\frac{\sqrt{\Omega^2+\delta^2}\,t}{2}\right).}
$$

For $\Omega\gg|\delta|$, the rotation axis is nearly transverse, the trajectory nearly a great circle, and transfer is almost complete. For $\Omega=\delta>0$, the axis bisects $+x$ and $+z$, the orbit lies in $R_x+R_z=1$, and $p_2=\tfrac12\sin^2(\sqrt2\Omega t/2)$ never exceeds $1/2$. Each member remains a [pure state](../../../../pure-state.md) in this coherent evolution.

<a id="1/image-pure-and-mixed-bloch-vectors-resonant-and-detuned-trajectories-and-their-population-oscillations"></a>
![](../../../../past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2015/paper-1-rabi-bloch.png)

**[Figure 1](#1/image-pure-and-mixed-bloch-vectors-resonant-and-detuned-trajectories-and-their-population-oscillations). Pure and mixed Bloch vectors, resonant and detuned trajectories, and their population oscillations**.

For the Ramsey free interval, let atom $j$ have detuning $\delta_j=\delta+\eta_j$. Instantaneous ideal pulses give the [Ramsey ensemble coherence](../../../../ramsey-ensemble-coherence.md) factor $\chi(T)=\langle e^{i\eta_jT}\rangle$. Averaging the free-evolution vector obtained in step (ii) gives

$$
\overline{\mathbf R}(T)=\left(\operatorname{Im}[e^{i\delta T}\chi(T)],\,-\operatorname{Re}[e^{i\delta T}\chi(T)],\,0\right),
\qquad
\boxed{\overline p_2(T)=\tfrac12\{1+\operatorname{Re}[e^{i\delta T}\chi(T)]\}.}
$$

Different atoms fan out around the equator, shortening the ensemble [Bloch vector](../../../../bloch-vector.md) even though every individual's vector remains unit length. A broad smooth detuning distribution usually makes the average spiral towards the centre and damps the Ramsey fringes towards $1/2$. The [dephasing](../../../../dephasing-channel.md) time is of order $1/\Delta\omega_0\sim5/\delta$. [inhomogeneous ensemble dephasing](../../../../inhomogeneous-ensemble-dephasing.md) is not necessarily irreversible decoherence of individual atoms; an appropriate [spin echo](../../../../spin-echo.md) can rephase static [frequency](../../../../frequency.md) offsets.

The given spread does not specify a [probability distribution](../../../../probability-distribution-split.md) or whether it denotes an RMS width. An exact envelope is therefore not determined. The figure illustrates, rather than infers, a [Gaussian distribution](../../../../normal-distribution.md) with RMS $\sigma_\delta=0.2\delta$, for which $\chi=e^{-\sigma_\delta^2T^2/2}$. A [uniform distribution](../../../../continuous-uniform-distribution.md) would instead give a sinc envelope and side lobes. Both have the same qualitative initial loss of contrast on the quoted inverse-spread scale.

<a id="1/image-an-ideal-ramsey-path-and-an-explicitly-illustrative-gaussian-ensemble-dephasing-envelope"></a>
![](../../../../past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2015/paper-1-ramsey.png)

**[Figure 2](#1/image-an-ideal-ramsey-path-and-an-explicitly-illustrative-gaussian-ensemble-dephasing-envelope). An ideal Ramsey path and an explicitly illustrative Gaussian ensemble-dephasing envelope**.

In the [rubidium-87 ground-state hyperfine structure](../../../../rubidium-87-ground-state-hyperfine-structure.md), $J=1/2$ and $I=3/2$, so $F=1,2$. Taking $H_{\rm hf}=A\mathbf I\cdot\mathbf J/\hbar^2$ gives

$$
E_F=\frac A2[F(F+1)-I(I+1)-J(J+1)],\qquad
E_1=-\frac54A,\quad E_2=\frac34A.
$$

The zero-field splitting is $\Delta_{\rm hf}=2A\simeq h\times6.8\,\mathrm{GHz}$. Ignoring the small nuclear magnetic term, the weak-field [Landé g-factors](../../../../lande-g-factor.md) are $g_{F=1}\simeq-1/2$ and $g_{F=2}\simeq+1/2$. The diagram labels all three $F=1$ and five $F=2$ substates, with linear shifts $g_F\mu_Bm_FB$.

The pair **$|1\rangle=|F=1,m_F=0\rangle$ and $|2\rangle=|F=2,m_F=0\rangle$** is connected by a [magnetic dipole transition](../../../../magnetic-dipole-transition.md) with $\Delta F=1$, $\Delta m_F=0$, driven with its oscillating magnetic component along the quantization axis. Both first-order shifts vanish, giving the [rubidium-87 clock transition](../../../../rubidium-87-clock-transition.md) first-order insensitivity near zero field. Its insensitivity does not imply absence of quadratic shifts.

For these two $m_F=0$ levels the [Breit-Rabi formula](../../../../breit-rabi-formula.md) gives the [quadratic Zeeman shift of a clock transition](../../../../quadratic-zeeman-shift-of-a-clock-transition.md):

$$
\Delta E(B)=\sqrt{(2A)^2+[(g_J-g_I)\mu_BB]^2}
\simeq2A+\frac{\mu_B^2B^2}{A},
$$

where the last expression neglects the nuclear term and sets $g_J\simeq2$. Hence

$$
\frac{\partial\Delta E}{\partial B}\simeq\frac{2\mu_B^2B}{A},\qquad
\boxed{\frac{|\mu_2-\mu_1|}{\mu_B}\simeq\frac{2\mu_BB}{A}\simeq8.2\times10^{-3}\quad(B=10\,\mathrm G).}
$$

This uses $\mu_B/h\simeq1.40\,\mathrm{MHz/G}$ and the supplied $A/h\simeq3.4\,\mathrm{GHz}$. With physical moments defined by $\mu_i=-\partial E_i/\partial B$, the [differential magnetic moment](../../../../differential-magnetic-moment.md) is **$\mu_2-\mu_1\simeq-8.2\times10^{-3}\mu_B$**. If effective magnetic moment denotes the positive [energy](../../../../energy-split.md) slope instead, that slope difference is positive. The magnitude and physical [frequency](../../../../frequency.md) sensitivity are the same. Retaining the full atomic factors gives the familiar quadratic clock-frequency coefficient about $575\,\mathrm{Hz/G^2}$; the simplified supplied parameters give about $576\,\mathrm{Hz/G^2}$.[§3, equations (26)–(29); table of magnetic factors and clock-transition quadratic shift](../../../../rubidium-87-d-line-data-by-daniel-a-steck.md)

<a id="1/image-weak-field-rubidium-87-hyperfine-manifolds-and-the-quadratic-clock-transition-shift"></a>
![](../../../../past-exam-of-the-atomic-and-optical-physics-course-of-the-university-of-cambridge/2015/paper-1-rubidium-levels.png)

**[Figure 3](#1/image-weak-field-rubidium-87-hyperfine-manifolds-and-the-quadratic-clock-transition-shift). Weak-field rubidium-87 hyperfine manifolds and the quadratic clock-transition shift**.

**Use a far-detuned [optical dipole trap](../../../../optical-dipole-trap.md)**, such as a red-detuned focused-beam trap, to confine both clock states. Their first-order magnetic moments vanish; their residual quadratic magnetic slopes are opposite, so a simple static magnetic-field minimum does not confine both in the same way. An optical potential acts through the electronic [polarizability](../../../../electric-polarizability.md) and can trap both ground hyperfine states. It is not perfectly state independent: differential [AC Stark shifts](../../../../ac-stark-shift.md), intensity noise and residual magnetic gradients still need control during Ramsey evolution.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the atomic and Optical Physics course of the University of Cambridge](../../../split.md)
5. [Atomic and Optical Physics course of the University of Cambridge](../../../../atomic-and-optical-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
