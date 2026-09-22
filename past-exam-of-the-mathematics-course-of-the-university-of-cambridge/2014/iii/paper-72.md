# Paper 72

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_72.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2014/paper_72.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Choose the time dependence $e^{-i\omega t}$ and measure distances in background-wavenumber units. Thus $L_0=\Delta+1$, the [incident field](../../../physics.md#incident-wave) satisfies $L_0\psi_i=0$, and the [scattering potential](../../../inverse-problem.md#scattering-potential) convention is $V=n^2-1$, giving $L_0\psi=-V\psi$. To match the minus sign in the paper's integral, take the outgoing [Green function](../../../analysis.md#green-s-function) to satisfy $L_0G=\delta$. This is the negative of the frequently used outgoing [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) fundamental solution satisfying $L_0G=-\delta$. In physical coordinates one restores $k_0^2$ in the [scattering potential](../../../inverse-problem.md#scattering-potential), or absorbs it in the integral kernel; the sign convention must remain consistent.

On a region where the incident and total fields are nonzero, introduce the [logarithmic wave perturbation](../../../inverse-problem.md#logarithmic-wave-perturbation)

$$
\psi=\psi_i e^\chi,\qquad \chi=\log(\psi/\psi_i).
$$

Choose a continuous logarithm branch connected to the unperturbed field. Substitution into the [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation) gives

$$
\mathcal L_i\chi+\nabla\chi\cdot\nabla\chi=-V,\qquad \mathcal L_i=\Delta+2\frac{\nabla\psi_i}{\psi_i}\cdot\nabla.
$$

The quadratic term uses the complex bilinear dot product, not the squared modulus of the gradient. Write $V=\varepsilon V_1$ and $\chi=\varepsilon\chi^{[1]}+\cdots$. The first-order [Rytov approximation](../../../inverse-problem.md#rytov-approximation) discards that quadratic term. Since $L_0(\psi_i\chi)=\psi_i\mathcal L_i\chi$, the outgoing first correction is

$$
\chi_1(\mathbf r)=-\frac1{\psi_i(\mathbf r)}\int G(\mathbf r,\mathbf r')V(\mathbf r')\psi_i(\mathbf r')\,d\mathbf r',
$$

and hence

$$
\boxed{\psi_1^{(R)}(\mathbf r)=\psi_i(\mathbf r)\exp\left[-\frac1{\psi_i(\mathbf r)}\int G(\mathbf r,\mathbf r')V(\mathbf r')\psi_i(\mathbf r')\,d\mathbf r'\right].}
$$

The [validity of the first Rytov approximation](../../../inverse-problem.md#validity-of-the-first-rytov-approximation) concerns the omitted logarithmic correction. Its next contribution satisfies $\mathcal L_i\chi_2=-\nabla\chi_1\cdot\nabla\chi_1$, so a useful explicit criterion is that the outgoing solution $\chi_2$ be small in the region of interest. Weak [refractive index](../../../electromagnetism.md#refractive-index) contrast and small [wave phase](../../../physics.md#phase-waves) gradients on a wavelength scale provide the usual perturbative regime, with weak [amplitude](../../../physics.md#wave-amplitude) fluctuations and no strong focusing or zeros that destroy the logarithm. A sufficient local source comparison is $|\nabla\chi_1\cdot\nabla\chi_1|\ll|V|$ where the [scattering potential](../../../inverse-problem.md#scattering-potential) is nonzero, together with control of propagation of that error. This is not a universal pointwise test at zeros of $V$.

**Small accumulated [wave phase](../../../physics.md#phase-waves) is not required in the same way as in a linear field approximation**: the exponential retains that [wave phase](../../../physics.md#phase-waves) accumulation. Large gradients, strong multiple-scattering [amplitude](../../../physics.md#wave-amplitude) effects or field zeros can still invalidate the [Rytov approximation](../../../inverse-problem.md#rytov-approximation). The integrals also require a finite scattering region or appropriate convergence conditions.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let $\delta\psi_B=\psi_1^{(B)}-\psi_i$ be the first-order scattered correction in the [Born approximation for scalar wave scattering](../../../inverse-problem.md#born-approximation-for-scalar-wave-scattering), using the paper's [Green function](../../../analysis.md#green-s-function) convention. Comparing its outgoing integral with the preceding logarithmic correction gives

$$
\chi_1=\frac{\delta\psi_B}{\psi_i}.
$$

Therefore the exact algebraic relation between the two first-order approximations is

$$
\boxed{\psi_1^{(R)}=\psi_i\exp\left(\frac{\psi_1^{(B)}-\psi_i}{\psi_i}\right)=\psi_i\exp\left(\frac{\psi_1^{(B)}}{\psi_i}-1\right).}
$$

If $V=O(\varepsilon)$, then $\chi_1=O(\varepsilon)$ on a controlled fixed region, and

$$
\psi_1^{(R)}=\psi_i(1+\chi_1)+O(\varepsilon^2)=\psi_1^{(B)}+O(\varepsilon^2).
$$

Thus **Born and Rytov agree to first order in the [scattering potential](../../../inverse-problem.md#scattering-potential)**, but differ as finite approximations. The [Rytov approximation](../../../inverse-problem.md#rytov-approximation) exponentiates the first logarithmic correction; the [Born approximation](../../../quantum-theory.md#born-approximation) adds the first field correction. The exponential's higher powers are not a calculation of all higher multiple-scattering terms in the [Born series](../../../inverse-problem.md#born-series). This distinction explains why a smooth, appreciable [wave phase](../../../physics.md#phase-waves) accumulation can be represented more naturally by the [Rytov approximation](../../../inverse-problem.md#rytov-approximation) even when the corresponding linear field expansion is inaccurate.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

Assume a real [refractive index](../../../electromagnetism.md#refractive-index) and write the [scattering potential](../../../inverse-problem.md#scattering-potential) as $V=\langle V\rangle+W$, so $\langle W\rangle=0$ by construction. With the real kernel components in the question, the logarithmic [Rytov approximation](../../../inverse-problem.md#rytov-approximation) separates into

$$
\operatorname{Re}\chi_1=-\int a(\mathbf r,\mathbf r')V(\mathbf r')\,d\mathbf r',\qquad \operatorname{Im}\chi_1=-\int b(\mathbf r,\mathbf r')V(\mathbf r')\,d\mathbf r'.
$$

Include the incident [wave phase](../../../physics.md#phase-waves) and the mean-potential [wave phase](../../../physics.md#phase-waves) in the deterministic reference $\phi_0$: at each observation point it is $\arg\psi_i-\int b\langle V\rangle$. It need not be spatially constant. The [amplitude](../../../physics.md#wave-amplitude) is $|\psi_i|\exp[-\int aV]$. The [phase covariance in the first Rytov approximation](../../../inverse-problem.md#phase-covariance-in-the-first-rytov-approximation) therefore starts from the fluctuating [wave phase](../../../physics.md#phase-waves)

$$
\boxed{\varphi(\mathbf r)=-\int b(\mathbf r,\mathbf r')W(\mathbf r')\,d\mathbf r'.}
$$

Under the integrability assumptions needed to interchange the expectation and integral,

$$
\boxed{\langle\varphi(\mathbf r)\rangle=-\int b(\mathbf r,\mathbf r')\langle W(\mathbf r')\rangle\,d\mathbf r'=0.}
$$

For a complex absorbing potential, the corresponding phase fluctuation is $-\int[b\operatorname{Re}W+a\operatorname{Im}W]$; the displayed scalar formula is the real-index case. The zero mean comes from centering $V$, not from setting the mean of $V$ equal to zero. In particular the printed $\langle n\rangle=0$ does not imply $\langle V\rangle=0$. A physical positive [refractive index](../../../electromagnetism.md#refractive-index) usually has a nonzero background mean; a zero-mean assumption normally refers to its fluctuation. The algebra above remains meaningful for a signed real random field and explicitly retains its mean [scattering potential](../../../inverse-problem.md#scattering-potential).

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Let the stationary [scattering potential](../../../inverse-problem.md#scattering-potential) fluctuation have [autocorrelation function of a random field](../../../stochastic-process.md#autocorrelation-function-of-a-random-field)

$$
C_W(\boldsymbol\rho)=\langle W(\mathbf r')W(\mathbf r'+\boldsymbol\rho)\rangle.
$$

Because $W$ is centered, this is also its [covariance function](../../../stochastic-process.md#covariance-function). Multiplying the two real [wave phase](../../../physics.md#phase-waves) integrals and taking expectations gives

$$
\boxed{\langle\varphi(\mathbf r)^2\rangle=\iint b(\mathbf r,\mathbf r')b(\mathbf r,\mathbf r'')C_W(\mathbf r''-\mathbf r')\,d\mathbf r'\,d\mathbf r''.}
$$

The two minus signs cancel. This is the [wave phase](../../../physics.md#phase-waves) [variance](../../../variance.md), since the [wave phase](../../../physics.md#phase-waves) mean is zero. More generally the [phase covariance in the first Rytov approximation](../../../inverse-problem.md#phase-covariance-in-the-first-rytov-approximation) replaces the first kernel by $b(\mathbf r_1,\mathbf r')$ and the second by $b(\mathbf r_2,\mathbf r'')$. Finite observation/scattering windows, or suitable weighted-integrability hypotheses, make these double integrals well-defined in a stationary infinite-medium model.

The correlation needed here is that of the [scattering potential](../../../inverse-problem.md#scattering-potential) fluctuation. With the printed $V=n^2-1$, the [covariance of a squared random field](../../../stochastic-process.md#covariance-of-a-squared-random-field) is

$$
C_W(\boldsymbol\rho)=\langle n(\mathbf r')^2n(\mathbf r'+\boldsymbol\rho)^2\rangle-\langle n^2\rangle^2.
$$

It involves a fourth moment of $n$, so its value is not generally determined by the ordinary two-point correlation $C_n=\langle n(\mathbf r')n(\mathbf r'+\boldsymbol\rho)\rangle$ alone. If one additionally assumes a zero-mean [Gaussian random field](../../../stochastic-process.md#gaussian-random-field), [Isserlis theorem](../../../probability-theory.md#isserlis-s-theorem) yields $C_W=2C_n^2$. That assumption is not printed and must not be inserted silently. Alternatively, for a physical weak fluctuation $n_{\rm phys}=1+\eta$, $W\simeq2\eta$ gives $C_W\simeq4C_\eta$. **The general answer uses $C_W$; either reduction to a [refractive index](../../../electromagnetism.md#refractive-index) two-point correlation requires an extra assumption.**

## 2

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Work above the surface, with $e^{-i\omega t}$ time dependence. Define the [scattered field](../../../physics.md#scattered-wave) by $\psi=\psi_i+\psi_s$, so it includes the reflection from a flat surface. For [small-height Dirichlet scattering](../../../physics.md#small-height-dirichlet-scattering), write $h=\varepsilon\eta$ and expand

$$
\psi_s=\psi_s^{[0]}+\psi_s^{[1]}+O(\varepsilon^2).
$$

The zeroth-order total field $\psi^{[0]}=\psi_i+\psi_s^{[0]}$ satisfies the [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) $\psi^{[0]}(x,0)=0$. Taylor expansion at the perturbed boundary gives

$$
0=\psi^{[0]}(x,0)+h(x)\partial_z\psi^{[0]}(x,0)+\psi_s^{[1]}(x,0)+O(\varepsilon^2).
$$

Thus the [first-order rough-surface scattered field](../../../physics.md#first-order-rough-surface-scattered-field) has mean-plane boundary data $g_1(x)=-h(x)\partial_z\psi^{[0]}(x,0)$.

Use the [outgoing angular spectrum](../../../physics.md#outgoing-angular-spectrum) to solve this boundary-value problem. For $\widehat g(q)=\int g(x)e^{-iqx}dx$, let

$$
\beta(q)=\begin{cases}\sqrt{k^2-q^2},&|q|\leq k,\\i\sqrt{q^2-k^2},&|q|>k,\end{cases}\qquad (\mathcal E g)(x,z)=\frac1{2\pi}\int\widehat g(q)e^{iqx+i\beta(q)z}dq.
$$

The branch ensures upward propagation or upward evanescent decay. Each component solves the [Helmholtz equation](../../../partial-differential-equation.md#helmholtz-equation), and $\mathcal E g$ has trace $g$ at $z=0$. Consequently

$$
\boxed{\psi_s^{[0]}=-\mathcal E[\psi_i(\cdot,0)],\qquad \psi_s^{[1]}=-\mathcal E[h\,\partial_z\psi^{[0]}(\cdot,0)].}
$$

This gives the [scattered field](../../../physics.md#scattered-wave) through first order by adding the two contributions. If one reserves “rough [scattered field](../../../physics.md#scattered-wave)” for the non-specular correction, it is $\psi_s^{[1]}$ alone; the convention here keeps the flat reflection as well.

The expansion is in height for a fixed sufficiently regular profile. The condition $|kh|\ll1$ controls the [incident wave](../../../physics.md#incident-wave)'s height expansion, but very short spatial scales can create large evanescent normal derivatives. The surface regularity and relevant spectral moments must also control the subsequent boundary expansions; small [amplitude](../../../physics.md#wave-amplitude) alone is not a uniform guarantee for arbitrarily fine roughness.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For the incident [acoustic plane wave](../../../physics.md#acoustic-plane-wave), set $q_0=k\sin\theta$ and $\beta_0=k\cos\theta>0$. The flat reflected field and total field are

$$
\psi_s^{[0]}=-e^{iq_0x+i\beta_0z},\qquad \psi^{[0]}=e^{iq_0x}(e^{-i\beta_0z}-e^{i\beta_0z}).
$$

Therefore $\partial_z\psi^{[0]}(x,0)=-2i\beta_0e^{iq_0x}$ and the [first-order rough-surface scattered field](../../../physics.md#first-order-rough-surface-scattered-field) is

$$
\psi_s^{[1]}(x,z)=\frac{2i\beta_0}{2\pi}\int\widehat h(q-q_0)e^{iqx+i\beta(q)z}dq.
$$

It is linear in the height. Since $\langle h(x)\rangle=0$, its mean vanishes, with the expectation interpreted through finite windows or stationary spectral distributions when needed. Hence

$$
\boxed{\langle\psi_s(x,z)\rangle_{\text{through first order}}=-e^{ik(x\sin\theta+z\cos\theta)}.}
$$

**The coherent first-order reflection is the flat-surface reflection.** If the field symbol is instead used only for the rough correction, its first-order mean is zero. [Stationarity](../../../time-series.md#stationary-process) ensures the coherent reflection retains the incident horizontal wavenumber, but zero mean height already explains the vanishing linear correction. The nonzero [root mean square](../../../analysis.md#root-mean-square) height does not enter this mean at first order; it does enter the fluctuating reflected field and its intensity.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For the [second-order rough-surface scattered field](../../../physics.md#second-order-rough-surface-scattered-field), the [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) expanded at the mean plane is

$$
\psi_s^{[2]}(x,0)=-h\partial_z\psi_s^{[1]}(x,0)-\frac{h^2}{2}\partial_z^2\psi^{[0]}(x,0).
$$

At normal incidence, $\psi^{[0]}=e^{-ikz}-e^{ikz}$, so its second normal derivative vanishes at zero. Define the [Dirichlet-to-Neumann map for a Helmholtz half-space](../../../partial-differential-equation.md#dirichlet-to-neumann-map-for-a-helmholtz-half-space) through the [Fourier multiplier](../../../analysis.md#fourier-multiplier) $\mathcal B$:

$$
\widehat{\mathcal B h}(q)=\beta(q)\widehat h(q),\qquad \partial_z\mathcal E g\big|_{z=0}=i\mathcal B g.
$$

The first-order trace is $2ikh$, hence $\partial_z\psi_s^{[1]}(x,0)=-2k\mathcal B h(x)$. It follows that

$$
\boxed{\psi_s(x,0)=-1+2ikh(x)+2k\,h(x)\mathcal B h(x)+O(\varepsilon^3),}
$$

where $h=O(\varepsilon)$ with fixed regular profile. In integral notation the quadratic contribution is

$$
2k\,h(x)\mathcal B h(x)=\frac{k}{\pi}h(x)\int\beta(q)\widehat h(q)e^{iqx}dq.
$$

The second-order field above the mean plane is $\mathcal E[2k h\mathcal B h]$ added to $-e^{ikz}+\mathcal E[2ikh]$. No local replacement of $\beta(q)$ by $k$ has been made; such a replacement would be an additional long-spatial-scale approximation.

The [physical surface trace and reference-plane trace](../../../physics.md#physical-surface-trace-and-reference-plane-trace) are distinct. At the actual rough boundary $z=h(x)$, the condition itself says $\psi_s(x,h(x))=-e^{-ikh(x)}$, so

$$
\boxed{\psi_s(x,h(x))=-1+ikh(x)+\frac{k^2h(x)^2}{2}+O(\varepsilon^3).}
$$

The first boxed expression is the reference-plane trace needed in part (d), at $z=0$, using the perturbative continuation where that plane lies below the actual boundary; the second answers the literal “at the surface” wording if it means the physical boundary. Taylor-expanding the first expression and its normal derivatives from $z=0$ to $z=h$ reproduces the second, so there is no contradiction between them.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Let the stationary height have [covariance function](../../../stochastic-process.md#covariance-function) $C_h(\xi)=\langle h(x)h(x+\xi)\rangle$, with $C_h(0)=\sigma^2$. Define the [power spectrum of surface height](../../../physics.md#power-spectrum-of-surface-height) by

$$
S_h(q)=\int C_h(\xi)e^{-iq\xi}d\xi,\qquad C_h(\xi)=\frac1{2\pi}\int S_h(q)e^{iq\xi}dq.
$$

For real stationary heights this spectrum is even and nonnegative. The [Fourier multiplier](../../../analysis.md#fourier-multiplier) identity in part (c) gives

$$
\langle h(x)\mathcal B h(x)\rangle=\frac1{2\pi}\int\beta(q)S_h(q)dq.
$$

Thus [coherent reflection from a stationary rough surface](../../../physics.md#coherent-reflection-from-a-stationary-rough-surface) at normal incidence is

$$
\boxed{\langle\psi_s(x,0)\rangle_{\text{through second order}}=-1+\frac{k}{\pi}\int_{\mathbb R}\beta(q)S_h(q)dq.}
$$

Require the corresponding weighted spectral moment to exist. If the stationary process has a spectral measure rather than a density, the same formula uses that measure with the matching normalization.

Splitting the propagating and evanescent parts makes the effect clear:

$$
\langle\psi_s(x,0)\rangle=-1+\frac{k}{\pi}\int_{|q|<k}\sqrt{k^2-q^2}\,S_h(q)dq+\frac{ik}{\pi}\int_{|q|>k}\sqrt{q^2-k^2}\,S_h(q)dq
$$

through second order. The positive real correction reduces the magnitude of the initially negative unit coherent reflection at this order, as some reflection becomes diffuse. The evanescent part produces a coherent [wave phase](../../../physics.md#phase-waves) correction. In contrast, the first-order mean was exactly the flat reflected wave.

The [height-correlation dependence of coherent reflection](../../../physics.md#height-correlation-dependence-of-coherent-reflection) cannot generally be determined from $\sigma$ alone: the quadratic term weights the whole spectrum by $\beta(q)$, while $\sigma^2=(2\pi)^{-1}\int S_h(q)dq$ is unweighted. If the roughness varies only on scales much longer than the wavelength, so its spectrum is concentrated at $|q|\ll k$, then $\beta\simeq k$ and

$$
\langle\psi_s(x,0)\rangle\simeq-1+2k^2\sigma^2.
$$

This is a useful limiting formula, not the general second-order answer under only small-height assumptions. Also the mean field sampled at the moving physical boundary is $-1+k^2\sigma^2/2$ through second order, from part (c), and is a different observable.

## 3

↑ **Parent:** [Paper 72](paper-72.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

For a bounded [linear operator](../../../vector-space.md#linear-operator) $A:X\to Y$ between [Hilbert spaces](../../../hilbert-space.md), let $N=\ker A$ and $R=\operatorname{ran}A$. The [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) is defined on

$$
\mathcal D(A^\dagger)=R\oplus R^\perp.
$$

For $y=Ax+z$, with $z\in R^\perp$, define

$$
\boxed{A^\dagger y=P_{N^\perp}x.}
$$

This is independent of the chosen preimage $x$, since two preimages differ by a vector in $N$. Equivalently, it is the inverse of the restriction of $A$ to $N^\perp$, applied to the component of the data in $R$, and is zero on $R^\perp$.

The generalized solution $x^\dagger=A^\dagger y$ is the unique minimum-norm [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem). Its residual is orthogonal to the range, giving the [operator normal equation](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem)

$$
\boxed{A^*Ax^\dagger=A^*y,\qquad x^\dagger\in(\ker A)^\perp.}
$$

The [operator normal equation](../../../inverse-problem.md#normal-equation-for-a-linear-inverse-problem) alone leaves an arbitrary null-space component; the second condition fixes the minimum-norm representative. The identities $A^\dagger A=P_{N^\perp}$ and $AA^\dagger=P_{\overline R}$ hold on their appropriate domains.

For an infinite-rank [compact operator](../../../compact-operator.md), the range need not be closed, and $A^\dagger$ is generally unbounded. Data outside $R\oplus R^\perp$ need not have any [least-squares solution](../../../inverse-problem.md#least-squares-solution-of-a-linear-inverse-problem) at all, even though they can be approximated by range elements. This domain qualification is crucial in part (d); the Moore–Penrose notation does not turn an ill-posed inverse into an everywhere-defined bounded operator.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

A [singular value system](../../../inverse-problem.md#singular-system-of-a-compact-operator) of a [compact operator](../../../compact-operator.md) consists of positive numbers $\sigma_j$ and orthonormal families $v_j\in X$, $u_j\in Y$ satisfying

$$
\boxed{Av_j=\sigma_j u_j,\qquad A^*u_j=\sigma_jv_j.}
$$

Thus $v_j$ are positive-eigenvalue [eigenvectors](../../../linear-operator-theory.md#eigenvector) of $A^*A$ and $u_j$ of $AA^*$, with [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\sigma_j^2$. The families are complete in $(\ker A)^\perp$ and $\overline{\operatorname{ran}A}$ respectively. The [singular values](../../../linear-algebra.md#singular-value) can be listed nonincreasingly with multiplicities, and tend to zero in the infinite-rank case. For finite rank there are only finitely many positive [singular values](../../../linear-algebra.md#singular-value); zero-kernel directions are handled separately.

Use the convention that $\langle f,g\rangle$ is conjugate-linear in its first entry. Then the [singular value system](../../../inverse-problem.md#singular-system-of-a-compact-operator) gives

$$
Ax=\sum_j\sigma_j u_j\langle v_j,x\rangle,\qquad A^\dagger y=\sum_j\frac{\langle u_j,y\rangle}{\sigma_j}v_j.
$$

The latter series converges precisely on the admissible range component specified by the [Picard criterion](../../../inverse-problem.md#picard-criterion):

$$
\sum_j\frac{|\langle u_j,y\rangle|^2}{\sigma_j^2}<\infty,
$$

with $R^\perp$ components annihilated by the inverse. Merely writing a formal singular expansion does not imply it converges in $X$.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Use the orthonormal [Fourier series](../../../fourier-series.md) basis $e_n(x)=(2\pi)^{-1/2}e^{inx}$, indexed by $n\in\mathbb Z$, and the [Hilbert space](../../../hilbert-space.md) [inner product](../../../linear-algebra.md#inner-product) $\langle f,g\rangle=\int_0^{2\pi}\overline{f(x)}g(x)dx$. The integral operator is a [periodic convolution operator](../../../fourier-analysis.md#periodic-convolution-operator). Changing variables $s=x-x'$ and using periodicity gives

$$
(Ae_n)(x)=\frac{e^{inx}}{\sqrt{2\pi}}\int_0^{2\pi}K(s)e^{-ins}ds=c_n e_n(x).
$$

There is no extra factor $2\pi$: the paper's $c_n$ already includes the full integral, rather than its normalized Fourier-series coefficient. The adjoint kernel is $\overline{K(x'-x)}$, so $A^*e_n=\overline{c_n}e_n$.

A [singular system of a periodic convolution operator](../../../inverse-problem.md#singular-system-of-a-periodic-convolution-operator) is therefore

$$
\boxed{\sigma_n=|c_n|,\qquad v_n=e_n,\qquad u_n=\frac{c_n}{|c_n|}e_n\quad(n\in\mathbb Z).}
$$

Indeed $Av_n=\sigma_nu_n$ and $A^*u_n=(c_n/|c_n|)\overline{c_n}e_n=\sigma_nv_n$. The unit factor determined by the [complex argument](../../../complex-analysis.md#argument-complex-analysis) of $c_n$ in $u_n$ is necessary when the complex [Fourier coefficients](../../../fourier-series.md#fourier-coefficient) are not positive real numbers. Both families are orthonormal and complete, since every $c_n\ne0$. One may enumerate $\mathbb Z$ by $\mathbb N$, or order the positive [singular values](../../../linear-algebra.md#singular-value) by decreasing magnitude.

The continuous kernel on a finite square makes $A$ a [Hilbert-Schmidt operator](../../../compact-operator.md#hilbert-schmidt-operator), hence compact. Since $K$ is continuously differentiable and periodic, integration by parts gives, for $n\ne0$,

$$
c_n=\frac1{in}\int_0^{2\pi}K'(s)e^{-ins}ds=o(1/|n|)
$$

by the [Riemann-Lebesgue lemma](../../../fourier-analysis.md#riemann-lebesgue-lemma). In particular the [singular values](../../../linear-algebra.md#singular-value) tend to zero. Nonzero multipliers imply both $\ker A=0$ and $\ker A^*=0$: the range is dense, but the inverse is unbounded and the range is not closed.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Let $y_n=\langle e_n,y\rangle$. Using the phase of $u_n$ in the [singular value system](../../../inverse-problem.md#singular-system-of-a-compact-operator), the [Moore–Penrose inverse of an operator](../../../inverse-problem.md#moore-penrose-inverse-of-an-operator) becomes

$$
\boxed{f^\dagger=\sum_{n\in\mathbb Z}\frac{y_n}{c_n}e_n,\qquad\sum_{n\in\mathbb Z}\frac{|y_n|^2}{|c_n|^2}<\infty.}
$$

This gives the [admissible data for a periodic convolution inverse](../../../fourier-analysis.md#admissible-data-for-a-periodic-convolution-inverse). Because the range is dense and the kernel is zero here, the domain of the inverse is exactly the range, not all of $L^2$.

For $y(x)=e^{\alpha x}$ and $\alpha\notin i\mathbb Z$,

$$
y_n=\frac1{\sqrt{2\pi}}\int_0^{2\pi}e^{(\alpha-in)x}dx=\frac{e^{2\pi\alpha}-1}{\sqrt{2\pi}(\alpha-in)}.
$$

The formal expression would consequently be

$$
f_{\rm formal}(x)=\frac{e^{2\pi\alpha}-1}{2\pi}\sum_{n\in\mathbb Z}\frac{e^{inx}}{(\alpha-in)c_n}.
$$

However, the [high-frequency obstruction for nonperiodic exponential data](../../../fourier-analysis.md#high-frequency-obstruction-for-nonperiodic-exponential-data) prevents this from being a Hilbert-space solution. The numerator is nonzero, $|y_n|$ is asymptotic to a nonzero constant divided by $|n|$, and part (c) proved $|c_n|=o(1/|n|)$. Hence $|y_n/c_n|\to\infty$, so the [Picard criterion](../../../inverse-problem.md#picard-criterion) fails. **For $\alpha\notin i\mathbb Z$, $A^\dagger y$ is not defined in the specified [Hilbert space](../../../hilbert-space.md).** The formal series is not a convergent generalized solution.

If $\alpha=im$ with $m\in\mathbb Z$, the data are a single periodic Fourier mode: $y_n=\sqrt{2\pi}\delta_{nm}$. Then there is an exact unique solution,

$$
\boxed{f^\dagger(x)=\frac{e^{imx}}{c_m}\quad\text{when }\alpha=im.}
$$

In particular, if the intended parameter is real, only $\alpha=0$ is admissible, giving $f^\dagger=1/c_0$.

For the inadmissible cases the inverse problem still has approximate solutions $f_N=\sum_{|n|\leq N}(y_n/c_n)e_n$: their images are Fourier projections converging to $y$ in $L^2$, while their [norms](../../../functional-analysis.md#norm) diverge. Thus the least-squares residual has infimum zero but no minimizer. This distinguishes an undefined exact inverse from a regularized truncated reconstruction; it is the necessary qualification to the question's unrestricted constant $\alpha$.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2014](../../2014.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
