# Paper 304

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_304.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_304.pdf)

**Table of contents**

- [1](#1)
  - [i](#1/i)
    - [Solution](#1/i/solution)
  - [ii](#1/ii)
    - [Solution](#1/ii/solution)
  - [iii](#1/iii)
    - [Solution](#1/iii/solution)
  - [iv](#1/iv)
    - [Solution](#1/iv/solution)
- [2](#2)
  - [i](#2/i)
    - [Solution](#2/i/solution)
  - [ii](#2/ii)
    - [Solution](#2/ii/solution)
  - [iii](#2/iii)
    - [Solution](#2/iii/solution)
  - [iv](#2/iv)
    - [Solution](#2/iv/solution)
- [3](#3)
  - [Solution](#3/solution)
  - [i](#3/i)
    - [Solution](#3/i/solution)
  - [ii](#3/ii)
    - [Solution](#3/ii/solution)
  - [iii](#3/iii)
    - [Solution](#3/iii/solution)
  - [iv](#3/iv)
    - [Solution](#3/iv/solution)
  - [v](#3/v)
    - [Solution](#3/v/solution)
- [4](#4)
  - [i](#4/i)
    - [Solution](#4/i/solution)
  - [ii](#4/ii)
    - [Solution](#4/ii/solution)
  - [iii](#4/iii)
    - [Solution](#4/iii/solution)

## 1

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="1/i">i</h3>

↑ **Parent:** [1](#1)

<h4 id="1/i/solution">Solution</h4>

↑ **Parent:** [I](#1/i)

For $\omega>0$, the [quantum harmonic oscillator](../../../quantum-mechanics.md#quantum-harmonic-oscillator) has energies $E_r=\omega(r+1/2)$, $r=0,1,\ldots$, in units $\hbar=1$. For positive [inverse temperature](../../../thermodynamics.md#inverse-temperature) $\beta$, taking the [trace](../../../linear-algebra.md#matrix-trace) in the energy basis and summing a [geometric series](../../../real-analysis.md#geometric-series) gives

$$
\boxed{\mathcal Z(\omega,\beta)=\frac{e^{-\beta\omega/2}}{1-e^{-\beta\omega}}=\frac1{2\sinh(\beta\omega/2)}.}
$$

This is the [thermal partition function of a quantum harmonic oscillator](../../../quantum-mechanics.md#thermal-partition-function-of-a-quantum-harmonic-oscillator), including its [zero-point energy](../../../quantum-mechanics.md#zero-point-energy). The assumptions $\beta,\omega>0$ ensure convergence; at $\omega=0$ the free particle on the noncompact line instead has an infinite spatial-volume factor.

<h3 id="1/ii">ii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#1/ii)

The [trace](../../../linear-algebra.md#matrix-trace) of the Euclidean evolution kernel identifies its initial and final positions. Thus the [Euclidean worldline path integral](../../../quantum-field-theory.md#euclidean-worldline-path-integral) is over periodic paths $x(\tau+\beta)=x(\tau)$, with $\tau\in[0,\beta]$:

$$
\boxed{\mathcal Z=\int_{x(0)=x(\beta)}\mathcal Dx\,e^{-S_E[x]},\qquad S_E[x]=\frac12\int_0^\beta\left[\dot x^2+\omega^2x^2\right]d\tau.}
$$

The circle has circumference $\beta$, not an arbitrary unit length. The [Euclidean action](../../../perturbative-quantum-field-theory.md#euclidean-action) follows by [Wick rotation](../../../perturbative-quantum-field-theory.md#wick-rotation) of the unit-mass oscillator action. Equivalently, [integration by parts](../../../calculus.md#integration-by-parts) with [periodic boundary conditions](../../../differential-equation.md#periodic-boundary-conditions) gives $S_E=\tfrac12\langle x,L_\omega x\rangle$ for $L_\omega=-\partial_\tau^2+\omega^2$. The [path integral](../../../quantum-field-theory.md#path-integral) measure is formal until a regularization and its normalization are specified; the next part supplies a finite-dimensional version.

<h3 id="1/iii">iii</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#1/iii)

Use a real [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of [Fourier modes](../../../fourier-analysis.md#fourier-mode) on the time circle:

$$
x_N(\tau)=\frac{q_0}{\sqrt\beta}+\sqrt{\frac2\beta}\sum_{r=1}^N\left[q_r\cos(\nu_r\tau)+s_r\sin(\nu_r\tau)\right],\qquad\nu_r=\frac{2\pi r}{\beta}.
$$

The [eigenvalue](../../../linear-operator-theory.md#eigenvalue) of $L_\omega$ on the constant mode is $\omega^2$, and each sine/cosine pair has [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $\omega^2+\nu_r^2$. Retaining these modes gives

$$
S_{E,N}=\frac12\omega^2q_0^2+\frac12\sum_{r=1}^N(\omega^2+\nu_r^2)(q_r^2+s_r^2),\qquad
\mathcal D_Nx=C_N\,dq_0\prod_{r=1}^Ndq_r\,ds_r,
$$

where $C_N$ can depend on $N,\beta$ but is independent of $\omega$. Each real [Gaussian integral](../../../calculus.md#gaussian-integral) contributes $\sqrt{2\pi/\lambda_r}$. Consequently the [Fourier-cutoff oscillator functional determinant](../../../quantum-field-theory.md#fourier-cutoff-oscillator-functional-determinant) is

$$
\boxed{\mathcal Z_N=\frac{A_N}{\omega}\prod_{r=1}^N(\omega^2+\nu_r^2)^{-1},\qquad A_N=C_N(2\pi)^{N+1/2}.}
$$

A spectral cutoff between successive [eigenvalue](../../../linear-operator-theory.md#eigenvalue) pairs selects precisely this finite subspace. In comparing two frequencies, the displayed regularization keeps the same number of modes $N$; holding an absolute spectral threshold fixed need not give the same $N$ at finite cutoff.

<h3 id="1/iv">iv</h3>

↑ **Parent:** [1](#1)

<h4 id="1/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#1/iv)

The frequency-independent measure factor cancels in the ratio:

$$
R_N=\frac{\omega_2}{\omega_1}\prod_{r=1}^N\frac{1+(\beta\omega_2/(2\pi r))^2}{1+(\beta\omega_1/(2\pi r))^2}.
$$

Upon [analytic continuation](../../../complex-analysis.md#analytic-continuation) in frequency, this has [poles](../../../isolated-singularity.md#pole) at $\omega_1=0,\ \pm2\pi i r/\beta$ and zeros at $\omega_2=0,\ \pm2\pi i r/\beta$, for $1\leq r\leq N$, apart from cancellations when numerator and denominator vanish together. They match those of $\sinh(\beta\omega_2/2)/\sinh(\beta\omega_1/2)$. To justify equality, rather than merely matching this divisor, use the [hyperbolic-sine infinite product](../../../real-analysis.md#hyperbolic-sine-infinite-product)

$$
\frac{\sinh(\beta\omega/2)}{\beta\omega/2}=\prod_{r=1}^\infty\left[1+\left(\frac{\beta\omega}{2\pi r}\right)^2\right].
$$

It follows from pairing the [Weierstrass product for the reciprocal gamma function](../../../complex-analysis.md#weierstrass-product-for-the-reciprocal-gamma-function) at opposite imaginary arguments and using the [Gamma reflection formula](../../../complex-analysis.md#gamma-reflection-formula). Normal convergence on compact sets follows from $\sum r^{-2}<\infty$. Thus, for positive real frequencies,

$$
\boxed{\lim_{N\to\infty}R_N=\frac{\sinh(\beta\omega_2/2)}{\sinh(\beta\omega_1/2)}=\frac{\mathcal Z(\omega_1,\beta)}{\mathcal Z(\omega_2,\beta)}.}
$$

The cutoff ratio determines the frequency dependence, agreeing with the [thermal partition function of a quantum harmonic oscillator](../../../quantum-mechanics.md#thermal-partition-function-of-a-quantum-harmonic-oscillator).

The printed assertion about an absolute $\lim_N\mathcal Z_N$ needs a normalization qualification: independence of $A_N$ from $\omega$ alone does not ensure existence of a nonzero limit. Set $B_N=A_N\prod_{r=1}^N\nu_r^{-2}$. Then $\mathcal Z_N=B_N\omega^{-1}\prod_r(1+\omega^2/\nu_r^2)^{-1}$, so if $B_N\to B\ne0$, its limit is $B\beta/[2\sinh(\beta\omega/2)]$. The choice $B_N=1/\beta$ gives the required limit. Conversely, $B_N=(1+(-1)^N/2)/\beta$ is a positive frequency-independent normalization with no absolute limit, though every ratio above still converges. Matching zeros and poles alone also permits nonvanishing [entire functions](../../../complex-analysis.md#entire-function); the convergent normalized product is what rules them out here.

## 2

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="2/i">i</h3>

↑ **Parent:** [2](#2)

<h4 id="2/i/solution">Solution</h4>

↑ **Parent:** [I](#2/i)

The [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) $c$ and $\bar c$ are spin-zero [Grassmann fields](../../../quantum-field-theory.md#grassmann-field) in the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) of $G$; their statistics are anticommuting, despite their scalar transformation under spacetime rotations. The [Nakanishi-Lautrup field](../../../relativistic-quantum-field.md#nakanishi-lautrup-field) $h$ is an auxiliary commuting spin-zero field, also in the [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra). Thus

$$
\boxed{c,\bar c:\ (0,\ \text{Grassmann odd},\ \mathrm{ad}\,G),\qquad h:\ (0,\ \text{Grassmann even},\ \mathrm{ad}\,G).}
$$

These [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) are not physical spin-zero fermion states; they represent the gauge-fixing Jacobian, so their scalar spin does not contradict the physical [Spin-statistics theorem](../../../quantum-mechanics.md#spin-statistics-theorem).

<h3 id="2/ii">ii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#2/ii)

Write $F[A]=\partial_\mu A_\mu+iA_\mu A_\mu$ and choose the [U(1) gauge symmetry](../../../relativistic-quantum-field.md#u-1-gauge-symmetry) convention $A_\mu\mapsto A_\mu+\partial_\mu\alpha$. Its infinitesimal variation is

$$
\delta_\alpha F[A]=M_A\alpha,\qquad M_A=\partial^2+2iA_\mu\partial_\mu.
$$

A formal [BRST symmetry](../../../relativistic-quantum-field.md#brst-symmetry) construction uses $sA_\mu=\partial_\mu c$, $sc=0$, $s\bar c=ih$, $sh=0$ and the [gauge-fixing fermion](../../../relativistic-quantum-field.md#gauge-fixing-fermion) $\Psi=\int\bar c(F-i\xi h/2)\,d^4x$. Acting with the odd differential gives

$$
\boxed{S_{\mathrm{gf+gh}}=s\Psi=\int d^4x\left[ihF[A]+\frac\xi2h^2+\bar c\,\mathcal O_Ac\right],\qquad\mathcal O_A=-\partial^2-2iA\cdot\partial.}
$$

For a real admissible gauge functional, integration over $h$ gives $F^2/(2\xi)$ in the [Euclidean action](../../../perturbative-quantum-field-theory.md#euclidean-action), and $\xi\to0$ imposes the gauge condition. Overall constant phases in the [Faddeev-Popov determinant](../../../relativistic-quantum-field.md#faddeev-popov-determinant) can be absorbed in the measure convention. Here [nonlinear Abelian gauge fixing](../../../relativistic-quantum-field.md#nonlinear-abelian-gauge-fixing) makes $\mathcal O_A$ depend on $A$. The action for the [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) contains the interaction $-2i\bar cA_\mu\partial_\mu c$, so the [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) cannot be discarded as in a linear Abelian gauge, even though the $U(1)$ [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) is trivial.

There is a genuine [reality obstruction for a complex Euclidean gauge condition](../../../relativistic-quantum-field.md#reality-obstruction-for-a-complex-euclidean-gauge-condition) in the source. For a Hermitian $U(1)$ [gauge field](../../../relativistic-quantum-field.md#gauge-field), each Euclidean component $A_\mu$ is real. The real and imaginary parts of $F=0$ separately require $\partial\cdot A=0$ and $\sum_\mu A_\mu^2=0$, hence $A=0$. For example $A_2=Bx_1$, with other components zero and $B\ne0$, has curvature $F_{12}=B$; no [gauge transformation](../../../electromagnetism.md#gauge-transformation) can put it on this slice because curvature is gauge invariant. Thus the stated condition is not a [gauge fixing](../../../relativistic-quantum-field.md#gauge-fixing) of general real Euclidean configurations. The boxed action is the intended formal complex-gauge construction. A legitimate complexified contour prescription would be additional data, not an ordinary real delta-functional enforcing this printed condition.

<h3 id="2/iii">iii</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#2/iii)

A pair of [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) has a [Grassmann Gaussian integral](../../../quantum-field-theory.md#grassmann-gaussian-integral), so its functional integral contributes $\det{}'\mathcal O_A$, whereas the effective action is minus the logarithm of the partition weight. Hence its field-dependent contribution is

$$
\boxed{\Gamma_{\mathrm{gh}}[A]=-\operatorname{Tr}'\log\mathcal O_A+\operatorname{Tr}'\log\mathcal O_0.}
$$

The second term is a convenient field-independent normalization. Primes indicate removal or separate fixing of residual [zero modes in field theory](../../../relativistic-quantum-field.md#zero-mode-in-field-theory), with identical boundary and regularization conventions. The sign differs from a commuting complex scalar determinant. This is the formal contribution of the [Faddeev-Popov ghost fields](../../../relativistic-quantum-field.md#faddeev-popov-ghost) for the [complex quadratic Abelian gauge condition](../../../relativistic-quantum-field.md#complex-quadratic-abelian-gauge-condition); the real-slice obstruction established in the preceding part still applies.

<h3 id="2/iv">iv</h3>

↑ **Parent:** [2](#2)

<h4 id="2/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#2/iv)

Choose one free, massless [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field) with unit charge magnitude and bosonic statistics, minimally coupled to $A$. To fix the sign, use the conventional [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative) $D_\mu=\partial_\mu-iqA_\mu$ and take $q=-1$, so $D_\mu=\partial_\mu+iA_\mu$ and $\varphi\mapsto e^{-i\alpha}\varphi$. Its antiparticle has charge $+1$. The matter data are

$$
\boxed{m_\varphi=0,\qquad q=-1\ \text{in }D=\partial-iqA,\qquad\text{spin }0,\qquad\text{bosonic statistics}.}
$$

There is no scalar self-interaction. For real fields before formal continuation, its action is $S_\varphi=\int(D_\mu\varphi)^*(D_\mu\varphi)\,d^4x=\int\bar\varphi(-D^2)\varphi\,d^4x$, by [integration by parts](../../../calculus.md#integration-by-parts). The [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) gives the inverse [functional determinant](../../../quantum-field-theory.md#functional-determinant) and thus $\Gamma_\varphi=+\operatorname{Tr}'\log(-D^2)$, up to normalization.

The key operator identity is

$$
D^2=\partial^2+2iA\cdot\partial+i\partial\cdot A-A^2=M_A+iF[A].
$$

On the formal complex gauge slice, $-D^2=-M_A=\mathcal O_A$. With matching regulators and omitted zero modes, this gives [ghost-scalar determinant cancellation in a complex quadratic gauge](../../../relativistic-quantum-field.md#ghost-scalar-determinant-cancellation-in-a-complex-quadratic-gauge), leaving the [Maxwell action](../../../electromagnetism.md#maxwell-action) as the background functional:

$$
\boxed{\Gamma_\varphi[A]+\Gamma_{\mathrm{gh}}[A]=0,\qquad S_{\mathrm{eff}}[A]=S_{\mathrm{Maxwell}}[A]=\frac14\int F_{\mu\nu}F_{\mu\nu}\,d^4x,}
$$

where gauge-fixing terms and field-independent constants are understood separately. For a fixed background the [complex scalar field](../../../scalar-field-theory.md#complex-scalar-field) and [Faddeev-Popov ghost field](../../../relativistic-quantum-field.md#faddeev-popov-ghost) integrals are Gaussian, so this determinant cancellation is exact within the formal construction. It is a cancellation of closed bosonic matter loops against [ghost loops](../../../relativistic-quantum-field.md#ghost-loop) in that background functional. It does not prove that physical [scalar quantum electrodynamics](../../../relativistic-quantum-field.md#scalar-electrodynamics) has no radiative corrections: the printed real Euclidean gauge slice contains only $A=0$ and misses every nonzero-curvature orbit. On that literal slice the equality is trivial; a nontrivial version requires the additional complex-contour interpretation.

## 3

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The kinetic term fixes the [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) of a canonically normalized [real scalar field](../../../scalar-field-theory.md#real-scalar-field) in $d$ dimensions to $(d-2)/2$. In six dimensions $[\phi]=2$, and every term in the [Lagrangian density](../../../quantum-field-theory.md#lagrangian-density) has dimension six. Therefore $[g_n]=6-2n$, and

$$
\boxed{n<3:\ \text{relevant};\qquad n=3:\ \text{marginal};\qquad n>3:\ \text{irrelevant}.}
$$

For positive integral $n$, these mean $n=1,2$, $n=3$ and $n\ge4$, respectively. If $n=0$ is included, its vacuum-energy constant is also relevant. These are classical [power counting in quantum field theory](../../../perturbative-quantum-field-theory.md#power-counting-in-quantum-field-theory) classifications of [relevant couplings](../../../perturbative-quantum-field-theory.md#relevant-coupling), [marginal couplings](../../../perturbative-quantum-field-theory.md#marginal-coupling) and [irrelevant couplings](../../../perturbative-quantum-field-theory.md#irrelevant-coupling), not assertions that loop corrections preserve exact marginality. For the remaining parts write $g=g_3$, assume $m^2>0$ and $0<\Lambda<\Lambda_0$, and define a local quartic coupling by $\int g_4\phi^4/4!$.

<h3 id="3/i">i</h3>

↑ **Parent:** [3](#3)

<h4 id="3/i/solution">Solution</h4>

↑ **Parent:** [I](#3/i)

For a [connected Feynman diagram](../../../perturbative-quantum-field-theory.md#connected-feynman-diagram) with cubic vertices with four external legs and one loop, $3V=2I+4$ and $1=I-V+1$ give $V=I=4$. In a [one-particle-irreducible Feynman diagram](../../../perturbative-quantum-field-theory.md#one-particle-irreducible-feynman-diagram), every internal edge lies on the single cycle. Each of the four cubic vertices therefore has two internal and one external leg, giving a [box Feynman diagram](../../../perturbative-quantum-field-theory.md#box-feynman-diagram). With labelled external momenta there are three inequivalent cyclic orderings, modulo rotation and reversal, represented by $1234$, $1243$ and $1324$:

<a id="3/i/image-the-three-labelled-cubic-scalar-box-diagrams"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-304-boxes.png)

**[Figure 1](#3/i/image-the-three-labelled-cubic-scalar-box-diagrams). The three labelled cubic-scalar box diagrams**. The three inequivalent external-leg orderings of a [box Feynman diagram](../../../perturbative-quantum-field-theory.md#box-feynman-diagram) in a [six-dimensional cubic scalar field theory](../../../scalar-field-theory.md#six-dimensional-cubic-scalar-field-theory). Each square contains four internal propagators and four cubic vertices.

Take all momenta incoming with $\sum_i p_i=0$. The [Feynman rules](../../../perturbative-quantum-field-theory.md#feynman-rule) for the [Euclidean action](../../../perturbative-quantum-field-theory.md#euclidean-action) give a propagator $(q^2+m^2)^{-1}$ and a cubic insertion $-g$. For order $1234$, the amputated connected insertion is

$$
\mathcal B_{1234}=g^4\int\frac{d^6q}{(2\pi)^6}\frac{\chi(q)\chi(q+p_1)\chi(q+p_1+p_2)\chi(q-p_4)}{(q^2+m^2)((q+p_1)^2+m^2)((q+p_1+p_2)^2+m^2)((q-p_4)^2+m^2)},
$$

where $\chi(q)=\mathbf1_{\{\Lambda<|q|<\Lambda_0\}}$ is the high-mode projector for a strict [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action). Each labelled box has [Feynman-diagram symmetry factor](../../../perturbative-quantum-field-theory.md#feynman-diagram-symmetry-factor) one. A common fixed-loop-cutoff convention instead restricts only the chosen $q$ integration to the shell; both prescriptions give the same zero-external-momentum value. The effective-action vertex has the opposite sign to this connected insertion. Thus $\boxed{\text{three labelled boxes, with one cyclic topology}.}$

<h3 id="3/ii">ii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#3/ii)

The box has four external fields at all momenta. Its constant term gives $\phi^4$; the momentum-dependent terms describe a [derivative expansion of a four-point vertex](../../../perturbative-quantum-field-theory.md#derivative-expansion-of-a-four-point-vertex). With an analytic local-expansion prescription, quadratic momentum terms give operators such as $\phi^2\partial_\mu\phi\partial_\mu\phi$ or $\phi^3\partial^2\phi$, equivalent up to [integration by parts](../../../calculus.md#integration-by-parts), followed by four-field operators with more derivatives. The kernel also retains its full momentum dependence as a nonlocal four-field interaction. Therefore

$$
\boxed{\text{the same box generates four-field derivative interactions, not two- or three-field vertices}.}
$$

The latter come from different diagrams. For the strictly sharp projector on every propagator in the preceding part, moving shell boundaries can produce nonanalytic momentum dependence. The usual derivative expansion is consequently a smooth-regulator or fixed-loop-cutoff local expansion; the zero-momentum quartic coefficient calculated next does not depend on that distinction.

<h3 id="3/iii">iii</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#3/iii)

Put $I_r=\int_{\Lambda<|q|<\Lambda_0}d^6q\,(2\pi)^{-6}(q^2+m^2)^{-r}$, the [scalar shell integral in six dimensions](../../../scalar-field-theory.md#scalar-shell-integral-in-six-dimensions). Each of the three boxes is $g^4I_4$ as a connected insertion. To fix the effective-action sign and avoid a factorial ambiguity, use the [one-loop scalar effective action](../../../perturbative-quantum-field-theory.md#one-loop-scalar-effective-action):

$$
\frac12\operatorname{Tr}\log(D+g\phi)=\frac12\operatorname{Tr}\log D+\frac12\sum_{r\ge1}\frac{(-1)^{r+1}g^r}{r}\operatorname{Tr}(D^{-1}\phi)^r,\qquad D=-\partial^2+m^2.
$$

For a constant background the fourth-order density is $-g^4I_4\phi^4/8$. Thus the [cubic scalar box contribution to a quartic coupling](../../../scalar-field-theory.md#cubic-scalar-box-contribution-to-a-quartic-coupling) is $\delta g_4=-3g^4I_4$, whose vertex insertion is $-\delta g_4=+3g^4I_4$.

Using the supplied area of the unit five-sphere,

$$
I_4=\frac1{64\pi^3}\int_\Lambda^{\Lambda_0}\frac{q^5\,dq}{(q^2+m^2)^4}=\frac1{128\pi^3}\left[G(\Lambda^2+m^2)-G(\Lambda_0^2+m^2)\right],
$$

where $G(u)=u^{-1}-m^2u^{-2}+m^4/(3u^3)$. This follows by substituting $u=q^2+m^2$ and integrating $(u-m^2)^2/(2u^4)$. Hence

$$
\boxed{\delta g_4=-\frac{3g^4}{128\pi^3}\left[G(\Lambda^2+m^2)-G(\Lambda_0^2+m^2)\right].}
$$

As a check, the massless limit at positive $\Lambda$ is $-3g^4(\Lambda^{-2}-\Lambda_0^{-2})/(128\pi^3)$. Both versions have [mass dimension](../../../perturbative-quantum-field-theory.md#mass-dimension) minus two, as a six-dimensional local quartic coupling must.

<h3 id="3/iv">iv</h3>

↑ **Parent:** [3](#3)

<h4 id="3/iv/solution">Solution</h4>

↑ **Parent:** [Iv](#3/iv)

There is an interpretation issue in this clause. A proper quartic vertex, defined as the fourth derivative of the [quantum effective action](../../../perturbative-quantum-field-theory.md#effective-action), has no additional tree or reducible contribution in the bare cubic theory: the three boxes exhaust its one-loop diagrams. The strict local zero-momentum vertex of a [Wilsonian effective action](../../../perturbative-quantum-field-theory.md#wilsonian-effective-action) also has no high-mode exchange bridge, since the momentum carried by that bridge would be zero, outside the shell. Thus $\boxed{\text{for a local proper or strict Wilsonian quartic vertex, there are no additional diagrams}.}$

If “other diagrams” means the [amputated connected correlation function](../../../critical-phenomenon.md#amputated-connected-correlation-function), there are additional [one-particle-reducible Feynman diagrams](../../../perturbative-quantum-field-theory.md#one-particle-reducible-feynman-diagram). Specify full external-propagator amputation and a vacuum with [tadpole subtraction](../../../perturbative-quantum-field-theory.md#tadpole-subtraction). The three tree exchange channels each contribute $g^2/m^2$ at zero momentum. At one loop, a [triangle Feynman diagram](../../../perturbative-quantum-field-theory.md#triangle-feynman-diagram) can replace either cubic end of any exchange, giving six diagrams; a [bubble diagram](../../../perturbative-quantum-field-theory.md#bubble-diagram) can be inserted in the internal exchange line, giving three diagrams with symmetry factor $1/2$. The proper lower-point vertices at zero momentum, from the same trace-log expansion, are

$$
\Gamma^{(3)}=g+g^3I_3,\qquad\Gamma^{(2)}=m^2-\frac{g^2}{2}I_2.
$$

Therefore the reducible part of the connected four-point amplitude is

$$
\boxed{\mathcal A_{4,\mathrm{exchange}}=\frac{3g^2}{m^2}+\frac{6g^4}{m^2}I_3+\frac{3g^4}{2m^4}I_2\quad\text{to one loop}.}
$$

Adding the three boxes gives $\mathcal A_4=3g^2/m^2+3g^4I_4+6g^4I_3/m^2+3g^4I_2/(2m^4)$ in this convention. This is the [cubic-scalar exchange corrections at zero momentum](../../../perturbative-quantum-field-theory.md#cubic-scalar-exchange-corrections-at-zero-momentum) result, obtained equivalently from $\mathcal A_4=-\Gamma^{(4)}+3(\Gamma^{(3)})^2/\Gamma^{(2)}$.

If the tadpole has not been subtracted, it is an additional one-loop subgraph that must not be forgotten. The proper one-point function is $t=gI_1/2$. Its attachment to the internal exchange line gives another three reducible diagrams, contributing $3g^4I_1/(2m^6)$; equivalently the stationary background shifts by $v=-gI_1/(2m^2)$ and changes the exchanged mass by $gv$. A linear [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) enforcing $v=0$ cancels this contribution. External [self-energy](../../../perturbative-quantum-field-theory.md#self-energy) or [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram) attachments are removed by the stated full-propagator amputation; using bare external amputation would retain them instead. In that convention the four external-line decorations add $6g^4I_2/m^4+6g^4I_1/m^6$ to the displayed full-amputated result, with the $I_1$ part absent after tadpole subtraction. If the expansion is expressed in renormalized parameters, also include the corresponding [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) diagrams: replacing either cubic exchange vertex gives $6g\delta g/m^2$, and a mass insertion on the bridge gives $-3g^2\delta m^2/m^4$. A linear [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) adds $3g^3\delta h/m^6$ through the same tadpole attachment and cancels it when $\delta h=-gI_1/2$. The kinetic [counterterm](../../../perturbative-quantum-field-theory.md#counterterm) has zero insertion at zero exchanged momentum. At one loop these exhaust the possibilities: the single cycle has length four, three, two or one, corresponding respectively to box, triangle, bubble or tadpole, with tree branches attached.

The [mass dimensions](../../../perturbative-quantum-field-theory.md#mass-dimension) are $[g]=0$, $[I_r]=6-2r$, $[m]=1$. Accordingly $g^2/m^2$, $g^4I_4$, $g^4I_3/m^2$, $g^4I_2/m^4$ and $g^4I_1/m^6$ all have dimension $-2$. These connected exchanges are generally nonlocal functions of external momentum before taking the zero-momentum value; they should not be silently reclassified as an independent local quartic coupling.

<h3 id="3/v">v</h3>

↑ **Parent:** [3](#3)

<h4 id="3/v/solution">Solution</h4>

↑ **Parent:** [V](#3/v)

At fixed $m>0$ and $\Lambda>0$, the radial integrands in the [scalar shell integral in six dimensions](../../../scalar-field-theory.md#scalar-shell-integral-in-six-dimensions) behave as $q^{5-2r}$ in the ultraviolet. Thus

$$
\begin{aligned}
I_4&\longrightarrow\text{a finite limit},\\
I_3&=\frac1{64\pi^3}\log(\Lambda_0/\Lambda)+O(1),\\
I_2&=\frac{\Lambda_0^2}{128\pi^3}+O(\log\Lambda_0),\\
I_1&=\frac{\Lambda_0^4}{256\pi^3}+O(\Lambda_0^2).
\end{aligned}
$$

Consequently the proper box quartic vertex is ultraviolet finite. The reducible triangle insertion contains the logarithmic cubic-vertex divergence. The internal bubble contains the mass divergence; its nonzero-momentum expansion additionally has a logarithmic kinetic-term divergence. An unsubtracted tadpole attachment has the quartic one-point divergence and is canceled by [tadpole subtraction](../../../perturbative-quantum-field-theory.md#tadpole-subtraction), or incorporated consistently in the chosen stationary background.

These divergent lower-point subgraphs require [counterterms](../../../perturbative-quantum-field-theory.md#counterterm), not a new independent divergent $\phi^4$ coupling. More generally, cubic graph identities give the [superficial degree of divergence](../../../perturbative-quantum-field-theory.md#superficial-degree-of-divergence)

$$
D=6L-2I=6-2E,\qquad 3V=2I+E,\quad L=I-V+1.
$$

Vacuum, one-, two-, and three-point functions need vacuum-energy, linear, mass, [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization) and cubic-coupling [counterterms](../../../perturbative-quantum-field-theory.md#counterterm). Proper higher-point functions have negative superficial degree and are finite after subtraction of divergent subgraphs. Hence the [perturbative renormalizability of cubic scalar theory in six dimensions](../../../scalar-field-theory.md#perturbative-renormalizability-of-cubic-scalar-theory-in-six-dimensions) permits a continuum perturbative expansion with finitely many renormalized parameters; induced irrelevant higher-field and derivative interactions are finite predictions at finite scale, not an infinite list of ultraviolet parameters.

This perturbative statement does not establish a nonperturbative real Euclidean measure. For any nonzero real $g$, $m^2\phi^2/2+g\phi^3/6$ tends to $-\infty$ in one field direction, so even its constant-field integral is divergent. Thus $\boxed{\text{perturbatively renormalizable, with no convergent positive real Euclidean cubic measure}.}$ Stability or a specified [analytic continuation](../../../complex-analysis.md#analytic-continuation) would be additional input beyond these loop calculations.

## 4

↑ **Parent:** [Paper 304](paper-304.md)

<h3 id="4/i">i</h3>

↑ **Parent:** [4](#4)

<h4 id="4/i/solution">Solution</h4>

↑ **Parent:** [I](#4/i)

Choose Hermitian Lie-algebra generators satisfying $[T^a,T^b]=if^{abc}T^c$, with real totally antisymmetric [Lie algebra structure constants](../../../lie-algebra.md#structure-constant-of-a-lie-algebra) in an orthonormal compact-group basis. The [Adjoint representation](../../../lie-algebra.md#adjoint-representation-of-a-lie-algebra) generators are $(T^b_{\mathrm{ad}})_{ac}=-if^{bac}$. For a canonically normalized [Yang-Mills action](../../../relativistic-quantum-field.md#yang-mills-action), the coupling is in the [gauge covariant derivative](../../../relativistic-quantum-field.md#gauge-covariant-derivative), rather than an overall $1/g^2$ kinetic prefactor. The conventions $D_\mu=\partial_\mu-igA_\mu^bT^b_{\mathrm{ad}}$ give

$$
\boxed{(\not D\psi)^a=\gamma^\mu\left(\partial_\mu\psi^a+gf^{abc}A_\mu^b\psi^c\right).}
$$

Equivalently, for the Lie-algebra-valued spinor, $D_\mu\psi=\partial_\mu\psi-ig[A_\mu,\psi]$. This is the [adjoint covariant derivative](../../../relativistic-quantum-field.md#adjoint-covariant-derivative) with the Hermitian-generator and explicit-coupling convention specified. Changing the sign convention for $D$ changes the accompanying gauge-transformation convention consistently.

<h3 id="4/ii">ii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/ii/solution">Solution</h4>

↑ **Parent:** [Ii](#4/ii)

Take Euclidean [gamma matrices](../../../algebra.md#gamma-matrices) with $\{\gamma_\mu,\gamma_\nu\}=2\delta_{\mu\nu}$, and independent [Grassmann fields](../../../quantum-field-theory.md#grassmann-field) $\psi,\bar\psi$. The minimally coupled [Dirac action](../../../relativistic-quantum-field.md#dirac-action) is

$$
\boxed{S_\psi=\int d^4x\,\bar\psi^a(\gamma_\mu D_\mu+m)_{ac}\psi^c.}
$$

Its mass term is the [Dirac mass term](../../../relativistic-quantum-field.md#dirac-mass-term), and the interaction is $-ig\bar\psi^a\gamma_\mu A_\mu^b(T^b_{\mathrm{ad}})_{ac}\psi^c$. With Fourier convention $e^{ip\cdot x}$, the free kinetic operator is $i\not p+m$. The [Euclidean adjoint Dirac Feynman rules](../../../relativistic-quantum-field.md#euclidean-adjoint-dirac-feynman-rules) are therefore

$$
\boxed{S^{ac}(p)=\delta^{ac}\frac{-i\not p+m}{p^2+m^2},\qquad V_\mu^{b;ac}=+ig\gamma_\mu(T^b_{\mathrm{ad}})_{ac}=gf^{bac}\gamma_\mu.}
$$

The vertex sign follows by expanding $e^{-S_\psi}$, not $e^{iS_\psi}$. [Momentum conservation](../../../classical-mechanics.md#momentum-conservation) supplies the usual [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) at each vertex. There is only a one-gluon fermion vertex, with no two-gluon seagull because the fermionic [covariant derivative](../../../general-relativity.md#covariant-derivative) is first order. A closed fermion loop has the usual [fermionic sign](../../../perturbative-quantum-field-theory.md#fermionic-sign) $-1$. The identity $(i\not p+m)(-i\not p+m)=(p^2+m^2)I$ checks the [Dirac propagator](../../../quantum-field-theory.md#dirac-propagator).

<h3 id="4/iii">iii</h3>

↑ **Parent:** [4](#4)

<h4 id="4/iii/solution">Solution</h4>

↑ **Parent:** [Iii](#4/iii)

Write $d=4-\epsilon$ and $C_A=C_2(G)$. The pole term is independent of $m$ and external momentum beyond the transverse tensor: $\int_0^1x(1-x)\,dx=1/6$, $\Gamma(\epsilon/2)=2/\epsilon+O(1)$ and $(\mu^2/\Delta)^{\epsilon/2}=1+O(\epsilon)$. The supplied gluon [self-energy](../../../perturbative-quantum-field-theory.md#self-energy) insertion therefore has

$$
\Pi_{\mu\nu}^{ab}\big|_{\mathrm{pole}}=-\frac{8g^2C_A}{3\epsilon(4\pi)^2}\delta^{ab}(k^2\delta_{\mu\nu}-k_\mu k_\nu).
$$

Using the insertion convention $\Gamma^{(2)}_{AA}=\Gamma^{(2)}_{AA,0}-\Pi$, its cancellation requires the matter contribution $\delta Z_A=-8g^2C_A/[3\epsilon(4\pi)^2]$ to the background gauge-field kinetic factor. One can extract the coupling running from this gauge-invariant matter determinant using the [background gauge-field renormalization identity](../../../perturbative-quantum-field-theory.md#background-gauge-field-renormalization-identity) $Z_gZ_A^{1/2}=1$. This is a background-field [Ward identity](../../../perturbative-quantum-field-theory.md#ward-identity), not a claim that the ordinary quantum-gluon wave-function factor alone always determines the full coupling [renormalization](../../../perturbative-quantum-field-theory.md#renormalization). For this one adjoint [Dirac spinor](../../../relativistic-quantum-field.md#dirac-spinor),

$$
g_0=\mu^{\epsilon/2}Z_gg=\mu^{\epsilon/2}\left[g+\frac{4C_A}{3\epsilon(4\pi)^2}g^3+O(g^5)\right].
$$

Differentiate at fixed $g_0$. If $a=4C_A/[3(4\pi)^2]$ and $\beta(g)=-\epsilon g/2+b g^3+O(g^5)$, the order-$g^3$ terms in $\mu\,dg_0/d\mu=0$ give $b=a$. Subtracting $-\gamma_E+\log4\pi$ as well as the pole in the [modified minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#modified-minimal-subtraction-scheme) does not change this one-loop coefficient. Thus the [adjoint Dirac contribution to the Yang-Mills beta function](../../../perturbative-quantum-field-theory.md#adjoint-dirac-contribution-to-the-yang-mills-beta-function) is

$$
\boxed{\beta_{\mathrm{spinor}}(g)=+\frac{4C_A}{3(4\pi)^2}g^3+O(g^5)\quad(d=4).}
$$

This is screening. The [pure Yang-Mills one-loop beta function](../../../perturbative-quantum-field-theory.md#pure-yang-mills-one-loop-beta-function) coefficient is $-11C_Ag^3/[3(4\pi)^2]$. With $N_D$ adjoint [Dirac spinors](../../../relativistic-quantum-field.md#dirac-spinor), the total [renormalization-group beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics) is consequently

$$
\boxed{\beta(g)=-\frac{C_A}{3(4\pi)^2}(11-4N_D)g^3+O(g^5).}
$$

For a non-Abelian simple factor $C_A>0$, vanishing of the nontrivial one-loop coefficient would require $N_D=11/4$. It cannot be a nonnegative integer, proving the [integer obstruction to one-loop marginality with adjoint Dirac fermions](../../../perturbative-quantum-field-theory.md#integer-obstruction-to-one-loop-marginality-with-adjoint-dirac-fermions). For a product group the same argument applies to every non-Abelian factor; the statement concerns the beta-function coefficient, not the trivial fixed point $g=0$. The [modified minimal subtraction scheme](../../../perturbative-quantum-field-theory.md#modified-minimal-subtraction-scheme) is mass independent, so a massive spinor has this ultraviolet contribution; decoupling below its mass instead requires effective-theory threshold matching.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
