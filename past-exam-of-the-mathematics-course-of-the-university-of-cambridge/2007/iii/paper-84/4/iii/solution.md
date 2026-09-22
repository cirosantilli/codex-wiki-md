<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a positive uniform [number density](../../../../../../number-density.md) $n_*$ and constant [superfluid velocity](../../../../../../superfluid-velocity.md) $v\widehat{\mathbf x}$, current divergence vanishes. The stationary density equation therefore imposes $(\gamma-\Gamma n_*)n_*=0$, giving $n_*=\gamma/\Gamma$. The [quantum potential](../../../../../../quantum-potential.md) vanishes, so the phase equation sets $\mu=mv^2/2+V_0\gamma/\Gamma$. Thus the [uniform-current pumped polariton condensate](../../../../../../uniform-current-pumped-polariton-condensate.md) is

$$
\boxed{\psi(\mathbf x,t)=\sqrt{\frac\gamma\Gamma}
\exp\left[\frac{i}{\hbar}\left(mvx-
\left(\frac{mv^2}{2}+V_0\frac\gamma\Gamma\right)t\right)\right]}.
$$

Direct substitution verifies the equation: the kinetic term gives $mv^2/2$, the interaction gives $V_0\gamma/\Gamma$, and the gain-loss term is zero. A constant overall phase is arbitrary.

With the stated $\gamma,\Gamma>0$, this nonzero plane wave exists for any real $v$ and real interaction coefficient $V_0$ when $\mu$ is determined by the solution. If a particular real [chemical potential](../../../../../../chemical-potential.md) is prescribed instead, the existence condition is

$$
\boxed{\mu\ge V_0\frac\gamma\Gamma,\qquad
v=\pm\sqrt{\frac2m\left(\mu-V_0\frac\gamma\Gamma\right)}}.
$$

Equality gives the uniform condensate at rest. A nonzero density generally requires $\gamma/\Gamma>0$; a zero nonlinear-loss coefficient with positive pumping would not allow this nonzero stationary balance. The vacuum is a separate zero solution, unstable to small perturbations for positive pump.

Existence should not be confused with stability. For completeness, linearize in the comoving frame with $\psi=\psi_*[1+u+iw]$, and let $\epsilon_k=\hbar^2k^2/(2m)$. The linear real-amplitude and phase equations give

$$
\begin{pmatrix}\dot u\\\dot w\end{pmatrix}
=\frac1\hbar\begin{pmatrix}-2\gamma&\epsilon_k\\
-(\epsilon_k+2V_0n_*)&0\end{pmatrix}
\begin{pmatrix}u\\w\end{pmatrix},
$$

so

$$
\lambda(\lambda+2\gamma/\hbar)
+\epsilon_k(\epsilon_k+2V_0n_*)/\hbar^2=0.
$$

For $V_0\ge0$ both [growth rates](../../../../../../growth-rate.md) have nonpositive real parts, including the neutral uniform-phase mode. For $V_0<0$, sufficiently small nonzero $k$ makes the constant term negative, so one [growth rate](../../../../../../growth-rate.md) is positive: the plane wave still exists but is unstable in an infinite system. Uniform drift adds only a Doppler phase to these [growth rates](../../../../../../growth-rate.md) in this model.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
