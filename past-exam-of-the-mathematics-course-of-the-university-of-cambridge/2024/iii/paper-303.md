# Paper 303

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_303.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2024/Paper_303.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
    - [iv](#1/b/iv)
      - [Solution](#1/b/iv/solution)
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
    - [i](#2/e/i)
      - [Solution](#2/e/i/solution)
    - [ii](#2/e/ii)
      - [Solution](#2/e/ii/solution)
    - [iii](#2/e/iii)
      - [Solution](#2/e/iii/solution)
    - [iv](#2/e/iv)
      - [Solution](#2/e/iv/solution)
    - [v](#2/e/v)
      - [Solution](#2/e/v/solution)
- [3](#3)
  - [a](#3/a)
    - [i](#3/a/i)
      - [Solution](#3/a/i/solution)
    - [ii](#3/a/ii)
      - [Solution](#3/a/ii/solution)
    - [iii](#3/a/iii)
      - [Solution](#3/a/iii/solution)
    - [iv](#3/a/iv)
      - [Solution](#3/a/iv/solution)
    - [v](#3/a/v)
      - [Solution](#3/a/v/solution)
    - [vi](#3/a/vi)
      - [Solution](#3/a/vi/solution)
  - [b](#3/b)
    - [i](#3/b/i)
      - [Solution](#3/b/i/solution)
    - [ii](#3/b/ii)
      - [Solution](#3/b/ii/solution)
    - [iii](#3/b/iii)
      - [Solution](#3/b/iii/solution)

## 1

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

The equilibrium magnetization is a [global minimum](../../../analysis.md#global-minimum) of the [Landau free energy](../../../critical-phenomenon.md#landau-free-energy). Its stationary values solve the [polynomial equation](../../../polynomial.md#polynomial-equation)

$$
\frac{\partial f}{\partial m}=4a_4m^3+6a_6m^5-B=0,
$$

and a local minimum must satisfy

$$
\frac{\partial^2f}{\partial m^2}=12a_4m^2+30a_6m^4\geq0.
$$

One compares the value of $f$ at every such local minimum and chooses the smallest. Since $a_6>0$, the [polynomial](../../../polynomial.md) tends to positive infinity as $|m|$ tends to infinity, so a global minimum exists.

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

Put $t=T-T_c$, so $a_4\sim t$. At zero field the stationary equation factors as

$$
2m^3(2a_4+3a_6m^2)=0.
$$

For $t>0$, $m=0$ is the unique minimum. For $t<0$, it is unstable and the two minima are

$$
m_\pm=\pm\sqrt{-\frac{2a_4}{3a_6}}.
$$

The [order parameter](../../../critical-phenomenon.md#order-parameter) therefore tends continuously to zero, and its [order-parameter critical exponent](../../../critical-phenomenon.md#order-parameter-critical-exponent) is $\boxed{\beta=1/2}$.

At either ordered minimum the singular free-energy density is

$$
f_{\min}=a_4m_\pm^4+a_6m_\pm^6
=\frac{4a_4^3}{27a_6^2}\sim-|t|^3,
$$

whereas it is zero for $t>0$. Two temperature derivatives give a singular [heat capacity](../../../thermodynamics.md#heat-capacity) proportional to $|t|$ below the transition and zero above it, so the [heat-capacity critical exponent](../../../critical-phenomenon.md#heat-capacity-critical-exponent) is $\boxed{\alpha=-1}$.

The inverse [magnetic susceptibility](../../../statistical-physics.md#magnetic-susceptibility) at a stable minimum is the curvature $\chi^{-1}=\partial^2f/\partial m^2$. Below $T_c$,

$$
\chi_-^{-1}=12a_4m_\pm^2+30a_6m_\pm^4
=\frac{16a_4^2}{3a_6},
$$

and hence $\chi_-\sim|t|^{-2}$ and $\boxed{\gamma_-=2}$. Above $T_c$, however, the curvature at $m=0$ vanishes for every $t>0$. Indeed, at small field $B=4a_4m^3+O(m^5)$, so $m\sim(B/(4a_4))^{1/3}$ and the linear susceptibility is already infinite away from the critical point. Consequently the usual [magnetic-susceptibility critical exponent](../../../critical-phenomenon.md#magnetic-susceptibility-critical-exponent) $\gamma_+$ is not defined for this exceptional free energy; assigning it a finite value would incorrectly assume a quadratic term.

At $T=T_c$, the equation of state is $B=6a_6m^5$, so $m\sim|B|^{1/5}$ and the [critical-isotherm exponent](../../../critical-phenomenon.md#critical-isotherm-exponent) is $\boxed{\delta=5}$. Thus the transition is continuous, although its missing quadratic term makes the high-temperature linear response singular throughout that phase.

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

For every $T<T_c$, the two zero-field minima $m_+$ and $m_-$ coexist. A positive field selects $m_+$ and a negative field selects $m_-$, so crossing $B=0$ makes the equilibrium magnetization jump between nonzero values. Hence $B=0$, $T<T_c$, is a line of [first-order phase transitions](../../../thermodynamics.md#first-order-phase-transition), ending at the continuous critical point $(T_c,0)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

Write $\boldsymbol\sigma_i=\mathbf m+\delta\boldsymbol\sigma_i$ and neglect products of two fluctuations. Then

$$
\boldsymbol\sigma_i\cdot\boldsymbol\sigma_j
\simeq\mathbf m\cdot(\boldsymbol\sigma_i+\boldsymbol\sigma_j)-m^2.
$$

Each site has $q$ neighbours and each bond is counted once, so the [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation) gives

$$
E_{\rm MF}=-Jq\,\mathbf m\cdot\sum_i\boldsymbol\sigma_i
+\frac{NJq}{2}m^2.
$$

Choose the $x$ axis along $\mathbf m$. For the [four-state clock model](../../../statistical-physics.md#four-state-clock-model), the single-site [partition function](../../../statistical-physics.md#canonical-partition-function) is

$$
z_1=\sum_{\theta=0,\pi/2,\pi,3\pi/2}e^{\beta Jqm\cos\theta}
=2+2\cosh(\beta Jqm).
$$

Consequently

$$
f=\frac{Jq}{2}m^2-T\log[2+2\cosh(\beta Jqm)],
$$

and therefore

$$
\boxed{A=\frac{Jq}{2},\qquad C=2,\qquad D=2}.
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Differentiating the mean-field free energy and imposing stationarity gives

$$
0=Jqm-Jq\frac{\sinh(\beta Jqm)}{1+\cosh(\beta Jqm)}.
$$

The [hyperbolic-function identity](../../../calculus.md#hyperbolic-function-identity) $\sinh x/(1+\cosh x)=\tanh(x/2)$ turns this into the [self-consistency equation](../../../critical-phenomenon.md#self-consistency-equation)

$$
\boxed{m=\tanh\!\left(\frac{Jqm}{2T}\right)}.
$$

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The [Taylor series](../../../calculus.md#taylor-series) at $x=0$ is

$$
\log(2+2\cosh x)=\log4+\frac{x^2}{4}-\frac{x^4}{96}+O(x^6).
$$

Substituting $x=Jqm/T$ gives

$$
f=-T\log4+
\left(\frac{Jq}{2}-\frac{(Jq)^2}{4T}\right)m^2
+\frac{(Jq)^4}{96T^3}m^4+O(m^6).
$$

The quartic coefficient is positive, while the quadratic coefficient changes sign at

$$
\boxed{T_c=\frac{Jq}{2}}.
$$

This is therefore a continuous mean-field [phase transition](../../../critical-phenomenon.md#phase-transition).

<h4 id="1/b/iv">iv</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#1/b/iv)

For finite $p=4$, the [clock model](../../../statistical-physics.md#clock-model) has a discrete symmetry. Domain walls have finite energy per unit boundary area, so thermal disorder destroys long-range order in one dimension but a finite-temperature ordered phase can exist in two dimensions. Its [lower critical dimension](../../../critical-phenomenon.md#lower-critical-dimension) is therefore $\boxed{d_{\mathrm l}=1}$.

As $p\to\infty$, the permitted angles become continuous and the model becomes the [XY model](../../../statistical-physics.md#xy-model) with $O(2)$ symmetry. The [Mermin-Wagner theorem](../../../critical-phenomenon.md#mermin-wagner-theorem) forbids spontaneous long-range order at positive temperature in two dimensions, so the lower critical dimension for conventional symmetry breaking is $\boxed{d_{\mathrm l}=2}$. The two-dimensional model can nevertheless undergo a [Berezinskii–Kosterlitz–Thouless transition](../../../critical-phenomenon.md#berezinskii-kosterlitz-thouless-transition) between algebraic and exponential correlation decay.

## 2

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

A [momentum-shell renormalization group](../../../critical-phenomenon.md#momentum-shell-renormalization-group) step has three parts. First split the [Fourier transform](../../../analysis.md#fourier-transform) of the field into slow modes $\phi_<$ with $|k|<\Lambda/\zeta$ and fast modes $\phi_>$ with $\Lambda/\zeta<|k|<\Lambda$, then perform the [functional integral](../../../quantum-field-theory.md#functional-measure) over $\phi_>$. Second rescale momenta by $k'=\zeta k$, equivalently coordinates by $x'=x/\zeta$, to restore the cutoff from $\Lambda/\zeta$ to $\Lambda$. Third rescale the field so that the coefficient of $(\nabla\phi)^2/2$ again has its chosen normalization. The effective free energy contains every operator allowed by the symmetries, with transformed coefficients. Repeating the step composes these coefficient maps and produces a [renormalization-group flow](../../../critical-phenomenon.md#renormalization-group-flow).

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The free energy is dimensionless in units with $k_BT=1$, so the integrand has momentum dimension $d$. Since a [derivative](../../../calculus.md#derivative) has dimension one, the kinetic term gives

$$
2+2[\phi]_{\rm eng}=d,
\qquad
\boxed{[\phi]_{\rm eng}=\frac{d-2}{2}}.
$$

The mass term then gives

$$
[\mu_0^2]+2[\phi]_{\rm eng}=d,
\qquad
\boxed{[\mu_0^2]=2}.
$$

These are [engineering dimensions](../../../critical-phenomenon.md#engineering-dimension).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

The engineering value follows from the Gaussian kinetic term. At an interacting [renormalization-group fixed point](../../../critical-phenomenon.md#renormalization-group-fixed-point), momentum-dependent self-energy diagrams change the kinetic coefficient, and restoring its normalization requires [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization). The resulting [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension) $\eta$ changes the full [scaling dimension](../../../string-theory.md#scaling-dimension) to

$$
\boxed{\Delta_\phi=\frac{d-2+\eta}{2}}.
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

The operator $\nabla^{2m}\phi^{2n}$ has [engineering dimension](../../../critical-phenomenon.md#engineering-dimension)

$$
2m+2n\frac{d-2}{2}=2m+n(d-2).
$$

The action integral is dimensionless, so

$$
\boxed{[\alpha]=d-2m-n(d-2)=2n-2m-(n-1)d}.
$$

Thus $\alpha$ is a [relevant coupling](../../../perturbative-quantum-field-theory.md#relevant-coupling), [marginal coupling](../../../perturbative-quantum-field-theory.md#marginal-coupling), or [irrelevant coupling](../../../perturbative-quantum-field-theory.md#irrelevant-coupling) according as

$$
\boxed{
d<\frac{2(n-m)}{n-1},\qquad
d=\frac{2(n-m)}{n-1},\qquad
d>\frac{2(n-m)}{n-1}}
$$

respectively.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/i">i</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/i/solution">Solution</h5>

↑ **Parent:** [I](#2/e/i)

At order $g_0^2$, use the two-point [sunset diagram](../../../perturbative-quantum-field-theory.md#sunset-diagram): two quartic vertices are joined by three internal propagators, with one external line attached to each vertex. Unlike the one-vertex [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram), its self-energy $\Sigma(p)$ depends nontrivially on the external momentum $p$. The coefficient of $p^2$ in the expansion of $\Sigma(p)$ changes the kinetic term, so normalizing that term requires [wave-function renormalization](../../../perturbative-quantum-field-theory.md#wave-function-renormalization) and gives a nonzero field [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension).

<h4 id="2/e/ii">ii</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/e/ii)

**No.** With only $\lambda_0\phi^6$, the free energy has an exact [Z2 symmetry](../../../quantum-field-theory.md#z2-symmetry) $\phi\mapsto-\phi$. Integrating out fast modes and rescaling preserve that symmetry, whereas $\phi^5$ is odd. Therefore no five-point vertex and no correction to $\gamma(\zeta)$ can be generated at any order in $\lambda_0$.

<h4 id="2/e/iii">iii</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/e/iii)

Choose four of the six fields at one sextic vertex to be slow and contract the remaining two fast fields into a [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram). There are $\binom64=15$ choices. If

$$
I_1(\zeta)=\int_{\Lambda/\zeta<|q|<\Lambda}
\frac{d^dq}{(2\pi)^d}\,G_0(q),
\qquad G_0(q)=\frac1{q^2+\mu_0^2},
$$

then the first term of the [cumulant expansion](../../../probability-theory.md#cumulant-expansion) contributes

$$
15\lambda_0I_1(\zeta)\int d^dx\,\phi_<^4.
$$

After the canonical coordinate and field rescaling, its contribution to the quartic coupling is

$$
\boxed{\Delta g(\zeta)=15\,\zeta^{4-d}\lambda_0I_1(\zeta)}.
$$

<h4 id="2/e/iv">iv</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#2/e/iv)

In the displayed connected [Feynman diagram](../../../perturbative-quantum-field-theory.md#feynman-diagram), each sextic vertex carries two slow external legs and the four remaining legs at each vertex are paired across the vertices. The second [cumulant expansion](../../../probability-theory.md#cumulant-expansion) has a factor $-1/2$, the slow legs can be selected in $\binom62^2$ ways, and the four cross-contractions can be paired in $4!$ ways. The coefficient is therefore

$$
-\frac12\binom62^2 4!=-2700.
$$

Writing $\mathcal S_\zeta=\{q:\Lambda/\zeta<|q|<\Lambda\}$, the local zero-external-momentum contribution is

$$
\boxed{
\Delta g(\zeta)=-2700\,\zeta^{4-d}\lambda_0^2
\int_{\mathcal S_\zeta}\frac{d^dq_1d^dq_2d^dq_3}{(2\pi)^{3d}}
G_0(q_1)G_0(q_2)G_0(q_3)G_0(q_1+q_2+q_3)},
$$

with the integral restricted further so that $q_1+q_2+q_3\in\mathcal S_\zeta$. The three independent internal momenta agree with the diagram's [loop order](../../../perturbative-quantum-field-theory.md#loop-order) $L=4-2+1=3$.

<h4 id="2/e/v">v</h4>

↑ **Parent:** [E](#2/e)

<h5 id="2/e/v/solution">Solution</h5>

↑ **Parent:** [V](#2/e/v)

Classify the connected contractions by the numbers $(r,4-r)$ of external slow legs on the two sextic vertices and by the number $c$ of fast propagators joining them. Besides the displayed $(2,2;c=4)$ graph, the distinct topologies are:

- $(2,2;c=2)$: two joining lines and one tadpole on each vertex.
- $(1,3;c=3)$: three joining lines and one tadpole on the one-external-leg vertex.
- $(0,4;c=2)$: two joining lines and two tadpoles on the vertex with no external legs.
- $(1,3;c=1)$: one joining line, two tadpoles on the one-external-leg vertex, and one tadpole on the three-external-leg vertex.

Exchanging the two vertices gives no new topology. All four are connected [Feynman diagrams](../../../perturbative-quantum-field-theory.md#feynman-diagram) selected by the logarithm in the [cumulant expansion](../../../probability-theory.md#cumulant-expansion). With an ideal sharp momentum shell and a projection at exactly zero external momentum, the single joining line in the last topology cannot carry shell momentum, so that topology gives zero to the local quartic coupling; it is still the remaining formal connected contraction.

## 3

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/i">i</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/i/solution">Solution</h5>

↑ **Parent:** [I](#3/a/i)

When all masses are equal, the free energy depends on the real vector $\boldsymbol\phi$ only through [inner products](../../../linear-algebra.md#inner-product), so its symmetry is the [orthogonal group](../../../linear-algebra.md#orthogonal-group) $O(N)$. The mean-field potential is

$$
V(\boldsymbol\phi)=\frac12\mu_0^2\boldsymbol\phi^2+g_0(\boldsymbol\phi^2)^2.
$$

For $\mu_0^2>0$, its unique minimum is $\boldsymbol\phi=0$, which preserves $O(N)$. For $\mu_0^2<0$, the minima form the [sphere](../../../geometry-and-topology.md#sphere)

$$
\boldsymbol\phi^2=-\frac{\mu_0^2}{4g_0}.
$$

Choosing one minimum leaves the subgroup $O(N-1)$ that fixes its direction, so [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking) gives $\boxed{O(N)\to O(N-1)}$.

<h4 id="3/a/ii">ii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/a/ii)

The leading mass corrections are one-vertex [tadpole diagrams](../../../perturbative-quantum-field-theory.md#tadpole-diagram). In index notation, one contraction closes a freely summed component loop and is proportional to $N$; the two exchange contractions force the internal component to equal the external one and are not proportional to $N$. Including their multiplicities gives

$$
\Delta\mu^2=4(N+2)g_0
\int_{\Lambda/\zeta}^{\Lambda}\frac{d^dq}{(2\pi)^d}\frac1{q^2+\mu_0^2}.
$$

**Thus the $N$ in $N+2$ comes from the closed index loop, while the $2$ comes from the two same-component contractions.**

<h4 id="3/a/iii">iii</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/a/iii)

The leading quartic corrections contain two quartic vertices joined by two internal propagators: the three familiar exchange channels distribute the four external legs in the $s$, $t$, and $u$ pairings. One index contraction contains a freely summed closed component loop and is proportional to $N$; the remaining contractions have indices fixed by the external legs. Their sum gives

$$
\Delta g=-4(N+8)g_0^2
\int_{\Lambda/\zeta}^{\Lambda}\frac{d^dq}{(2\pi)^d}\frac1{(q^2+\mu_0^2)^2}.
$$

The $N$ term is the closed-index-loop topology and the eight is the combined multiplicity of the other contractions.

<h4 id="3/a/iv">iv</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/iv/solution">Solution</h5>

↑ **Parent:** [Iv](#3/a/iv)

Under $x'=x/\zeta$ and the Gaussian field rescaling $\phi'(x')=\zeta^{(d-2)/2}\phi(x)$, a mass squared has [engineering dimension](../../../critical-phenomenon.md#engineering-dimension) two and a quartic coupling has dimension $4-d$. Therefore

$$
\boxed{A=2,\qquad B=4-d}.
$$

<h4 id="3/a/v">v</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/v/solution">Solution</h5>

↑ **Parent:** [V](#3/a/v)

Let

$$
K_d=\frac{\Omega_{d-1}}{(2\pi)^d}.
$$

For a radial integrand $h(q)$, differentiating the thin shell at $\zeta=e^s$ gives

$$
\left.\frac d{ds}\int_{\Lambda e^{-s}}^\Lambda\frac{d^dq}{(2\pi)^d}h(q)\right|_{s=0}
=K_d\Lambda^dh(\Lambda).
$$

Replacing the bare parameters by running ones after each infinitesimal step yields the [beta functions](../../../complex-analysis.md#beta-function)

$$
\boxed{
\frac{d\mu^2}{ds}=2\mu^2+
4(N+2)gK_d\frac{\Lambda^d}{\Lambda^2+\mu^2}},
$$



$$
\boxed{
\frac{dg}{ds}=(4-d)g-
4(N+8)g^2K_d\frac{\Lambda^d}{(\Lambda^2+\mu^2)^2}}.
$$

<h4 id="3/a/vi">vi</h4>

↑ **Parent:** [A](#3/a)

<h5 id="3/a/vi/solution">Solution</h5>

↑ **Parent:** [Vi](#3/a/vi)

For $d=4-\epsilon$, define the dimensionless couplings $r=\mu^2/\Lambda^2$ and $u=\widetilde g=\Lambda^{-\epsilon}g$. Since $K_4=1/(8\pi^2)$, the leading [epsilon expansion](../../../critical-phenomenon.md#epsilon-expansion) of the flow is

$$
\frac{dr}{ds}=2r+4(N+2)K_4\frac{u}{1+r},
\qquad
\frac{du}{ds}=\epsilon u-4(N+8)K_4\frac{u^2}{(1+r)^2}.
$$

There is a [Gaussian fixed point](../../../critical-phenomenon.md#gaussian-fixed-point) $(r_*,u_*)=(0,0)$. Its thermal eigenvalue is $y_t=2$, so its [correlation-length critical exponent](../../../critical-phenomenon.md#correlation-length-critical-exponent) is $\boxed{\nu_{\rm G}=1/2}$.

The interacting [Wilson-Fisher fixed point](../../../critical-phenomenon.md#wilson-fisher-fixed-point) is

$$
\boxed{u_*=\frac{2\pi^2}{N+8}\epsilon+O(\epsilon^2),
\qquad
r_*=-\frac{N+2}{2(N+8)}\epsilon+O(\epsilon^2)}.
$$

Linearizing the [renormalization-group flow](../../../critical-phenomenon.md#renormalization-group-flow) gives the thermal eigenvalue

$$
y_t=2-\frac{N+2}{N+8}\epsilon+O(\epsilon^2).
$$

Taking its reciprocal gives

$$
\boxed{\nu_{\rm WF}=\frac12+\frac{N+2}{4(N+8)}\epsilon+O(\epsilon^2)}.
$$

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/i">i</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/i/solution">Solution</h5>

↑ **Parent:** [I](#3/b/i)

Write $r_a=\mu_{0,a}^2$. The stationary equations for

$$
V=\frac12r_1\phi_1^2+\frac12r_2\phi_2^2+g_0(\phi_1^2+\phi_2^2)^2
$$

are

$$
\phi_a\left[r_a+4g_0(\phi_1^2+\phi_2^2)\right]=0.
$$

For $r_1,r_2>0$, the disordered minimum is $(0,0)$. If $r_1<0$ and $r_1<r_2$, the first component orders with $\phi_1^2=-r_1/(4g_0)$ and $\phi_2=0$. If $r_2<0$ and $r_2<r_1$, the second component orders analogously.

The positive $r_2$ half of $r_1=0$ and the positive $r_1$ half of $r_2=0$ are continuous-transition lines. Along the negative diagonal $r_1=r_2<0$, the potential has an enhanced $O(2)$ symmetry and a circle of minima. Crossing that diagonal exchanges the two ordered axes and makes derivatives of the minimum free energy jump, so it is a [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition) line. The origin, where the two continuous lines meet the first-order line, is a [bicritical point](../../../thermodynamics.md#bicritical-point).

<h4 id="3/b/ii">ii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#3/b/ii)

Define the two shell [integrals](../../../calculus.md#integral)

$$
I_a(\zeta)=\int_{\Lambda/\zeta}^{\Lambda}
\frac{d^dq}{(2\pi)^d}\frac1{q^2+\mu_{0,a}^2}.
$$

For an external $\phi_1$, the $\phi_1^4$ part of the interaction gives the scalar tadpole coefficient $12g_0I_1$, while $2g_0\phi_1^2\phi_2^2$ gives $4g_0I_2$. Interchanging the components gives

$$
\boxed{
\mu_1^2(\zeta)=\zeta^2
\left[\mu_{0,1}^2+4g_0(3I_1+I_2)\right]},
$$



$$
\boxed{
\mu_2^2(\zeta)=\zeta^2
\left[\mu_{0,2}^2+4g_0(I_1+3I_2)\right]}.
$$

When the masses agree, $I_1=I_2$ and both formulas reduce to $4(N+2)g_0I_1$ with $N=2$.

<h4 id="3/b/iii">iii</h4>

↑ **Parent:** [B](#3/b)

<h5 id="3/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#3/b/iii)

**No.** Even when the two masses differ, the free energy retains an independent [Z2 symmetry](../../../quantum-field-theory.md#z2-symmetry) for each component: $\phi_1\mapsto-\phi_1$ and $\phi_2\mapsto-\phi_2$. The bilinear $\phi_1\phi_2$ is odd under either transformation, so integrating out modes cannot generate it.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2024](../../2024.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
