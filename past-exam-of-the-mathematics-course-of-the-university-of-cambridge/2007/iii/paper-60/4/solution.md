<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [open-loop control](../../../../../open-loop-control.md) is computed from a dynamical model and the initial preparation, then applied without changing it in response to measurements during that run. [Controllability](../../../../../controllability.md) determines which transformations are possible in principle; field design must also account for duration, available control generators, amplitude and bandwidth limits, and calibration errors.

Three useful model-based strategies are the following. [Resonant quantum control](../../../../../resonant-quantum-control.md) chooses carrier frequencies and phases to select transitions, and uses [quantum pulse area](../../../../../quantum-pulse-area.md) or elementary [rotation gates](../../../../../rotation-gate.md) to compile the desired transformation. [Adiabatic quantum control](../../../../../adiabatic-quantum-control.md) chooses a slowly varying path of [Quantum Hamiltonians](../../../../../hamiltonian-quantum-mechanics.md) whose relevant eigenstate connects the initial and target states, maintaining a sufficiently large [spectral gap](../../../../../spectral-gap.md). [Quantum optimal control](../../../../../quantum-optimal-control.md) parametrizes or varies the fields and maximizes a fidelity or observable objective, while penalizing resources and enforcing the dynamical equations. These can all produce predetermined laboratory waveforms; experimental feedback is a separate design choice.

For a detailed variational construction, let

$$
H(u,t)=H_0+\sum_{k=1}^m u_k(t)H_k,\qquad i\hbar\dot\psi=H(u,t)\psi,\qquad\psi(0)=\psi_0.
$$

Choose a positive target observable $O$, for example $O=|\psi_d\rangle\langle\psi_d|$ for pure-state transfer. Maximize

$$
J[u]=\langle\psi(T)|O|\psi(T)\rangle-\frac12\sum_k\lambda_k\int_0^T u_k(t)^2\,dt,\qquad\lambda_k>0.
$$

The terminal term is the target probability or observable [expectation](../../../../../expected-value.md), and the quadratic integral penalizes field energy. A [costate](../../../../../costate.md) $\chi(t)$ enforces the [Schrödinger equation](../../../../../schrodinger-equation.md) through the real augmented functional

$$
\mathcal J=J-2\operatorname{Re}\int_0^T\left\langle\chi\middle|\dot\psi+\frac i\hbar H(u,t)\psi\right\rangle dt.
$$

Variation in $\chi$ recovers the state equation. Integrating the variation in $\dot\psi$ by parts gives the terminal boundary term $2\operatorname{Re}\langle O\psi(T)-\chi(T)|\delta\psi(T)\rangle$ and the interior adjoint equation. Thus the Euler-Lagrange conditions are

$$
\boxed{i\hbar\dot\psi=H\psi,\quad\psi(0)=\psi_0;\qquad i\hbar\dot\chi=H\chi,\quad\chi(T)=O\psi(T).}
$$

The [costate](../../../../../costate.md) obeys the same Hamiltonian equation but is propagated backward from its terminal value. The field variation is

$$
\delta\mathcal J=\sum_k\int_0^T\left\{\frac2\hbar\operatorname{Im}\langle\chi(t)|H_k|\psi(t)\rangle-\lambda_k u_k(t)\right\}\delta u_k(t)\,dt.
$$

Hence the [variational costate gradient for Hamiltonian quantum control](../../../../../variational-costate-gradient-for-hamiltonian-quantum-control.md) is

$$
g_k(t)=\frac{\delta J}{\delta u_k(t)}=\frac2\hbar\operatorname{Im}\langle\chi(t)|H_k|\psi(t)\rangle-\lambda_k u_k(t).
$$

At an unconstrained stationary field,

$$
\boxed{u_k(t)=\frac2{\hbar\lambda_k}\operatorname{Im}\langle\chi(t)|H_k|\psi(t)\rangle.}
$$

These equations couple forward and backward boundary data, so this is not a single initial-value integration, nor a direct feedback law for an unknown experimental state.

A practical [direct-adjoint looping](../../../../../direct-adjoint-looping.md) algorithm starts from an admissible trial field. Propagate $\psi$ forward and store its trajectory; set $\chi(T)=O\psi(T)$ and propagate $\chi$ backward; compute $g_k$ along the two trajectories; then update $u_k^{\mathrm{new}}=u_k+\eta g_k$ for a positive step size $\eta$. A line search evaluates the actual objective and decreases $\eta$ until the ascent condition is met. Project into the admissible amplitude range or optimize a finite Fourier or pulse basis to enforce bandwidth constraints. Repeat until the projected gradient and change in objective are small. Repeated initializations help explore different local optima; the stationarity equations alone do not guarantee a global optimum.

For a piecewise constant discretization, define $H_j=H_0+\sum_k u_{k,j}H_k$ and $U_j=e^{-i\Delta tH_j/\hbar}$. Forward multiplication gives the state trajectory; backward multiplication gives the [costate](../../../../../costate.md). The exact matrix-exponential derivative is

$$
\frac{\partial U_j}{\partial u_{k,j}}=-\frac i\hbar\int_0^{\Delta t}e^{-i(\Delta t-s)H_j/\hbar}H_k e^{-isH_j/\hbar}\,ds.
$$

This supplies accurate discrete gradients even when $H_j$ and $H_k$ do not commute. The small-step expression $\partial U_j/\partial u_{k,j}\simeq-i\Delta tH_kU_j/\hbar$ is only an approximation. Forward/backward factorization is the basis of [gradient ascent pulse engineering](../../../../../gradient-ascent-pulse-engineering.md). For a full-gate objective, propagate all basis columns or $U(t)$ itself and use a terminal objective such as the [phase-insensitive unitary gate error](../../../../../phase-insensitive-unitary-gate-error.md); optimizing one state alone does not implement a prescribed operation on every input.

To implement the result, convert the optimized envelope and quadratures into the calibrated electric or magnetic drive fields. An arbitrary-waveform source can set time-domain quadratures; optical [spectral pulse shaping](../../../../../spectral-pulse-shaping.md) applies a complex mask to the available pulse spectrum,

$$
\widetilde E_{\mathrm{out}}(\omega)=M(\omega)\widetilde E_{\mathrm{in}}(\omega),
$$

using, for example, a [4f pulse shaper](../../../../../4f-pulse-shaper.md) and [spatial light modulator](../../../../../spatial-light-modulator.md). Finite spectral support, mask resolution and actuator limits must be included in the optimization: smoothing an unconstrained optimum afterward may spoil it. Simulating the calibrated final pulse, optionally over an ensemble of detunings or calibration errors, checks its predicted fidelity and robustness. The computed fields are then executed as [open-loop control](../../../../../open-loop-control.md), with all measurements used for later calibration rather than an assumed instantaneous state readout.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 60](../../paper-60-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
