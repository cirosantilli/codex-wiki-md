# Paper 1

↑ **Parent:** [2014](../2014.md)

[Original public PDF, physical pages 327–334](https://www.whatdotheyknow.com/request/natural_science_tripos_physics_e_2/response/2340776/attach/2/FOI%202023%20399%20Zahid%20materials.pdf?cookie_passthrough=1)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
- [5](#5)
  - [a](#5/a)
    - [Solution](#5/a/solution)
  - [b](#5/b)
    - [Solution](#5/b/solution)
  - [c](#5/c)
    - [Solution](#5/c/solution)
  - [d](#5/d)
    - [Solution](#5/d/solution)
- [6](#6)
  - [a](#6/a)
    - [Solution](#6/a/solution)
  - [b](#6/b)
    - [Solution](#6/b/solution)
  - [c](#6/c)
    - [Solution](#6/c/solution)
  - [d](#6/d)
    - [Solution](#6/d/solution)

## 1

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

An initially occupied, isolated instantaneous [energy eigenstate](../../energy-eigenvalue.md#energy-eigenstate) follows its changing eigenspace, acquiring a [dynamical phase](../../quantum-system.md#dynamical-phase) and generally a [Berry phase](../../quantum-mechanics.md#berry-phase). For smooth nondegenerate evolution, a useful local smallness condition is

$$
\boxed{\frac{\hbar|\langle m(t)|\dot H(t)|n(t)\rangle|}{|E_n(t)-E_m(t)|^2}\ll1\quad(m\ne n)}.
$$

A nonvanishing [spectral gap](../../linear-operator-theory.md#spectral-gap) and suitably smooth, slow driving throughout the evolution are needed; the local inequality alone is not a universal long-time error bound. Gap closure invalidates the simple nondegenerate approximation. A separated degenerate eigenspace may mix internally even when transitions out of it are suppressed.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Set $\vartheta_\alpha(t)=\hbar^{-1}\int^t E_\alpha(s)ds$. Differentiating the expansion produces $\dot a_\beta|\varphi_\beta\rangle+a_\beta|\dot\varphi_\beta\rangle-iE_\beta a_\beta|\varphi_\beta\rangle/\hbar$ for each term. The [energy](../../energy.md) term cancels $H|\Psi\rangle$ in the [Schrödinger equation](../../mathematical-physics.md#schrodinger-equation). Projecting the remainder with $\langle\varphi_\alpha|$ and using [orthonormality](../../inner-product.md#orthonormal-set) yields

$$
\boxed{\dot a_\alpha=-\sum_\beta\langle\varphi_\alpha|\dot\varphi_\beta\rangle a_\beta e^{i(\vartheta_\alpha-\vartheta_\beta)}}.
$$

The diagonal term is purely imaginary and supplies the [geometric phase](../../quantum-system.md#geometric-phase). Off-diagonal [instantaneous eigenstate couplings](../../quantum-theory.md#instantaneous-eigenstate-coupling) transfer population; differentiating the [eigenvalue](../../linear-operator-theory.md#eigenvalue) equation gives $\langle m|\dot n\rangle=\langle m|\dot H|n\rangle/(E_n-E_m)$ when the levels are distinct.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Use normalized instantaneous modes $\varphi_p(x,t)=\sqrt{2/L}\sin(p\pi x/L)$ and expand $\Psi=\sum_p a_pe^{-i\vartheta_p}\varphi_p$. Differentiating at fixed $x$ gives

$$
\partial_t\varphi_p=-\frac{\dot L}{2L}\varphi_p-\sqrt{\frac2L}\frac{p\pi x\dot L}{L^2}\cos(p\pi x/L).
$$

For $n\ne p$, [integration](../../integral.md) uses

$$
\int_0^1 u\sin(n\pi u)\cos(p\pi u)\,du
=-\frac{(-1)^{n+p}n}{\pi(n^2-p^2)},
$$

so the [moving-wall derivative coupling](../../quantum-mechanics.md#moving-wall-derivative-coupling) is

$$
\langle\varphi_n|\dot\varphi_p\rangle
=\frac{\dot L}{L}(-1)^{n+p}\frac{2np}{n^2-p^2}.
$$

For $n=p$ the normalization [derivative](../../calculus.md#derivative) and the remaining [integral](../../integral.md) cancel exactly, giving zero. The moving [integration](../../integral.md) endpoint contributes no boundary term because every mode vanishes there. Therefore

$$
\boxed{\dot a_n=\frac{\dot L}{L}\sum_{p\ne n}(-1)^{n+p}\frac{2np}{p^2-n^2}\,a_p e^{i(\vartheta_n-\vartheta_p)}}.
$$

The real coupling [matrix](../../vector-space.md#matrix) is antisymmetric, as required by conservation of total [probability](../../probability-theory.md#probability).

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For [first-order excitation in a linearly expanding infinite well](../../quantum-mechanics.md#first-order-excitation-in-a-linearly-expanding-infinite-well), retain only the ground-state amplitude on the right. For the second level, the coupling coefficient is $4\dot L/(3L)$. With $L=vt$,

$$
\frac{E_2-E_1}{\hbar}=\frac{\alpha}{t^2},\qquad
\alpha=\frac{3\pi^2\hbar}{2mv^2}.
$$

The relative [dynamical phase](../../quantum-system.md#dynamical-phase) is $-\alpha/t$ plus a constant. Up to an irrelevant phase,

$$
a_2(t)\simeq\frac43\int_0^t\frac{e^{-i\alpha/s}}{s}\,ds,
\qquad
\boxed{P_{1\to2}\simeq\frac{16}{9}\left|\int_0^t\frac{e^{-i\alpha/s}}s\,ds\right|^2}.
$$

The lower endpoint is an oscillatory improper limit: substituting $u=\alpha/s$ gives $\int_{\alpha/t}^\infty e^{-iu}du/u$. A physical initial state cannot occupy a zero-width well. Prepare the ground state at $t_0>0$, integrate from $t_0$, and then take the formal $t_0\downarrow0$ limit of the [probability](../../probability-theory.md#probability). For $t/\alpha\ll1$, endpoint asymptotics give $P\sim16t^2/(9\alpha^2)$; the first-order expression is reliable only while total excitation remains small.

## 2

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

The [quantum propagator](../../quantum-system.md#quantum-propagator) is the position-space kernel of the [time-evolution operator](../../quantum-system.md#time-evolution-operator): $\Psi(x,t)=\int K(x,t|x',t')\Psi(x',t')dx'$. For a time-independent [Quantum Hamiltonian](../../quantum-system.md#hamiltonian-quantum-mechanics), $U=e^{-iH(t-t')/\hbar}$. Inserting a complete orthonormal [energy](../../energy.md) eigenbasis gives

$$
\boxed{K(x,t|x',t')=\sum_\alpha\varphi_\alpha(x)\varphi_\alpha^*(x')e^{-iE_\alpha(t-t')/\hbar}}.
$$

A [continuous spectrum](../../linear-operator-theory.md#continuous-spectrum) requires the corresponding [integral](../../integral.md). At equal times, completeness makes this kernel a [Dirac delta function](../../distribution-theory.md#dirac-delta-function).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Let $I=mR^2$, $T=t-t'>0$, and $\Delta=\theta-\theta'$. Periodic angular [wave functions](../../wave-function.md) have modes $e^{il\theta}/\sqrt{2\pi}$ with integer $l$ and [energies](../../energy.md) $\hbar^2l^2/(2I)$. Normalizing the kernel with respect to $d\theta'$ gives

$$
\boxed{K_\theta(\Delta,T)=\frac1{2\pi}\sum_{l\in\mathbb Z}e^{il\Delta-i\hbar l^2T/(2I)}}.
$$

If the [integration](../../integral.md) measure is arc length $R\,d\theta'$, the corresponding kernel is $K_\theta/R$. This measure choice accounts for the otherwise ambiguous [radius](../../topology.md#radius) prefactor.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Lift the circle to its real-valued angular covering coordinate. The free classical equation is $\ddot\theta=0$. For each [winding number](../../complex-analysis.md#winding-number) $p\in\mathbb Z$, the endpoint lift is $\theta+2\pi p$, and

$$
\boxed{\theta_p(s)=\theta'+\frac{\Delta+2\pi p}{T}(s-t'),\qquad
S_p=\frac{I(\Delta+2\pi p)^2}{2T}}.
$$

Positive and negative windings are distinct [classical paths](../../quantum-field-theory.md#classical-path) with the same physical endpoints. Reducing the angle modulo $2\pi$ returns their trajectories on the ring.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The angular [action](../../lagrangian-mechanics.md#action) is $S=\int I\dot\theta^2ds/2$. In each winding sector, write $\theta=\theta_p+\xi$ with $\xi$ zero at both endpoints. The cross term vanishes and the Gaussian fluctuation [integral](../../integral.md) is the free-particle prefactor with [mass](../../classical-mechanics.md#mass) replaced by $I$. Thus

$$
\boxed{K_\theta(\Delta,T)=\sqrt{\frac{I}{2\pi i\hbar T}}\sum_{p\in\mathbb Z}\exp\left[\frac{iI(\Delta+2\pi p)^2}{2\hbar T}\right]}.
$$

Equivalently, multiply the line kernel for displacement $R(\Delta+2\pi p)$ by $R$ to change its measure from arc length to angle. The quadratic [action](../../lagrangian-mechanics.md#action) makes the classical-path sum exact, rather than merely a [stationary phase](../../analysis.md#stationary-phase-method) approximation. Real-time sums are understood with the usual negative imaginary part of $T$ and its boundary limit.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Take $\alpha=I/(i\hbar T)$ in the supplied Poisson summation identity, initially with a convergent regulator. Its left side is the winding sum. Multiplying its right side by the prefactor in part d gives

$$
\sqrt{\frac{I}{2\pi i\hbar T}}\sqrt{\frac1{2\pi\alpha}}=\frac1{2\pi},
\qquad
-\frac{q^2}{2\alpha}=-\frac{i\hbar Tq^2}{2I}.
$$

Consequently

$$
K_\theta=\frac1{2\pi}\sum_qe^{-iq\Delta-i\hbar q^2T/(2I)}.
$$

Relabelling $q=-l$ gives exactly the spectral answer. The square-root branch is fixed by continuation from positive imaginary-time damping; the limiting kernel has the required periodic delta-function normalization.

## 3

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For an interaction of finite range $b$, higher [partial waves](../../quantum-scattering.md#partial-wave) are suppressed at $kb\ll1$ by the [centrifugal barrier](../../mathematical-physics.md#centrifugal-barrier), away from exceptional higher-wave resonances. Outside the potential, the zero-energy radial [S-wave scattering](../../quantum-scattering.md#s-wave-quantum-scattering) equation is $u''=0$, where $\psi=u/r$. Its solution is proportional to $r-a$, so normalization of the constant term gives

$$
\boxed{\psi\simeq1-\frac ar}.
$$

The [scattering length](../../quantum-scattering.md#scattering-length-from-a-partial-wave-s-matrix) $a$ is the extrapolated zero of $u(r)$. At nonzero small $k$, this form applies in the overlap region $b\ll r\ll k^{-1}$; it is not the far-field limit at fixed $k$. Equivalently, $k\cot\delta_0\to-1/a$ and $f_0\to-a$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Put $d=|\mathbf r_1-\mathbf r_2|$, $g=e^{ikd}/d$ and $s_j=e^{i\mathbf k_i\cdot\mathbf r_j}$. In the range-to-wavelength overlap region around centre $j$, the outgoing wave's singular and constant terms are $c_j/(k\rho_j)+ic_j$. Matching their ratio to the [Bethe-Peierls boundary condition](../../quantum-scattering.md#bethe-peierls-boundary-condition) yields

$$
(1+ika_1)c_1+a_1g c_2=-ka_1s_1,\qquad
(1+ika_2)c_2+a_2g c_1=-ka_2s_2.
$$

Define $A_j=1+ika_j$ and $D=A_1A_2-a_1a_2g^2$. Solving the coupled system gives

$$
\boxed{c_1=-ka_1\frac{A_2s_1-a_2gs_2}{D},\qquad
c_2=-ka_2\frac{A_1s_2-a_1gs_1}{D}}.
$$

This is the [two-centre scattering-length model](../../quantum-scattering.md#two-centre-scattering-length-model) result, retaining the outgoing-wave $ik$ term and all repeated exchange between the two centres. If terms of order $ka_j$ are neglected in the local matching, set $A_1=A_2=1$ in these formulae; if also $kd\ll1$, set $g\simeq1/d$ and $s_j\simeq1$. Away from a vanishing denominator this gives $c_1\simeq-ka_1(1-a_2/d)/(1-a_1a_2/d^2)$ and its exchanged partner. The isolated-centre limit is $c_j=-ka_js_j/(1+ika_j)$. Finite-range corrections require additional effective-range data, not supplied here.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

At large $r$, $|\mathbf r-\mathbf r_j|=r-\hat{\mathbf r}\cdot\mathbf r_j+O(r^{-1})$. Retain the displacement in the phase, but replace the denominator by $r$. Therefore

$$
\boxed{f(\hat{\mathbf r})=\frac1k\left[c_1e^{-ik\hat{\mathbf r}\cdot\mathbf r_1}+c_2e^{-ik\hat{\mathbf r}\cdot\mathbf r_2}\right]}.
$$

The [differential scattering cross-section](../../quantum-scattering.md#differential-scattering-cross-section) is $|f|^2$ for [elastic scattering](../../quantum-scattering.md#elastic-scattering) with this unit incident plane-wave normalization. [interference](../../physical-optics.md#interference-wave-propagation) depends on outgoing direction and centre separation as well as the incoming phases already contained in $c_j$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Choose the polar axis along $\mathbf r_1-\mathbf r_2$. Then

$$
\int e^{-ik\hat{\mathbf r}\cdot(\mathbf r_1-\mathbf r_2)}d\Omega
=2\pi\int_{-1}^1e^{-ikdu}du=4\pi\frac{\sin(kd)}{kd}.
$$

Using the [angular interference integral for two point scatterers](../../quantum-scattering.md#angular-interference-integral-for-two-point-scatterers), integrating the two self terms and the [interference](../../physical-optics.md#interference-wave-propagation) terms gives

$$
\boxed{\sigma_{\rm tot}=\frac{4\pi}{k^2}\left[|c_1|^2+|c_2|^2+2\operatorname{Re}(c_1c_2^*)\frac{\sin(kd)}{kd}\right]}.
$$

For $kd\ll1$, the amplitudes add coherently and $\sigma\to4\pi|c_1+c_2|^2/k^2$; when $kd\gg1$ the angle-integrated [interference](../../physical-optics.md#interference-wave-propagation) is suppressed. These limits hold for fixed incoming direction; no incoming-orientation average has been silently imposed.

## 4

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

With $\beta=(k_BT)^{-1}$, the normalized canonical [density operator](../../density-matrix.md) is

$$
\boxed{\rho=\frac{e^{-\beta H}}Z,\qquad Z=\operatorname{Tr}e^{-\beta H}}.
$$

Its [eigenvalues](../../linear-operator-theory.md#eigenvalue) are the Boltzmann probabilities and its trace is one.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

The [density operator](../../density-matrix.md) is diagonal in the oscillator number basis, so $\langle a^2\rangle=\langle a^{\dagger2}\rangle=0$. With $\bar n=\langle a^\dagger a\rangle$ and $aa^\dagger=a^\dagger a+1$,

$$
\langle x^2\rangle=\frac{\hbar}{2m\omega}(2\bar n+1),\qquad
\langle p^2\rangle=\frac{m\hbar\omega}{2}(2\bar n+1).
$$

Hence

$$
\boxed{\left\langle\frac{p^2}{2m}\right\rangle
=\left\langle\frac{m\omega^2x^2}{2}\right\rangle
=\frac{\hbar\omega}{4}(2\bar n+1)}.
$$

Equality holds even at zero [temperature](../../temperature.md), when each contribution is $\hbar\omega/4$. Classical equipartition alone would miss this [zero-point energy](../../quantum-harmonic-oscillator.md#zero-point-energy).

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

Set $q=e^{-\beta\hbar\omega}$. The oscillator populations are $(1-q)q^n$, and differentiating the [geometric series](../../sequence-and-series.md#geometric-series) gives $\bar n=q/(1-q)$. The [canonical oscillator coordinate variance](../../quantum-harmonic-oscillator.md#canonical-oscillator-coordinate-variance) follows from $2\bar n+1=(1+q)/(1-q)=\coth(\beta\hbar\omega/2)$, and

$$
\boxed{\langle x^2\rangle_T=\frac{\hbar}{2m\omega}\coth\left(\frac{\hbar\omega}{2k_BT}\right)}.
$$

It approaches $\hbar/(2m\omega)$ at zero [temperature](../../temperature.md) and $k_BT/(m\omega^2)$ at high [temperature](../../temperature.md), agreeing respectively with ground-state fluctuations and classical equipartition.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

Write $T_p=p^2/(2m)$ and $V=m\omega^2x^2/2$. Dropping [commutators](../../lie-algebra.md#commutator) of order $\beta^2$ permits $e^{-\beta H}\simeq e^{-\beta V}e^{-\beta T_p}$. With $\langle x|p\rangle=e^{ipx/\hbar}/\sqrt{2\pi\hbar}$, the [momentum](../../momentum.md) Gaussian gives

$$
\langle x|e^{-\beta H}|x'\rangle\simeq
\sqrt{\frac{m}{2\pi\beta\hbar^2}}\exp\left[-\frac{m(x-x')^2}{2\beta\hbar^2}-\frac{\beta m\omega^2x^2}{2}\right].
$$

Integrating the diagonal yields $Z\simeq1/(\beta\hbar\omega)$, so the [leading high-temperature density kernel](../../density-matrix.md#leading-high-temperature-density-kernel) is

$$
\boxed{\langle x|\rho|x'\rangle\simeq
\omega\sqrt{\frac{\beta m}{2\pi}}\exp\left[-\frac{m(x-x')^2}{2\beta\hbar^2}-\frac{\beta m\omega^2x^2}{2}\right]}.
$$

This unsymmetrized product has an apparent off-diagonal asymmetry at the omitted order; reversing the product puts $x'$ in the potential factor. A manifestly [Hermitian](../../hilbert-space.md#hermitian-operator) approximation uses $e^{-\beta V/2}e^{-\beta T_p}e^{-\beta V/2}$, replacing $\beta m\omega^2x^2/2$ by $\beta m\omega^2(x^2+x'^2)/4$ with the same leading normalization. The condition is $\beta\hbar\omega\ll1$; the Gaussian off-diagonal width is of order $\hbar\sqrt{\beta/m}$.

## 5

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="5/a">a</h3>

↑ **Parent:** [5](#5)

<h4 id="5/a/solution">Solution</h4>

↑ **Parent:** [A](#5/a)

[orthogonality](../../inner-product.md#orthogonal-vectors) of angular modes makes the one-body term $\mathcal E a_1^\dagger a_1$, where

$$
\boxed{\mathcal E=\frac{\hbar^2}{2mR^2}}.
$$

The contact-interaction [integral](../../integral.md) supplies $(U/4\pi)\delta_{l_1+l_2,l_3+l_4}$, expressing [angular momentum conservation](../../momentum.md#conservation-of-angular-momentum). Within modes zero and one, the four mixed permutations each reduce to $a_1^\dagger a_0^\dagger a_0a_1$. The two remaining terms have all four indices equal. Thus

$$
H=\mathcal E N_1+\frac U{4\pi}\left[N_0(N_0-1)+N_1(N_1-1)+4N_0N_1\right].
$$

This is the projected two-mode [Quantum Hamiltonian](../../quantum-system.md#hamiltonian-quantum-mechanics); the full interaction could scatter into excluded modes, so the truncation is an assumed approximation rather than an exact invariant subspace of the complete ring problem.

<h3 id="5/b">b</h3>

↑ **Parent:** [5](#5)

<h4 id="5/b/solution">Solution</h4>

↑ **Parent:** [B](#5/b)

The occupation state is an [eigenstate](../../energy-eigenvalue.md#eigenstate) of the projected [Quantum Hamiltonian](../../quantum-system.md#hamiltonian-quantum-mechanics). Since $a_j^\dagger a_j^\dagger a_ja_j=N_j(N_j-1)$,

$$
\boxed{E_{N_0,N_1}=\mathcal E N_1+\frac U{4\pi}\left[N_0(N_0-1)+N_1(N_1-1)+4N_0N_1\right]}.
$$

Equivalently, the bracket is $N(N-1)+2N_0N_1$, where $N=N_0+N_1$; there is no self-interaction for a single particle.

<h3 id="5/c">c</h3>

↑ **Parent:** [5](#5)

<h4 id="5/c/solution">Solution</h4>

↑ **Parent:** [C](#5/c)

Put $C=\cos(\chi/2)$ and $S=\sin(\chi/2)$. Commutativity of the two [creation operators](../../quantum-harmonic-oscillator.md#creation-operator) and the [binomial theorem](../../binomial-coefficient.md#binomial-theorem) give

$$
|\chi\rangle=\sum_{j=0}^N\sqrt{\binom Nj}\,C^{N-j}S^j|N-j,j\rangle.
$$

Thus

$$
\boxed{P(N_1=j)=\binom Nj(1-p)^{N-j}p^j,\quad p=S^2},
\qquad
\boxed{\overline N_1=Np,\quad\overline N_0=N(1-p)}.
$$

The state is a [fixed-number two-mode condensate](../../quantum-ideal-gas-statistics.md#fixed-number-two-mode-condensate) with binomial mode occupations; it is not a product of two independent Poisson-distributed Glauber [coherent states](../../quantum-theory.md#coherent-state).

<h3 id="5/d">d</h3>

↑ **Parent:** [5](#5)

<h4 id="5/d/solution">Solution</h4>

↑ **Parent:** [D](#5/d)

Binomial [factorial moments](../../continuous-time-markov-chain.md#factorial-moment) give $\langle N_1(N_1-1)\rangle=N(N-1)p^2$, its mode-zero counterpart $N(N-1)(1-p)^2$, and $\langle N_0N_1\rangle=N(N-1)p(1-p)$. Consequently the exact projected expectation is

$$
\frac{E(\chi)}N=\mathcal E p+\frac{U(N-1)}{4\pi}[1+2p(1-p)].
$$

Since $p(1-p)=\sin^2\chi/4$ and $n=N/(2\pi)$,

$$
\boxed{\frac{E(\chi)}N\simeq\mathcal E\sin^2(\chi/2)+\frac{nU}{2}\left[1+\frac12\sin^2\chi\right]}.
$$

The finite-$N$ correction is simply the replacement $N\mapsto N-1$ in the interaction term. Number correlations must be retained to obtain that correction.

## 6

↑ **Parent:** [Paper 1](paper-1.md)

<h3 id="6/a">a</h3>

↑ **Parent:** [6](#6)

<h4 id="6/a/solution">Solution</h4>

↑ **Parent:** [A](#6/a)

With $J=\operatorname{diag}(1,-1)$ these matrices obey $M^\dagger JM=J$ and $\det M=1$, identifying the group as [SU(1,1)](../../lie-theory.md#su-1-1). Products preserve the displayed conjugate-entry pattern and [determinant](../../multilinear-algebra.md#determinant); the identity belongs, and

$$
M^{-1}=\begin{pmatrix}\alpha^*&-\beta\\-\beta^*&\alpha\end{pmatrix}
$$

also belongs. Multiplication and inversion are smooth. The real constraint $|\alpha|^2-|\beta|^2=1$ has nonzero gradient on its level set, so the matrices form a smooth real three-dimensional manifold. Associativity is inherited from [matrix multiplication](../../vector-space.md#matrix-multiplication). These facts establish a [Lie group](../../lie-theory.md#lie-group), which is noncompact because $|\beta|$ is unbounded.

<h3 id="6/b">b</h3>

↑ **Parent:** [6](#6)

<h4 id="6/b/solution">Solution</h4>

↑ **Parent:** [B](#6/b)

At first order write $\alpha=1+iz$ and $\beta=x+iy$ with real $x,y,z$. The constraint forces the real part of the change in $\alpha$ to vanish. Then

$$
m=\begin{pmatrix}iz&x+iy\\x-iy&-iz\end{pmatrix}
=2x\,m_1-2y\,m_2+2z\,m_3.
$$

Thus the three supplied generators span the [tangent space](../../tangent-vector.md#tangent-space) over the reals. Multiplying their matrices gives

$$
\boxed{[m_1,m_2]=m_3,\qquad[m_2,m_3]=-m_1,\qquad[m_3,m_1]=-m_2}.
$$

For example, $m_1=\sigma_x/2$, $m_2=\sigma_y/2$, $m_3=i\sigma_z/2$ makes the noncompact signs explicit.

<h3 id="6/c">c</h3>

↑ **Parent:** [6](#6)

<h4 id="6/c/solution">Solution</h4>

↑ **Parent:** [C](#6/c)

Set $P=a^\dagger b^\dagger$ and $Q=ab$. Independent [bosonic](../../tensor-product-of-quantum-systems.md#boson) [canonical commutation relations](../../quantum-mechanics.md#canonical-commutation-relation) give $[Q,P]=N_a+N_b+1=2K_3$, while $[K_3,P]=P$ and $[K_3,Q]=-Q$. Substituting $K_1=(P+Q)/2$ and $K_2=(P-Q)/(2i)$ yields

$$
[K_1,K_2]=-iK_3,\qquad[K_2,K_3]=iK_1,\qquad[K_3,K_1]=iK_2.
$$

Therefore

$$
\boxed{[iK_1,iK_2]=iK_3,\quad[iK_2,iK_3]=-iK_1,\quad[iK_3,iK_1]=-iK_2},
$$

which matches the [matrix](../../vector-space.md#matrix) [Lie algebra](../../lie-algebra.md). This [boson-pair realization of SU(1,1)](../../lie-theory.md#boson-pair-realization-of-su-1-1) differs from the number-conserving [Schwinger boson representation](../../quantum-mechanics.md#schwinger-boson-representation) of $SU(2)$.

<h3 id="6/d">d</h3>

↑ **Parent:** [6](#6)

<h4 id="6/d/solution">Solution</h4>

↑ **Parent:** [D](#6/d)

The pair products are $PQ=N_aN_b$ and $QP=(N_a+1)(N_b+1)$. Hence

$$
K_1^2+K_2^2=\frac12(PQ+QP)
=N_aN_b+\frac12(N_a+N_b+1),
$$

whereas $K_3=(N_a+N_b+1)/2$. Subtraction gives

$$
\boxed{C=\frac{(N_a-N_b)^2-1}{4}}.
$$

The number difference commutes with pair creation, pair annihilation and $K_3$, since each pair operation changes both occupations equally. Its [boson-pair Casimir operator](../../lie-theory.md#boson-pair-casimir-operator) $C$ therefore commutes with every generator. In a fixed-difference sector $N_a-N_b=d$, the Casimir [eigenvalue](../../linear-operator-theory.md#eigenvalue) is $(d^2-1)/4$, including $-1/4$ for equal occupations.

## ↑ Ancestors (12)

1. [2014](../2014.md)
2. [Past exam of the theoretical physics II course of the University of Cambridge](../../past-exam-of-the-theoretical-physics-ii-course-of-the-university-of-cambridge.md)
3. [Theoretical Physics II course of the University of Cambridge](../../university-of-cambridge.md#theoretical-physics-ii-course-of-the-university-of-cambridge)
4. [Theoretical Physics course of the University of Cambridge](../../university-of-cambridge.md#theoretical-physics-course-of-the-university-of-cambridge)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-3-of-the-natural-sciences-course-of-the-university-of-cambridge)
7. [Year of the natural sciences course of the University of Cambridge](../../university-of-cambridge.md#year-of-the-natural-sciences-course-of-the-university-of-cambridge)
8. [Natural sciences course of the University of Cambridge](../../university-of-cambridge.md#natural-sciences-course-of-the-university-of-cambridge)
9. [Course of the University of Cambridge](../../university-of-cambridge.md#course-of-the-university-of-cambridge)
10. [University of Cambridge](../../university-of-cambridge.md)
11. [List of universities](../../README.md#list-of-universities)
12. [Codex Wiki](../../README.md)
