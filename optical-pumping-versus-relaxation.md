# Optical pumping versus relaxation

↑ **Parent:** [Optical pumping](optical-pumping.md)

For $\gamma>0$, setting the [rate equations](rate-equation.md) to zero gives the unique [stationary distribution](stationary-distribution.md) of this [continuous-time Markov chain](continuous-time-markov-chain-split.md):

$$
p_-^*=\frac{\gamma}{3\gamma+2R},\qquad
p_0^*=p_+^*=\frac{\gamma+R}{3\gamma+2R},\qquad
\langle m\rangle^*=p_+^*-p_-^*=\frac{R}{3\gamma+2R}.
$$

The nonzero mean [magnetic quantum number](magnetic-quantum-number.md) represents [atomic orientation](atomic-orientation.md). Increasing $R/\gamma$ empties the bright state, but leaves two dark populations. For $R=0$, relaxation alone gives $p_i(t)=1/3+[p_i(0)-1/3]e^{-\gamma t}$. When $\gamma=0$ and $R>0$, every distribution with $p_-=0$ is stationary; the initial difference between the two dark populations survives. The equal dark populations below follow from the specified unpolarized initial condition.

Starting from $p_i(0)=1/3$, the solution for $R>0$ or $\gamma>0$ is

$$
p_-(t)=p_-^*+\left(\frac13-p_-^*\right)e^{-(\gamma+2R/3)t},\qquad
p_0(t)=p_+(t)=\frac{1-p_-(t)}2.
$$

For pure pumping, take $p_-^*=0$ in this formula. Its redistribution time is $3/(2R)$, longer than the mean scattering interval $1/R$ of a bright atom, because one third of scattering events return it to the same sublevel. For arbitrary initial populations the additional mode satisfies $p_0(t)-p_+(t)=[p_0(0)-p_+(0)]e^{-\gamma t}$.

For an original numerical example choose $R=6\ \mathrm{s}^{-1}$ and $\gamma=1\ \mathrm{s}^{-1}$, with $\Gamma$ much larger than either. Then

$$
(p_-^*,p_0^*,p_+^*)=\frac1{15}(1,7,7),\qquad
\langle m\rangle^*=\frac25,\qquad
\tau_{\rm pump}=\frac1{\gamma+2R/3}=0.20\ \mathrm s.
$$

At $t=\tau_{\rm pump}$, $p_-\simeq0.1648$, while $p_0=p_+\simeq0.4176$. If the light is then switched off, relaxation returns all three populations toward $1/3$ with time constant $1/\gamma=1\ \mathrm s$. Faster optical preparation and slower dark recovery measure different combinations of rates.

In an optically thin uniform sample of $N$ atoms, with equal collection efficiency $\eta$ for each decay branch, the detected [fluorescence](fluorescence-split.md) count rate is approximately $S_{\rm fl}=\eta N R p_-$. The same scattering removes pump [photons](photon.md), giving $\Phi_{\rm out}\simeq\Phi_{\rm in}-NRp_-$ when depletion is small. For the chosen example the steady scattering rate is $R/15=0.40\ \mathrm{s}^{-1}$ per atom, compared with the initial $R/3=2\ \mathrm{s}^{-1}$. Pumping lowers this signal fivefold, while increasing transmission. If rapid mixing restores nearly uniform populations, scattering rises again. Reabsorption, strong attenuation, unequal collection efficiencies or coherent RF dynamics require a more detailed model; the reset rate $\gamma$ does not stand for an exact RF Hamiltonian.

## ↑ Ancestors (5)

1. [Optical pumping](optical-pumping.md)
2. [Atomic measurement methods](atomic-measurement-methods.md)
3. [Atomic physics](atomic-physics-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
