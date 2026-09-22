# Wave equation on a string

↑ **Parent:** [Wave equation](wave-equation-split.md)

An ideal uniform, flexible string under constant [tension](tension.md) $T>0$ has transverse displacement $y(x,t)$ satisfying

$$
\mu y_{tt}=Ty_{xx},\qquad c=\sqrt{\frac{T}{\mu}},
$$

where $\mu>0$ is [linear mass density](linear-mass-density.md), meaning mass per unit length of the straight reference string. The approximation assumes small slope $|y_x|\ll1$, transverse motion, negligible bending stiffness, negligible [damping](damping.md), and no distributed external force. Constant [tension](tension.md) and uniform [linear mass density](linear-mass-density.md) make $c$ constant. Some texts use $\rho$ for this same [linear mass density](linear-mass-density.md), giving $c=\sqrt{T/\rho}$; here $\rho$ must have units $\mathrm{kg\,m^{-1}}$, rather than units of volume [mass density](density.md). [5 Wave Equation in R](math-220a-partial-differential-equations-of-applied-mathematics/5-wave-equation-in-r.md)

The units provide a useful check: $T/\mu$ has units $(\mathrm{kg\,m\,s^{-2}})/(\mathrm{kg\,m^{-1}})=\mathrm{m^2\,s^{-2}}$. For $T=100\,\mathrm N$ and $\mu=0.010\,\mathrm{kg\,m^{-1}}$, the [wave speed](wave-speed.md) is $100\,\mathrm{m\,s^{-1}}$, so a pulse crosses a one-metre string in $0.010\,\mathrm s$. Quadrupling [tension](tension.md) doubles [wave speed](wave-speed.md); quadrupling [linear mass density](linear-mass-density.md) halves it. These square-root laws explain how material and loading set the time scale of the vibration.

For a length-$L$ string with fixed endpoints, the homogeneous [Dirichlet boundary conditions](dirichlet-boundary-condition.md) are $y(0,t)=y(L,t)=0$. Its nonzero [normal modes](normal-mode.md) have

$$
\phi_n(x)=\sin\frac{n\pi x}{L},\qquad
\omega_n=\frac{cn\pi}{L},\qquad
\nu_n=\frac{\omega_n}{2\pi}=\frac{cn}{2L},\qquad n=1,2,\ldots.
$$

