<h1 id="section-c/c10/solution">Solution</h1>

↑ **Parent:** [C10](../c10.md)

A localized quantum particle is described by a [wave packet](../../../../../wave-packet.md): a coherent [quantum superposition](../../../../../quantum-superposition.md) of [momentum](../../../../../momentum-split.md) components, rather than a single delocalized [plane wave](../../../../../plane-wave.md). The [Born rule](../../../../../born-rule.md) assigns the [position](../../../../../position.md) [probability density](../../../../../probability-density.md) $|\psi(x,t)|^2$. A useful normalized initial [Gaussian wave packet](../../../../../gaussian-wave-packet.md) is

$$
\psi(x,0)=(2\pi\sigma_0^2)^{-1/4}\exp\left[-\frac{(x-x_0)^2}{4\sigma_0^2}+\frac{ip_0(x-x_0)}\hbar\right].
$$

Its mean [position](../../../../../position.md) and [momentum](../../../../../momentum-split.md) are $x_0$ and $p_0$, and its [standard deviations](../../../../../standard-deviation.md) satisfy $\sigma_x(0)=\sigma_0$, $\sigma_p=\hbar/(2\sigma_0)$. This unchirped initial state saturates the [Heisenberg uncertainty relation](../../../../../heisenberg-uncertainty-relation.md).

For a [free particle](../../../../../free-particle.md), the momentum-space [Schrödinger equation](../../../../../schrodinger-equation.md) multiplies each [amplitude](../../../../../wave-amplitude.md) by $e^{-ip^2t/(2m\hbar)}$. The inverse [Fourier transform](../../../../../fourier-transform-split.md) is a [Gaussian integral](../../../../../gaussian-integral.md), giving the [free Gaussian wave packet evolution](../../../../../free-gaussian-wave-packet-evolution.md)

$$
\psi(x,t)=\frac{(2\pi\sigma_0^2)^{-1/4}}{\sqrt{1+i\eta}}\exp\left[-\frac{(x-x_0-p_0t/m)^2}{4\sigma_0^2(1+i\eta)}+\frac{ip_0(x-x_0)}\hbar-\frac{ip_0^2t}{2m\hbar}\right],\qquad \eta=\frac{\hbar t}{2m\sigma_0^2}.
$$

One way to obtain this expression explicitly is to write the initial [momentum](../../../../../momentum-split.md) [amplitude](../../../../../wave-amplitude.md) as proportional to $\exp[-\sigma_0^2(p-p_0)^2/\hbar^2-ipx_0/\hbar]$, multiply by the free evolution phase and complete the square in $p$. Taking the modulus squared removes the position-dependent phase and leaves

$$
\boxed{|\psi(x,t)|^2=\frac{1}{\sqrt{2\pi}\sigma_x(t)}\exp\left[-\frac{(x-x_c(t))^2}{2\sigma_x(t)^2}\right],\quad x_c(t)=x_0+\frac{p_0t}{m},\quad \sigma_x(t)=\sigma_0\sqrt{1+\left(\frac{t}{\tau}\right)^2},\quad \tau=\frac{2m\sigma_0^2}{\hbar}.}
$$

The [expectation value](../../../../../expectation-value.md) follows uniform classical motion while the density spreads. A narrower initial packet needs a wider [momentum](../../../../../momentum-split.md) distribution and therefore spreads more rapidly. At long times its width grows linearly with $|t|$; its [variance](../../../../../variance-split.md) grows quadratically, unlike the linear [variance](../../../../../variance-split.md) growth of ordinary [diffusion](../../../../../diffusion.md). The [probability continuity equation](../../../../../probability-continuity-equation.md) preserves total [probability](../../../../../probability.md) despite the decreasing peak height. The mean [momentum](../../../../../momentum-split.md) and the mean [energy](../../../../../energy-split.md) $(p_0^2+\sigma_p^2)/(2m)$ remain constant, since the [momentum](../../../../../momentum-split.md) populations do not change.

The same result has a wave interpretation. For a free nonrelativistic particle $\omega(k)=\hbar k^2/(2m)$, so the [group velocity](../../../../../group-velocity.md) is $d\omega/dk=\hbar k/m$, equal to $p_0/m$ at the packet center. The curvature $d^2\omega/dk^2=\hbar/m$ makes different [momentum](../../../../../momentum-split.md) components travel with different [group velocities](../../../../../group-velocity.md), producing dispersion. The [phase velocity](../../../../../phase-velocity.md) is $\omega/k=\hbar k/(2m)$ for this [energy](../../../../../energy-split.md) convention and does not describe the motion of the envelope. The evolving quadratic spatial phase is essential to the spreading; a density snapshot alone does not specify the full [quantum state](../../../../../quantum-state.md).

