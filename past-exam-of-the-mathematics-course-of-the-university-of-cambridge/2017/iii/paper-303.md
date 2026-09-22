# Paper 303

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_303.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2017/paper_303.pdf)

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
  - [e](#1/e)
    - [Solution](#1/e/solution)
  - [f](#1/f)
    - [Solution](#1/f/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)

## 1

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

In the [Landau theory](../../../critical-phenomenon.md#landau-theory) approximation, choose the [global minimum](../../../analysis.md#global-minimum) of the [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) as a function of the [magnetization](../../../electromagnetism.md#magnetization). Since $\mathcal A_6>0$, the [polynomial](../../../polynomial.md) is a [coercive function](../../../real-analysis.md#coercive-function) and a [global minimum](../../../analysis.md#global-minimum) exists. The candidates are [stationary points](../../../calculus-of-variations.md#stationary-point) satisfying

$$
\boxed{\mathcal A_2m+\mathcal A_4m^3+\mathcal A_6m^5=h.}
$$

Check their values of the [free-energy density](../../../statistical-physics.md#free-energy-density); a [stationary point](../../../calculus-of-variations.md#stationary-point) or a [metastable](../../../critical-phenomenon.md#metastability) [local minimum](../../../analysis.md#local-minimum) alone need not be the equilibrium state. Positive curvature $\mathcal A_2+3\mathcal A_4m^2+5\mathcal A_6m^4$ ensures local stability; when it vanishes, higher terms must be checked. The selected [global minimum](../../../analysis.md#global-minimum) is the [equilibrium magnetization](../../../critical-phenomenon.md#equilibrium-magnetization) within this approximation.

At zero [magnetic field](../../../electromagnetism.md#magnetic-field), equal opposite minima describe distinct phases exhibiting [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking). A [spontaneous magnetization](../../../statistical-physics.md#spontaneous-magnetization) is obtained by taking the [thermodynamic limit](../../../statistical-physics.md#thermodynamic-limit) before $h\to0^+$ or $h\to0^-$. A symmetric finite-volume average can instead have zero [expectation](../../../probability-theory.md#expected-value) even when the minima are nonzero. Thus one must specify the phase when interpreting the minimizer as the equilibrium [expectation](../../../probability-theory.md#expected-value).

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Discuss the zero-field phase boundaries, taking $h=0$ and writing $r=\mathcal A_2$, $q=\mathcal A_4$, $s=\mathcal A_6>0$. This qualification matters because a conjugate field generally rounds the zero-field continuous transition. Nonzero [stationary points](../../../calculus-of-variations.md#stationary-point) satisfy $r+qm^2+sm^4=0$.

For $q>0$, the [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition) occurs at

$$
\boxed{r=0,\qquad q>0.}
$$

On the $r>0$ side the only stable phase is $m=0$; on the $r<0$ side the equilibrium [global minima](../../../analysis.md#global-minimum) are $\pm m_0$ with $m_0^2\sim-r/q$. The [magnetization](../../../electromagnetism.md#magnetization) therefore grows continuously from zero as $r$ changes sign.

For $q<0$, the [first-order phase transition](../../../thermodynamics.md#first-order-phase-transition) instead occurs while $r$ is positive. At [phase coexistence](../../../critical-phenomenon.md#phase-coexistence), $m=0$ and $m=\pm m_0$ are equally deep [global minimum](../../../analysis.md#global-minimum) points. With $a=m_0^2>0$, stationarity and equality of [free energies](../../../thermodynamics.md#thermodynamic-free-energy) give

$$
r+qa+sa^2=0,\qquad \frac12ra+\frac14qa^2+\frac16sa^3=0.
$$

Eliminating $r$ gives $-qa^2/4-sa^3/3=0$, hence

$$
\boxed{m_0^2=-\frac{3\mathcal A_4}{4\mathcal A_6},\qquad \mathcal A_2=\frac{3\mathcal A_4^2}{16\mathcal A_6},\qquad \mathcal A_4<0.}
$$

At this coexistence value, the [sextic even Landau potential](../../../critical-phenomenon.md#sextic-even-landau-potential) factors as $f(m)=s m^2(m^2+3q/(4s))^2/6\geq0$. This verifies that the three equal stationary values are [global minima](../../../analysis.md#global-minimum). Above this coexistence value of $r$ the disordered phase wins; below it the ordered phase wins, with a finite jump in the phase-selected [magnetization](../../../electromagnetism.md#magnetization). The values $r=0$ and $r=q^2/(4s)$ are the disordered and ordered [spinodal points](../../../critical-phenomenon.md#spinodal-point), respectively, not the coexistence boundary: the latter follows from the repeated root of $r+qa+sa^2=0$.

The two transition loci meet at the [tricritical point](../../../critical-phenomenon.md#tricritical-point),

$$
\boxed{\mathcal A_2=\mathcal A_4=0,\qquad \mathcal A_6>0.}
$$

Two independent control parameters such as $T$ and $g$ can tune these two conditions. In a generic local phase diagram their coefficient map has a [Jacobian matrix](../../../calculus.md#jacobian-matrix) of [rank](../../../linear-algebra.md#rank-one-quadratic-form) two at the intersection; unspecified functions $\mathcal A_2(T,g)$ and $\mathcal A_4(T,g)$ do not by themselves determine the geometric orientation of the boundaries. The sextic term stabilizes this intersection and the negative-quartic first-order side.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

These are [mean-field critical exponents](../../../critical-phenomenon.md#mean-field-critical-exponent) at a [tricritical point](../../../critical-phenomenon.md#tricritical-point). Hold the other control at its tricritical value and take the coefficients to be [real analytic functions](../../../analysis.md#real-analytic-function) of [temperature](../../../thermodynamics.md#temperature) along a thermal approach with $\mathcal A_2=a(T-T_c)+o(T-T_c)$, $a>0$, $\mathcal A_6\to s>0$, and $\mathcal A_4=0$ or $\mathcal A_4=o(|\mathcal A_2|^{1/2})$. At fixed tricritical $g$, a generic [real analytic](../../../analysis.md#real-analytic-function) [temperature](../../../thermodynamics.md#temperature) path with nonzero thermal slope has $\mathcal A_4=O(T-T_c)$ and meets the last condition. Paths tangent to a scaling direction can have different apparent [temperature](../../../thermodynamics.md#temperature) powers.

At zero field on the ordered side with $\mathcal A_4=0$, stationarity gives $m^4=-\mathcal A_2/s$; under the more general approach $\mathcal A_4=o(|\mathcal A_2|^{1/2})$, this relation holds to leading order. Thus the [order-parameter critical exponent](../../../critical-phenomenon.md#order-parameter-critical-exponent) is

$$
\boxed{m\sim\left(\frac{a(T_c-T)}s\right)^{1/4},\qquad \beta=\frac14.}
$$

For the zero-quartic representative, putting this minimum into the [Landau free energy](../../../critical-phenomenon.md#landau-free-energy) gives the singular order-parameter contribution (and the leading asymptotic contribution under the stated negligible-quartic approach)

$$
f_{\rm s}=-\frac{|\mathcal A_2|^{3/2}}{3\sqrt s}.
$$

Using $C_{\rm s}=-T\,\partial_T^2f_{\rm s}$ at fixed other control yields $C_{\rm s}\sim(T_c-T)^{-1/2}$, specifically $Ta^{3/2}/(4\sqrt{s(T_c-T)})$ to leading order. Hence

$$
\boxed{\alpha=\frac12.}
$$

This [heat-capacity critical exponent](../../../critical-phenomenon.md#heat-capacity-critical-exponent) refers to the nonzero ordered-side singular amplitude; in this [mean-field approximation](../../../critical-phenomenon.md#mean-field-approximation) to [Landau theory](../../../critical-phenomenon.md#landau-theory), the disordered [global minimum](../../../analysis.md#global-minimum) contributes zero singular [free energy](../../../thermodynamics.md#thermodynamic-free-energy), while any regular background remains. Fluctuation corrections lie outside the present approximation.

In the disordered phase, differentiating the equation of state at $m=h=0$ gives the [magnetic susceptibility](../../../statistical-physics.md#magnetic-susceptibility) $\chi=1/\mathcal A_2$. On the ordered branch its curvature is $\mathcal A_2+5sm^4=4|\mathcal A_2|$, so $\chi=1/(4|\mathcal A_2|)$. Both give the [magnetic-susceptibility critical exponent](../../../critical-phenomenon.md#magnetic-susceptibility-critical-exponent)

$$
\boxed{\gamma=1.}
$$

At the tricritical [temperature](../../../thermodynamics.md#temperature) with both lower coefficients zero, $h=sm^5$, so $m=\operatorname{sgn}(h)(|h|/s)^{1/5}$ and the [critical-isotherm exponent](../../../critical-phenomenon.md#critical-isotherm-exponent) is

$$
\boxed{\delta=5,\qquad (\alpha,\beta,\gamma,\delta)=\left(\frac12,\frac14,1,5\right).}
$$

The [Widom scaling relation](../../../critical-phenomenon.md#widom-scaling-relation) $\gamma=\beta(\delta-1)$ and [Rushbrooke scaling relation](../../../critical-phenomenon.md#rushbrooke-scaling-relation) $\alpha+2\beta+\gamma=2$ both check these powers. Their validity here is a mean-field conclusion, not a claim that fluctuations in every spatial dimension preserve them.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $\mathcal A_2\ne0$, rescale the [order parameter](../../../critical-phenomenon.md#order-parameter) by $m=(|\mathcal A_2|/\mathcal A_6)^{1/4}\psi$. Write $\sigma=\operatorname{sgn}\mathcal A_2$ and introduce dimensionless scaling variables

$$
X=\frac{\mathcal A_4}{|\mathcal A_2|^{1/2}\mathcal A_6^{1/2}},\qquad Y=\frac{h\mathcal A_6^{1/4}}{|\mathcal A_2|^{5/4}}.
$$

Every term then has the common energy-density factor $|\mathcal A_2|^{3/2}/\mathcal A_6^{1/2}$:

$$
\mathcal A=\frac{|\mathcal A_2|^{3/2}}{\mathcal A_6^{1/2}}\left(\frac\sigma2\psi^2+\frac X4\psi^4+\frac16\psi^6-Y\psi\right).
$$

Minimizing over $\psi$ defines the [tricritical crossover scaling](../../../critical-phenomenon.md#tricritical-crossover-scaling) functions

$$
\Phi_\sigma(X,Y)=\min_{\psi\in\mathbb R}\left(\frac\sigma2\psi^2+\frac X4\psi^4+\frac16\psi^6-Y\psi\right).
$$

For the minimized potential, following the paper's notation $\mathcal F$, this proves

$$
\boxed{(u,v,w,x,y,z)=\left(\frac32,\frac12,\frac12,\frac12,\frac14,\frac54\right).}
$$

The exponent names $x,y$ here are unrelated to the couplings in question 2. The expression concerns the specified order-parameter [polynomial](../../../polynomial.md); a general material can also have a smooth, field-independent background [free-energy density](../../../statistical-physics.md#free-energy-density). Such a background should be separated before writing a homogeneous singular scaling form. A potential at prescribed [magnetization](../../../electromagnetism.md#magnetization), instead of prescribed field, is a different [Legendre transform](../../../convex-optimization.md#convex-conjugate) and is not obtained by this minimization.

There is a needed qualification to the printed single $\Phi$ and nonzero-value condition. At $(X,Y)=(0,0)$, the ordered branch has minimizers $\psi=\pm1$ and $\Phi_-(0,0)=-1/3$, whereas the disordered branch has minimizer zero and $\Phi_+(0,0)=0$. Thus

$$
\boxed{\Phi_-(0,0)=-\frac13,\qquad \Phi_+(0,0)=0.}
$$

For example, $\mathcal A_2>0$, $\mathcal A_4=h=0$ gives an identically zero minimized [polynomial](../../../polynomial.md), contradicting a nonzero $\Phi(0,0)$ on that side. The valid scaling statement uses separate sign branches, or restricts the asserted nonzero value to approach from the ordered side. At $\mathcal A_2=0$ the displayed coordinates are singular; the critical isotherm is obtained as a limit or directly from the equation of state.

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

At an ordinary zero-field [continuous phase transition](../../../critical-phenomenon.md#continuous-phase-transition), the positive quartic coefficient remains nonzero while $\mathcal A_2\to0$. Approaching from the ordered side therefore sends the variable $X$ in the [tricritical crossover scaling](../../../critical-phenomenon.md#tricritical-crossover-scaling) form to $+\infty$, rather than to zero. With $Y=0$ the dimensionless minimizer obeys $\psi^4+X\psi^2-1=0$, so

$$
\psi^2=\frac{\sqrt{X^2+4}-X}{2}\sim X^{-1}.
$$

At that stationary point, substitution gives $\Phi_-(X,0)=-\psi^2/4-\psi^6/12$. Its [large-quartic asymptotic of tricritical scaling](../../../critical-phenomenon.md#large-quartic-asymptotic-of-tricritical-scaling) is consequently $\Phi_-(X,0)\sim-1/(4X)$, and

$$
f_{\rm s}\sim-\frac{|\mathcal A_2|^{3/2}}{4\sqrt{\mathcal A_6}X}=-\frac{\mathcal A_2^2}{4\mathcal A_4}.
$$

If $\mathcal A_2$ crosses zero linearly with [temperature](../../../thermodynamics.md#temperature), this is quadratic in $T-T_c$, giving a finite [heat capacity](../../../thermodynamics.md#heat-capacity) jump rather than a power divergence. Therefore

$$
\boxed{\alpha=0.}
$$

For locally constant $\mathcal A_4>0$ and slope $a=\partial_T\mathcal A_2|_{T_c}$, the leading singular [heat capacity](../../../thermodynamics.md#heat-capacity) jump from this term is $\Delta C=T_ca^2/(2\mathcal A_4)$. Treating $\Phi$ as a nonzero constant while $X\to\infty$ would incorrectly assign the tricritical exponent to this ordinary transition.

<h3 id="1/f">f</h3>

↑ **Parent:** [1](#1)

<h4 id="1/f/solution">Solution</h4>

↑ **Parent:** [F](#1/f)

On a tricritical thermal path, the quartic scaling variable $X$ tends to zero, and at zero field $Y=0$. On the ordered side the [tricritical crossover scaling](../../../critical-phenomenon.md#tricritical-crossover-scaling) function tends to $\Phi_-(0,0)=-1/3$. Consequently

$$
f_{\rm s}\sim-\frac{|\mathcal A_2|^{3/2}}{3\mathcal A_6^{1/2}}\sim-(T_c-T)^{3/2},
$$

provided the quadratic coefficient has a nonzero thermal slope and the sextic coefficient has a finite positive limit. Since the [heat-capacity critical exponent](../../../critical-phenomenon.md#heat-capacity-critical-exponent) satisfies $f_{\rm s}\sim|T-T_c|^{2-\alpha}$,

$$
\boxed{2-\alpha=\frac32,\qquad \alpha=\frac12.}
$$

Equivalently, twice differentiating this ordered-side [free-energy density](../../../statistical-physics.md#free-energy-density) produces the $(T_c-T)^{-1/2}$ singularity. The scaling path and branch qualifications are the same as for the direct [Landau theory](../../../critical-phenomenon.md#landau-theory) calculation: a nonzero fixed positive quartic coefficient would instead send $X\to\infty$ and yield the ordinary transition of part (e).

## 2

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Take the couplings in the [Hamiltonian](../../../classical-mechanics.md#hamiltonian) to include [inverse temperature](../../../thermodynamics.md#inverse-temperature), so the [Boltzmann factor](../../../statistical-physics.md#boltzmann-factor) is $e^{-H}$. If physical energies are used instead, first replace $J,L,D,K$ by their products with $1/(k_BT)$. Split the on-site term equally between its two bonds. For spin states $s,t\in\{1,0,-1\}$ the [spin-chain transfer matrix](../../../statistical-physics.md#transfer-matrix-for-a-classical-spin-chain) has entries

$$
W_{st}=\exp\left[Jst+Ls^2t^2+\frac D2(s^2+t^2)+K\right].
$$

Using the specified coupling coordinates, in the order $(1,0,-1)$ this is

$$
\boxed{W=\frac{e^K}{z}\begin{pmatrix}1&x&y\\x&z&x\\y&x&1\end{pmatrix}.}
$$

For example, $e^{D/2}=x/z$ and $e^{-J+L+D}=y/z$. This is the nearest-neighbour [Blume–Emery–Griffiths model](../../../statistical-physics.md#blume-emery-griffiths-model) with an additive constant and the paper's sign convention for $D$.

Summing the periodic spin chain gives the [partition function](../../../statistical-physics.md#canonical-partition-function) $Z_N=\operatorname{tr}W^N=\sum_{a=1}^3\lambda_a^N$. For finite real couplings all entries of $W$ are strictly positive; the [Perron–Frobenius theorem](../../../vector-space.md#perron-frobenius-theorem) gives a unique positive [dominant eigenvalue](../../../linear-operator-theory.md#dominant-eigenvalue) with $\lambda_1>|\lambda_a|$ for $a\ne1$. Since $W$ is a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), all its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are real. Thus in the [thermodynamic limit](../../../statistical-physics.md#thermodynamic-limit),

$$
\boxed{\frac{F_N}{Nk_BT}\longrightarrow-\log\lambda_1.}
$$

The positivity condition is stronger and more useful than mere ordering by signed value: subdominant [eigenvalues](../../../linear-operator-theory.md#eigenvalue) can be negative. Also, the printed strict ordering between the other two is not guaranteed for all couplings. For instance, $J=L=D=0$ makes $W$ the positive constant [matrix](../../../vector-space.md#matrix) $e^K\mathbf1\mathbf1^T$ with two equal zero [eigenvalues](../../../linear-operator-theory.md#eigenvalue). Degeneracy there does not affect the largest-eigenvalue limit; no explicit generic [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are needed.

For [spin magnetization](../../../statistical-physics.md#spin-magnetization), introduce a dimensionless field $h$ through $-h\sum_i\sigma_i$, or insert $S=\operatorname{diag}(1,0,-1)$ into the [trace](../../../linear-algebra.md#matrix-trace). Then

$$
\langle\sigma_i\rangle=\frac{\operatorname{tr}(SW^N)}{\operatorname{tr}W^N}\longrightarrow v_1^TSv_1=\left.\partial_h\log\lambda_1(h)\right|_{h=0},
$$

where $v_1$ is a normalized [eigenvector](../../../linear-operator-theory.md#eigenvector) of the largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) and $W_{st}(h)=e^{h(s+t)/2}W_{st}(0)$. [Spin inversion symmetry](../../../statistical-physics.md#spin-inversion-symmetry) gives $v_{1,+}=v_{1,-}$, since the positive [eigenvector](../../../linear-operator-theory.md#eigenvector) of the largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is unique. Therefore

$$
\boxed{\langle\sigma_i\rangle=0}
$$

at zero field, both at finite $N$ and in the finite-coupling [thermodynamic limit](../../../statistical-physics.md#thermodynamic-limit). The finite-$N$ result follows directly by pairing each configuration with its spin-reversed partner. [Eigenvalues](../../../linear-operator-theory.md#eigenvalue) at a single fixed field do not determine a general observable: a field derivative of the largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue), or its [eigenvector](../../../linear-operator-theory.md#eigenvector), is required. Positivity and the [real analytic](../../../analysis.md#real-analytic-function) dependence on the couplings exclude a finite-temperature [spontaneous symmetry breaking](../../../quantum-field-theory.md#spontaneous-symmetry-breaking) transition in this one-dimensional finite-range chain; singular zero-temperature coupling limits require separate treatment.

For even $N$, [spin decimation](../../../critical-phenomenon.md#spin-decimation) on alternate sites sums the middle spin of each two-bond segment, hence the coarse [spin-chain transfer matrix](../../../statistical-physics.md#transfer-matrix-for-a-classical-spin-chain) is $W'=W^2$. Define

$$
A=1+x^2+y^2,\qquad B=x(1+y+z),\qquad C=x^2+2y,\qquad E=z^2+2x^2.
$$

Direct multiplication gives $W^2=e^{2K}z^{-2}\begin{pmatrix}A&B&C\\B&E&B\\C&B&A\end{pmatrix}$. Matching its entry ratios to the original parameterization yields the [spin-1 chain decimation recursion](../../../critical-phenomenon.md#spin-1-chain-decimation-recursion)

$$
\boxed{x'=\frac{x(1+y+z)}{1+x^2+y^2},\qquad y'=\frac{x^2+2y}{1+x^2+y^2},\qquad z'=\frac{z^2+2x^2}{1+x^2+y^2}.}
$$

The remaining overall positive factor is absorbed into $K'$. Keeping that factor preserves the [free energy](../../../thermodynamics.md#thermodynamic-free-energy) as well as normalized spin [probabilities](../../../probability-theory.md#probability). Indeed $\operatorname{tr}(W^2)^{N/2}=\operatorname{tr}W^N$, exactly; on an odd ring an unmatched boundary segment needs separate handling rather than assuming a uniform two-site block decomposition.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

The fixed-point equation for $u$ factors as

$$
u\bigl[(1+u^2)^2-4u\bigr]=u(u-1)(u^3+u^2+3u-1)=0.
$$

The cubic derivative is $3u^2+2u+3>0$ for every real $u$; its values at zero and one have opposite signs. Thus the possible first coordinates in the stated domain are exactly $u=0,u_*,1$.

For finite $v$, the second fixed-point equation is $v[v^3-(1+u^2)^2]=0$. The [renormalization-group fixed points](../../../critical-phenomenon.md#renormalization-group-fixed-point) are consequently

$$
\boxed{(a,0),\quad \bigl(a,(1+a^2)^{2/3}\bigr),\quad (a,\infty),\qquad a\in\{0,u_*,1\}.}
$$

There are six finite points and three boundary points at infinity. Infinity is interpreted in a compactified domain, not as an ordinary real number. The [reciprocal coordinate at infinite coupling](../../../critical-phenomenon.md#reciprocal-coordinate-at-infinite-coupling) $w=1/v$ transforms as $w'=(1+u^2)^2w^4$, making $w=0$ a well-defined boundary fixed point.

At any finite fixed point $(\tilde u,\tilde v)$, let $\delta u=u-\tilde u$, $\delta v=v-\tilde v$. The [Jacobian matrix](../../../calculus.md#jacobian-matrix) linearization is

$$
\begin{pmatrix}\delta u'\\\delta v'\end{pmatrix}=\begin{pmatrix}\dfrac{8\tilde u(1-\tilde u^2)}{(1+\tilde u^2)^3}&0\\[5pt]-\dfrac{4\tilde u\tilde v^4}{(1+\tilde u^2)^3}&\dfrac{4\tilde v^3}{(1+\tilde u^2)^2}\end{pmatrix}\begin{pmatrix}\delta u\\\delta v\end{pmatrix}+O(\|(\delta u,\delta v)\|^2).
$$

The only point with both coordinates strictly interior is $\tilde u=u_*$, $\tilde v=(1+u_*^2)^{2/3}$. Using its fixed-point relations, the [matrix](../../../vector-space.md#matrix) becomes

$$
M_* =\begin{pmatrix}\rho&0\\c&4\end{pmatrix},\qquad \rho=\frac{2(1-u_*^2)}{1+u_*^2},\qquad c=-\frac{4u_*\tilde v}{1+u_*^2}.
$$

Its [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $\rho$ and $4$. In particular, $u_*<1/\sqrt3$ because the increasing cubic is already positive there, so $\rho>1$ (numerically about $1.68$). The corresponding [eigenvectors](../../../linear-operator-theory.md#eigenvector) can be chosen as $(1,c/(\rho-4))^T$ and $(0,1)^T$. Both discrete multipliers exceed one, hence

$$
\boxed{\text{the unique interior fixed point is repulsive in both directions}.}
$$

Both perturbations are [relevant directions of a fixed point](../../../critical-phenomenon.md#relevant-direction-of-a-fixed-point) under repeated coarse-graining, rather than one stable and one unstable direction. A length-rescaling factor was not specified, so these multipliers should not be assigned numerical critical scaling exponents without additional information. At $a=0,1$, the $u$ multiplier is zero; at $v=0$ or $w=0$ the other multiplier is also zero. Thus the four corner points attract locally within the domain, the two positive finite boundary points at $a=0,1$ are saddles, and the points $(u_*,0),(u_*,\infty)$ have one repulsive and one attractive direction.

## 3

↑ **Parent:** [Paper 303](paper-303.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Use a dimensionless [Hamiltonian](../../../classical-mechanics.md#hamiltonian) in the functional weight $e^{-H}$, assume $\alpha>0$, and let $\phi(\mathbf x)=\int_{|\mathbf p|\leq\Lambda}d^Dp\,(2\pi)^{-D}e^{i\mathbf p\cdot\mathbf x}\widetilde\phi(\mathbf p)$. Reality means $\widetilde\phi(-\mathbf p)=\widetilde\phi(\mathbf p)^*$. At zero field, the [quadratic form](../../../linear-algebra.md#quadratic-form) is

$$
H_0=\frac12\int_{|\mathbf p|\leq\Lambda}\frac{d^Dp}{(2\pi)^D}\left(\alpha^{-1}p^2+r_0\right)|\widetilde\phi(\mathbf p)|^2.
$$

In the [momentum-shell renormalization group](../../../critical-phenomenon.md#momentum-shell-renormalization-group), split into $\phi_<+\phi_>$ below and above $\Lambda/b$. Disjoint Fourier supports make the [quadratic form](../../../linear-algebra.md#quadratic-form) split into $H_0[\phi_<]+H_0[\phi_>]$. Integration over the shell gives a source-independent [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) multiplying the [partition function](../../../statistical-physics.md#canonical-partition-function), or an additive constant in the effective [free energy](../../../thermodynamics.md#thermodynamic-free-energy); it leaves the slow-mode quadratic coefficients unchanged before rescaling. A uniform field has support only at zero momentum, so it does not change this shell integration.

Restore the [ultraviolet cutoff](../../../quantum-field-theory.md#ultraviolet-cutoff) by $\mathbf p'=b\mathbf p$, $\mathbf x'=\mathbf x/b$, and choose

$$
\phi'(\mathbf x')=b^{(D-2)/2}\phi_<(b\mathbf x'),\qquad \widetilde\phi'(\mathbf p')=b^{-(D+2)/2}\widetilde\phi_< (\mathbf p'/b).
$$

The measure, two gradients and two fields have scale factors $b^D$, $b^{-2}$ and $b^{-(D-2)}$, whose product is one. The mass term has factor $b^D b^{-(D-2)}=b^2$, while the uniform source term has factor $b^D b^{-(D-2)/2}=b^{(D+2)/2}$. Hence the [Gaussian momentum-shell scaling](../../../critical-phenomenon.md#gaussian-momentum-shell-scaling) is

$$
\boxed{\alpha^{-1}\longmapsto\alpha^{-1},\qquad r_0\longmapsto b^2r_0,\qquad h\longmapsto b^{(D+2)/2}h.}
$$

For a slowly varying nonuniform source the corresponding formula is $h'(\mathbf x')=b^{(D+2)/2}h(b\mathbf x')$. Here the nonuniform source on the right is its projection onto the retained [Fourier modes](../../../fourier-analysis.md#fourier-mode); an eliminated source component contributes only to the field-independent Gaussian normalization. The field [engineering dimension](../../../critical-phenomenon.md#engineering-dimension) is $(D-2)/2$ and its Gaussian [anomalous dimension](../../../critical-phenomenon.md#anomalous-dimension) is zero. The mass and uniform source are relevant perturbations of the [Gaussian fixed point](../../../critical-phenomenon.md#gaussian-fixed-point). Positivity of $\alpha$ is necessary for a stable [kinetic term](../../../quantum-field-theory.md#kinetic-term) near this point. One can use a finite volume and positive mass as infrared regulators and then take the critical limit; at exactly zero mass the integral over the zero [Fourier mode](../../../fourier-analysis.md#fourier-mode) alone is not a normalized finite-volume [Gaussian measure](../../../stochastic-process.md#gaussian-measure).

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Compute the coupling flow at zero [magnetic field](../../../electromagnetism.md#magnetic-field), or assume the source has support only in retained [Fourier modes](../../../fourier-analysis.md#fourier-mode), so that the shell [Gaussian measure](../../../stochastic-process.md#gaussian-measure) is centered. First justify the shell propagator. For a positive quadratic kernel on the shell, the [Gaussian functional integral](../../../quantum-field-theory.md#gaussian-functional-integral) gives [covariance](../../../variance.md#covariance) equal to the inverse kernel,

$$
\langle\widetilde\phi_>(\mathbf p)\widetilde\phi_>(\mathbf q)\rangle_0^{\rm shell}=(2\pi)^D\delta^{(D)}(\mathbf p+\mathbf q)\frac{\alpha}{p^2+\alpha r_0},
$$

with both momenta restricted to $\Lambda/b<|\mathbf p|\leq\Lambda$. Inserting the [Fourier transforms](../../../analysis.md#fourier-transform) and using the [Dirac delta function](../../../distribution-theory.md#dirac-delta-function) yields the [Gaussian shell covariance](../../../critical-phenomenon.md#gaussian-shell-covariance)

$$
\boxed{G_>(\mathbf x-\mathbf y)=\int_{\Lambda/b<|\mathbf p|\leq\Lambda}\frac{d^Dp}{(2\pi)^D}\frac{\alpha e^{i\mathbf p\cdot(\mathbf x-\mathbf y)}}{p^2+\alpha r_0}.}
$$

Changing $\mathbf p$ to $-\mathbf p$ gives the negative-exponent convention as well. The dependence is on the separation, as required by [translation invariance](../../../physics.md#translation-invariance). The printed numerator uses $\mathbf x$ alone: it is correct only if that symbol means the separation or if $\mathbf y=0$. For example at $\mathbf x=\mathbf y\ne0$, the [covariance](../../../variance.md#covariance) must equal the constant coincident value $G_>(0)$, while the literal printed integral generally depends on $\mathbf x$. Thus the missing separation is a real source qualification, not a change of Fourier-sign convention.

Integrating out the shell gives $H_{\rm eff}[\phi_<]=H_0[\phi_<]-\log\langle e^{-V[\phi_<+\phi_>]}\rangle_0^{\rm shell}$, up to a field-independent constant. At first order in $u_0$, the [cumulant expansion of a coarse-grained free energy](../../../critical-phenomenon.md#cumulant-expansion-of-a-coarse-grained-free-energy) retains $\langle V\rangle$. Odd moments of the centered [Gaussian measure](../../../stochastic-process.md#gaussian-measure) vanish and [Wick theorem](../../../perturbative-quantum-field-theory.md#wick-s-theorem) gives $\langle\phi_>^4\rangle=3G_>(0)^2$. Writing $I_1=G_>(0)$,

$$
\langle V\rangle=\frac{u_0}{24}\int d^Dx\,[\phi_<^4+6I_1\phi_<^2+3I_1^2].
$$

The last term affects only the constant; the second is a momentum-independent [tadpole diagram](../../../perturbative-quantum-field-theory.md#tadpole-diagram) correction. Before rescaling it changes $r_0$ to $r_0+u_0I_1/2$, leaves the quartic coefficient at $u_0$, and produces no [gradient](../../../calculus.md#gradient) correction. Combining with part (a) gives the leading coupling recursion

$$
\boxed{r_0'=b^2\left(r_0+\frac{u_0}{2}I_1\right)+O(u_0^2),\qquad u_0'=b^{4-D}u_0+O(u_0^2),\qquad \alpha^{-1\prime}=\alpha^{-1}+O(u_0^2).}
$$

This is [one-loop shell mass renormalization in scalar quartic theory](../../../critical-phenomenon.md#one-loop-shell-mass-renormalization-in-scalar-quartic-theory). Here $I_1=\int_{\rm shell}d^Dp\,(2\pi)^{-D}\alpha/(p^2+\alpha r_0)$. The shell Gaussian is well defined if $p^2+\alpha r_0>0$ there; near $r_0=0$ this follows from $\alpha>0$. A negative slow-mode mass may be stabilized by the retained quartic term and does not require pretending that the full unconstrained quadratic measure at negative mass is normalizable.

Linearizing about $(r_0,u_0)=(0,0)$ gives

$$
\begin{pmatrix}r_0'\\u_0'\end{pmatrix}=\begin{pmatrix}b^2&\tfrac12b^2I_1(0)\\0&b^{4-D}\end{pmatrix}\begin{pmatrix}r_0\\u_0\end{pmatrix}+O(r_0u_0,u_0^2).
$$

Its mass and quartic [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are $b^2$ and $b^{4-D}$. The off-diagonal term is an additive critical-mass shift: setting the bare $r_0=0$ is not generally the critical tuning when $u_0>0$. The mass remains relevant for every $D$; at $D=2$ the two linear [eigenvalues](../../../linear-operator-theory.md#eigenvalue) coincide and the [matrix](../../../vector-space.md#matrix) can have a [Jordan block](../../../linear-operator-theory.md#jordan-block), but both perturbations are still relevant.

For $D>4$, the quartic interaction is an [irrelevant operator](../../../critical-phenomenon.md#irrelevant-operator), and the [Gaussian fixed point](../../../critical-phenomenon.md#gaussian-fixed-point) attracts weak quartic perturbations after the mass and [magnetic field](../../../electromagnetism.md#magnetic-field) have been tuned. The quartic can nevertheless be a [dangerously irrelevant coupling](../../../critical-phenomenon.md#dangerously-irrelevant-coupling): its positive value stabilizes the ordered phase. For $D<4$, it is a [relevant operator](../../../critical-phenomenon.md#relevant-operator), so the Gaussian description is unstable toward interactions. At $D=4$ it is a [marginal operator](../../../critical-phenomenon.md#marginal-operator); first-order perturbation theory alone does not decide its fate.

To settle that borderline case, retain the leading quartic contribution from the second cumulant, at zero external momentum in the local expansion. The two-fast-field part of $V$ is $(u_0/4)\int\phi_<^2\phi_>^2$. Since $\langle\phi_>^2(\mathbf x)\phi_>^2(\mathbf y)\rangle_c=2G_>(\mathbf x-\mathbf y)^2$, its connected second cumulant contributes

$$
-\frac{u_0^2}{16}\int d^Dx\,d^Dy\,\phi_<^2(\mathbf x)\phi_<^2(\mathbf y)G_>(\mathbf x-\mathbf y)^2.
$$

Keeping the local quartic term and using [Parseval identity](../../../fourier-analysis.md#parseval-identity) gives $\int d^Dy\,G_>(\mathbf x-\mathbf y)^2=I_2$, where $I_2=\int_{\rm shell}d^Dp\,(2\pi)^{-D}[\alpha/(p^2+\alpha r_0)]^2$. Thus the [one-loop shell quartic renormalization](../../../critical-phenomenon.md#one-loop-shell-quartic-renormalization) is

$$
\boxed{u_0'=b^{4-D}\left[u_0-\frac32u_0^2I_2\right]+\text{higher-order and derivative terms}.}
$$

The coefficient follows from multiplying the quartic density correction $-u_0^2I_2/16$ by $4!=24$. This local, zero-external-momentum coupling extraction is not a claim that the exact finite-shell effective action retains only its original [polynomial](../../../polynomial.md); further operators are generated.

More explicitly, for a thin shell $b=e^{d\ell}$, let $c_D=\operatorname{area}(S^{D-1})/(2\pi)^D$, $R=\alpha r_0/\Lambda^2$ and $g=c_D\alpha^2\Lambda^{D-4}u_0$. With increasing length scale $\ell$, the leading flow is

$$
\frac{dR}{d\ell}=2R+\frac{g}{2(1+R)}+O(g^2),\qquad \frac{dg}{d\ell}=(4-D)g-\frac{3g^2}{2(1+R)^2}+O(g^3).
$$

This convention has the opposite scale direction to a [renormalization-group beta function](../../../perturbative-quantum-field-theory.md#beta-function-physics) defined using increasing momentum. On the tuned [critical surface](../../../critical-phenomenon.md#critical-surface) at $D=4$, $R=O(g)$ and $dg/d\ell=-3g^2/2+O(g^3)$, so weak positive $g$ is [marginally irrelevant](../../../critical-phenomenon.md#marginally-irrelevant-operator), tending to zero with logarithmic corrections rather than remaining an exactly marginal parameter. Just below four dimensions, $D=4-\varepsilon$ with $0<\varepsilon\ll1$, the same calculation yields the [Wilson-Fisher fixed point](../../../critical-phenomenon.md#wilson-fisher-fixed-point) $g_*=2\varepsilon/3+O(\varepsilon^2)$, $R_*=-\varepsilon/6+O(\varepsilon^2)$. It does not justify extrapolating a small-$\varepsilon$ expansion to every lower dimension. The ordinary scalar quartic [upper critical dimension](../../../critical-phenomenon.md#upper-critical-dimension) is therefore

$$
\boxed{D_c=4.}
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2017](../../2017.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