Thus $cn\pi/L$ is an [angular frequency](angular-frequency.md), in radians per second, whereas $cn/(2L)$ is the [frequency](frequency.md) in hertz. The [wavelength](wavelength.md) is $2L/n$, and each [node of a standing wave](node-physics.md) lies at $x=jL/n$ for some $j=0,\ldots,n$. For the numerical string above with $L=1\,\mathrm m$, the first three [frequencies](frequency.md) are $50$, $100$ and $150\,\mathrm{Hz}$, with [angular frequencies](angular-frequency.md) $100\pi$, $200\pi$ and $300\pi\,\mathrm{s^{-1}}$. [Richard Fitzpatrick, Normal Modes of Uniform String](https://farside.ph.utexas.edu/teaching/315/Waveshtml/node28.html)

<a id="image-first-three-fixed-end-string-modes-showing-opposite-extrema-and-stationary-nodes"></a>
![](string-standing-modes.png)

**[Figure 5](#image-first-three-fixed-end-string-modes-showing-opposite-extrema-and-stationary-nodes). First three fixed-end string modes, showing opposite extrema and stationary nodes**.

Each [normal mode](normal-mode.md) is a [standing wave](standing-wave.md), but it also has a [travelling wave](travelling-wave.md) description:

$$
\sin(kx)\cos(ckt)=\frac12\sin(k(x-ct))+\frac12\sin(k(x+ct)).
$$

At a fixed endpoint an incident displacement pulse reflects with reversed sign, allowing incident and reflected displacements to cancel at the endpoint. [Periodic reflection for a fixed-end string](periodic-reflection-for-a-fixed-end-string.md) implements both endpoints through odd, $2L$-periodic extensions of the initial data. This is the bridge between moving pulses and the stationary [Fourier sine basis](fourier-sine-basis.md). [MIT, Wave Propagation, Section 2.4](https://ocw.mit.edu/courses/2-062j-wave-propagation-spring-2017/9e6f7f49eea8381d72965b469e1a3fdf_MIT2_062J_S17_Chap2.pdf)

A short derivation comes from [Newton's second law](newton-s-second-law.md). The transverse force on a small segment is approximately $T[y_x(x+\delta x,t)-y_x(x,t)]$, and its mass is $\mu\delta x$. Dividing the force balance by $\delta x$ and taking the limit gives $\mu y_{tt}=Ty_{xx}$. [Separation of variables](separation-of-variables.md) then gives $\phi''+k^2\phi=0$; the fixed-end [boundary conditions](boundary-condition.md) select $k=n\pi/L$, while the temporal equation is a [harmonic oscillator equation](simple-harmonic-motion.md) with $\omega=ck$.

**Table of contents**

- [Two-sided string data with zero slope](two-sided-string-data-with-zero-slope.md)
  - [Displacement cancellation without slope cancellation in crossing pulses](displacement-cancellation-without-slope-cancellation-in-crossing-pulses.md)
- [Free-end reflection of a transverse string wave](free-end-reflection-of-a-transverse-string-wave.md)
- [Energy flux of a transverse string wave](energy-flux-of-a-transverse-string-wave.md)
- [Driven-string endpoint power](driven-string-endpoint-power.md)
- [String with an endpoint mass](string-with-an-endpoint-mass.md)
- [Characteristic impedance of a stretched string](characteristic-impedance-of-a-stretched-string.md)
  - [Amplitude scaling along a slowly tapered string](amplitude-scaling-along-a-slowly-tapered-string.md)
  - [Viscous termination of a stretched string](viscous-termination-of-a-stretched-string.md)
  - [Reflection at a density step on a string](reflection-at-a-density-step-on-a-string.md)
  - [String density ratio for prescribed reflected power](string-density-ratio-for-prescribed-reflected-power.md)
- [Impulsively struck fixed-end string](impulsively-struck-fixed-end-string.md)
- [Modal energy of a localized velocity impulse on a string](modal-energy-of-a-localized-velocity-impulse-on-a-string.md)
- [Periodic reflection for a fixed-end string](periodic-reflection-for-a-fixed-end-string.md)
- [Linearly damped string](linearly-damped-string.md)
  - [Velocity-impulse Green function for a damped string](velocity-impulse-green-function-for-a-damped-string.md)
  - [Separated solution of the damped string equation](separated-solution-of-the-damped-string-equation.md)
  - [Energy dissipation identity for a linearly damped string](energy-dissipation-identity-for-a-linearly-damped-string.md)

## ↑ Ancestors (6)

1. [Wave equation](wave-equation-split.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (17)

- [Characteristic impedance of a stretched string](characteristic-impedance-of-a-stretched-string.md)
- [Eigenfrequency](eigenfrequency.md)
- [Fixed-end standing wave frequencies](fixed-end-standing-wave-frequencies.md)
- [Node (physics)](node-physics.md)
- [Normal mode](normal-mode.md)
- [Normal-mode energy exchange](normal-mode-energy-exchange.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-3/12h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/15b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/19/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2018/paper-2/section-b/b9/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2/section-b/b6/a/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2021/paper-2/section-b/b6/c/solution.md)
- [Standing wave phase and energy](standing-wave-phase-and-energy.md)
- [Two-sided string data with zero slope](two-sided-string-data-with-zero-slope.md)
- [Viscous termination of a stretched string](viscous-termination-of-a-stretched-string.md)
- [Wave equation](wave-equation-split.md)
- [Wave speed](wave-speed.md)