A freely spreading [Gaussian wave packet](../../../../../gaussian-wave-packet.md) remains a pure Gaussian state but develops position-momentum correlations. Its symmetrized [covariance](../../../../../covariance.md) is $C_{xp}=\langle\{x-\langle x\rangle,p-\langle p\rangle\}\rangle/2=t\sigma_p^2/m$. Consequently

$$
\sigma_x\sigma_p=\frac\hbar2\sqrt{1+\eta^2},\qquad \boxed{\sigma_x^2\sigma_p^2-C_{xp}^2=\frac{\hbar^2}{4}.}
$$

Equality in the [Robertson-Schrödinger uncertainty relation](../../../../../robertson-schrodinger-uncertainty-relation.md) survives at every time, whereas the simpler product $\sigma_x\sigma_p$ equals $\hbar/2$ only initially. A [chirped Gaussian wave packet](../../../../../chirped-gaussian-wave-packet.md) can already have $C_{xp}(0)\ne0$. More generally, $x(t)=x(0)+p(0)t/m$ gives $\sigma_x(t)^2=\sigma_x(0)^2+2tC_{xp}(0)/m+t^2\sigma_p(0)^2/m^2$. A sufficiently negative initial [covariance](../../../../../covariance.md) permits initial contraction before subsequent spreading.

<a id="section-c/c10/image-free-gaussian-spreading-constant-coherent-state-width-and-the-breathing-width-of-a-squeezed-state"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1-gaussian-packets.png)

**[Figure 3](#section-c/c10/image-free-gaussian-spreading-constant-coherent-state-width-and-the-breathing-width-of-a-squeezed-state). Free Gaussian spreading, constant coherent-state width and the breathing width of a squeezed state**.

A [potential energy](../../../../../potential-energy.md) changes this behavior. A quadratic potential preserves the Gaussian form because the evolution of [position](../../../../../position.md) and [momentum](../../../../../momentum-split.md) is linear. For a [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator-split.md), the [Gaussian covariance in a harmonic potential](../../../../../gaussian-covariance-in-a-harmonic-potential.md) is

$$
\sigma_x(t)^2=\sigma_x(0)^2\cos^2\omega t+\frac{\sigma_p(0)^2}{m^2\omega^2}\sin^2\omega t+\frac{2C_{xp}(0)}{m\omega}\sin\omega t\cos\omega t.
$$

A [coherent state](../../../../../coherent-state.md) has $\sigma_x^2=\hbar/(2m\omega)$, $\sigma_p^2=m\hbar\omega/2$ and zero centered [covariance](../../../../../covariance.md). Its width is constant, and its center follows $x_c(t)=x_0\cos\omega t+p_0\sin\omega t/(m\omega)$. In oscillator notation its [coherent state](../../../../../coherent-state.md) label rotates as $\alpha(t)=\alpha(0)e^{-i\omega t}$, apart from the common ground-energy phase of the [state vector](../../../../../state-vector.md). A [squeezed coherent state](../../../../../squeezed-coherent-state.md) generally has a width that breathes at $2\omega$. Thus being Gaussian does not imply either free spreading or constant width; the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) and initial [covariance](../../../../../covariance.md) determine the result.

For a general nonquadratic potential, different parts of the packet experience different nonlinear forces, and an initially Gaussian profile need not remain Gaussian. [Ehrenfest theorem](../../../../../ehrenfest-theorem.md) gives the exact relations $d\langle x\rangle/dt=\langle p\rangle/m$ and $d\langle p\rangle/dt=-\langle V'(x)\rangle$. Replacing the last mean by $-V'(\langle x\rangle)$ is exact for a quadratic potential and approximate for a packet narrow compared with the scale on which the force varies. This connects packet motion to the [correspondence principle](../../../../../correspondence-principle.md) without treating a [quantum state](../../../../../quantum-state.md) as a definite classical path. Scattering can split a packet into reflected and transmitted components, while confinement can produce oscillations and interference between discrete [energy eigenstates](../../../../../energy-eigenstate.md). Their relative phases evolve even when their populations remain constant. Localization, spreading and coherent motion all follow from the same linear [unitary time evolution](../../../../../unitary-time-evolution.md).

## ↑ Ancestors (14)

1. [C10](../c10.md)
2. [Section C](../../section-c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2019](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
