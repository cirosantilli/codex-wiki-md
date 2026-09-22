# Paper 57

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper57.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2007/Paper57.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

The [Noether gauging procedure](../../../quantum-field-theory.md#noether-gauging-procedure) begins with a rigid symmetry parameter $\epsilon$. Replacing it by $\epsilon(x)$ leaves in the action variation a term proportional to $j^\mu\partial_\mu\epsilon$. Introduce a [gauge field](../../../relativistic-quantum-field.md#gauge-field) whose variation contains $\partial_\mu\epsilon$ and couple it to the [Noether current](../../../quantum-field-theory.md#noether-current) $j^\mu$ to cancel that term. The new coupling produces further variations, so both the action and transformation laws are corrected successively in the coupling constant until local invariance is obtained. [Covariant derivatives](../../../general-relativity.md#covariant-derivative) organize this iterative completion.

For the [Wess–Zumino model](../../../supersymmetry.md#wess-zumino-model), the parameter is a spinor and the current is the [supercurrent](../../../supersymmetry.md#supercurrent). Its derivative part has the structure $\gamma^\nu\partial_\nu(A-i\gamma_5B)\gamma^\mu\psi$, up to the fixed [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) normalization and improvements. The [gauge field](../../../relativistic-quantum-field.md#gauge-field) is the [spin](../../../quantum-mechanics.md#spin)-$3/2$ [gravitino](../../../supersymmetry.md#gravitino) $\Psi_\mu$, with leading transformation $\delta\Psi_\mu=\kappa^{-1}D_\mu\epsilon+\cdots$. A coupling of $\bar\Psi_\mu$ to that current cancels the derivative of the local parameter. Since the commutator of two local [supersymmetries](../../../supersymmetry.md) includes a spacetime transformation, the [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) and gravity must participate as well. This gives the [Wess-Zumino chiral multiplet coupled to supergravity](../../../supersymmetry.md#wess-zumino-chiral-multiplet-coupled-to-supergravity).

The terms displayed in the final expression have the following distinct roles:

- The [scalar field](../../../quantum-field-theory.md#scalar-field) [kinetic term](../../../quantum-field-theory.md#kinetic-term) acquires the invariant volume density $e$ and the inverse [metric tensor](../../../general-relativity.md#metric-tensor). For a [Lorentz scalar](../../../special-relativity.md#lorentz-scalar) the spacetime [covariant derivative](../../../general-relativity.md#covariant-derivative) is just its ordinary derivative; the metric contraction is what changes from the rigid theory.
- The [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) [kinetic term](../../../quantum-field-theory.md#kinetic-term) uses curved [gamma matrices](../../../algebra.md#gamma-matrices) $\gamma^\mu=e_a{}^\mu\gamma^a$ and the [spinor covariant derivative](../../../connection-1-form.md#spinor-covariant-derivative). The factor one half avoids double counting the real Majorana degrees of freedom. The [spin connection](../../../connection-1-form.md#spin-connection) makes the term locally [Lorentz covariant](../../../special-relativity.md#lorentz-covariance).
- The curvature term is the [Einstein-Hilbert action](../../../general-relativity.md#einstein-hilbert-action), with gravitational coupling $\kappa$. Its variation cancels the curvature terms generated when [covariant derivatives](../../../general-relativity.md#covariant-derivative) are commuted in the [gravitino](../../../supersymmetry.md#gravitino) variation. Its sign follows the source's curvature and metric conventions.
- The [gravitino](../../../supersymmetry.md#gravitino) [kinetic term](../../../quantum-field-theory.md#kinetic-term) is the curved-space [Rarita-Schwinger field](../../../relativistic-quantum-field.md#rarita-schwinger-field) action. It supplies the dynamical [gauge field](../../../relativistic-quantum-field.md#gauge-field) needed to localize [supersymmetry](../../../supersymmetry.md), just as a gauge-field kinetic term accompanies an ordinary gauging.
- The term of order $\kappa$ is the [gravitino](../../../supersymmetry.md#gravitino)–[supercurrent](../../../supersymmetry.md#supercurrent) coupling. Its scalar factor must be differentiated: in standard notation it contains $\not\!D(A-i\gamma_5B)$. The glyph rendered as $\phi$ before the parentheses in the source formula must be read as a slashed derivative, or corrected to one; the undifferentiated scalar product would not be the free [Wess–Zumino model](../../../supersymmetry.md#wess-zumino-model) [supercurrent](../../../supersymmetry.md#supercurrent).
- The order-$\kappa^2$ term bilinear in [gravitini](../../../supersymmetry.md#gravitino) couples their chiral current to the [scalar field](../../../quantum-field-theory.md#scalar-field) phase [Noether current](../../../quantum-field-theory.md#noether-current) $J_\mu=A D_\mu B-(D_\mu A)B$.
- The remaining order-$\kappa^2$ term couples the matter [axial current](../../../relativistic-quantum-field.md#axial-current) $\bar\psi\gamma_5\gamma^\mu\psi$ to the same $J_\mu$.

The last two interactions are part of the higher-order local [supersymmetry](../../../supersymmetry.md) completion. They can be organized through the [composite Kähler connection](../../../supersymmetry.md#composite-kahler-connection) in the fermion derivatives, or derived by eliminating the corresponding supergravity auxiliary connection. Matter fermions and [gravitini](../../../supersymmetry.md#gravitino) carry the appropriate chiral Kähler weights, fixing the relative current couplings. They are not new adjustable [Yukawa interactions](../../../standard-model.md#yukawa-interaction). In reading this organization, one must not include the composite connection in $D_\mu$ and then count its separately displayed current terms a second time.

Finally the [spin connection](../../../connection-1-form.md#spin-connection) itself acquires [gravitino-induced torsion](../../../supersymmetry.md#gravitino-induced-torsion) and matter spin-current contributions. Eliminating this algebraic connection, or solving for [auxiliary fields](../../../supersymmetry.md#auxiliary-field), can make further fermion contact terms implicit in the chosen [covariant derivatives](../../../general-relativity.md#covariant-derivative) and component convention. The key mechanism is **current coupling at first order, followed by the covariant and higher-order terms required by local [supersymmetry](../../../supersymmetry.md)**, rather than merely changing ordinary derivatives in the original matter Lagrangian.

## 2

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

Use four-dimensional [Minkowski spacetime](../../../special-relativity.md#minkowski-spacetime) with $\{\gamma^\mu,\gamma^\nu\}=2\eta^{\mu\nu}$ and $\gamma^{\mu\nu\rho}=\gamma^{[\mu}\gamma^\nu\gamma^{\rho]}$. The [Clifford algebra](../../../algebra.md#clifford-algebra) duality identity makes the displayed epsilon-form equation equivalent, up to a nonzero convention-dependent phase, to

$$
E^\mu:=\gamma^{\mu\nu\rho}\partial_\nu\Psi_\rho=0.
$$

This is the [Euler-Lagrange equation](../../../analysis.md#euler-lagrange-equation) of the first-order [Rarita-Schwinger field](../../../relativistic-quantum-field.md#rarita-schwinger-field) action $-\tfrac12\bar\Psi_\mu\gamma^{\mu\nu\rho}\partial_\nu\Psi_\rho$, with the overall phase adjusted to the chosen Majorana convention. Varying the [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) action accounts for both occurrences of the field and cancels the one-half normalization.

A vector times a spinor contains [spin](../../../quantum-mechanics.md#spin)-$3/2$ and unwanted [spin](../../../quantum-mechanics.md#spin)-$1/2$ pieces, so the tensor type alone does not establish the physical spin. The field equation has [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance)

$$
\Psi_\mu\longmapsto\Psi_\mu+\partial_\mu\epsilon,
$$

since the two derivatives contract an antisymmetric pair of gamma indices. Put $\chi=\gamma^\mu\Psi_\mu$ and $d=\partial^\mu\Psi_\mu$. [Gamma matrix](../../../algebra.md#gamma-matrices) multiplication gives

$$
E^\mu=\not\!\partial\Psi^\mu-\partial^\mu\chi
+\gamma^\mu(\not\!\partial\chi-d),\qquad
\gamma_\mu E^\mu=2(\not\!\partial\chi-d).
$$

Hence $d=\not\!\partial\chi$. Use the [gauge transformation](../../../electromagnetism.md#gauge-transformation), under which $\delta\chi=\not\!\partial\epsilon$, to impose $\chi=0$. The equations then imply

$$
\boxed{\gamma\cdot\Psi=0,\qquad\partial\cdot\Psi=0,\qquad
\not\!\partial\Psi_\mu=0,}
$$

with residual gauge freedom satisfying $\not\!\partial\epsilon=0$.

For a [plane wave](../../../quantum-mechanics.md#plane-wave) with nonzero momentum satisfying the [null condition](../../../special-relativity.md#null-condition) along the third axis, this residual freedom sets the temporal component to zero. Transversality then removes the longitudinal component, leaving the [tensor product](../../../linear-algebra.md#tensor-product) of two transverse vector polarizations with the two massless spinor [helicities](../../../special-relativity.md#helicity). The possible total [helicities](../../../special-relativity.md#helicity) are $\pm3/2$ and $\pm1/2$. The [gamma trace](../../../relativistic-quantum-field.md#gamma-trace-of-a-vector-spinor) is a rotation-covariant map to a spinor, which has only [helicities](../../../special-relativity.md#helicity) $\pm1/2$. It therefore vanishes on the aligned $\pm3/2$ combinations and removes the two mixed combinations. Equivalently, the transverse [gamma trace](../../../relativistic-quantum-field.md#gamma-trace-of-a-vector-spinor) condition has rank two on the four remaining complex positive-frequency coefficients. The [massless Rarita-Schwinger polarization count](../../../relativistic-quantum-field.md#massless-rarita-schwinger-polarization-count) is thus

$$
\boxed{h=\pm\tfrac32:\quad2\text{ physical states for a Majorana gravitino}.}
$$

The [Majorana spinor](../../../relativistic-quantum-field.md#majorana-spinor) reality condition relates negative-frequency coefficients to their conjugates; it does not introduce a separate antiparticle multiplet. A complex vector-spinor would also have independent antiparticle states.

A nonzero standard [Rarita-Schwinger field](../../../relativistic-quantum-field.md#rarita-schwinger-field) mass term destroys the massless [gauge invariance](../../../relativistic-quantum-field.md#gauge-invariance) and adds the two longitudinal [helicities](../../../special-relativity.md#helicity). To see the constraints explicitly, choose its momentum-space sign so the equation is

$$
\gamma^{\mu\nu\rho}p_\nu u_\rho+m\gamma^{\mu\rho}u_\rho=0.
$$

Contracting with $p_\mu$ gives $\not\!p(\gamma\cdot u)-p\cdot u=0$. Its [gamma trace](../../../relativistic-quantum-field.md#gamma-trace-of-a-vector-spinor) then gives $3m\,\gamma\cdot u=0$. For $m\ne0$ these imply $\gamma\cdot u=p\cdot u=0$, and the remaining [Dirac equation](../../../relativistic-quantum-field.md#dirac-equation) is $(\not\!p-m)u_\mu=0$. In the rest frame $u_0=0$. Three spatial vector components times two positive-energy spinor components give six coefficients, and the [gamma trace](../../../relativistic-quantum-field.md#gamma-trace-of-a-vector-spinor) removes two, leaving the irreducible [spin](../../../quantum-mechanics.md#spin)-$3/2$ representation. Therefore

$$
\boxed{\text{a massive Majorana gravitino has }4\text{ physical states},
\quad h=\pm\tfrac32,\ \pm\tfrac12.}
$$

In [supergravity](../../../supersymmetry.md#supergravity) a consistent spontaneous mass generation is the [super-Higgs mechanism](../../../supersymmetry.md#super-higgs-mechanism), which supplies those extra states from the [goldstino](../../../supersymmetry.md#goldstino).

The massless [graviton](../../../quantum-theory.md#graviton) also has two physical [helicities](../../../special-relativity.md#helicity), so the [graviton](../../../quantum-theory.md#graviton) and [gravitino](../../../supersymmetry.md#gravitino) already match on shell. The reason for [auxiliary fields](../../../supersymmetry.md#auxiliary-field) is the [off-shell component count of minimal supergravity](../../../supersymmetry.md#off-shell-component-count-of-minimal-supergravity) mismatch, not a mismatch of these physical states. After removing gauge functions but before using field equations, a metric has $10-4=6$ independent bosonic components, while a Majorana vector-spinor has $16-4=12$ fermionic components. In [vierbein](../../../general-relativity.md#orthonormal-coframe-in-spacetime) language the same bosonic count is $16-6-4=6$, subtracting local Lorentz and [diffeomorphism](../../../geometry-and-topology.md#diffeomorphism) gauges. [Old-minimal supergravity](../../../supersymmetry.md#old-minimal-supergravity) adds a complex scalar and a real vector, supplying six real nonpropagating bosonic components. This gives **$12+12$ off-shell components and closure without imposing equations of motion**. Their algebraic elimination leaves the physical $2+2$ [graviton](../../../quantum-theory.md#graviton)–[gravitino](../../../supersymmetry.md#gravitino) spectrum unchanged.

## 3

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

Write $S=\Phi_0$, $u=\Phi_+$, $v=\Phi_-$, $M=M_p$, $P=uv-\zeta$, $x=|S|^2/M^2$ and $q=|u|^2+|v|^2$. Assume $g\ne0$ and, initially, $\zeta\ne0$. The [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential) is

$$
V_F=e^{K/M^2}\left(K^{i\bar j}D_iW\overline{D_jW}-\frac{3|W|^2}{M^2}\right),\qquad D_iW=W_i+\frac{K_iW}{M^2}.
$$

The canonical [Kähler potential](../../../supersymmetry.md#kahler-potential) gives the identity [Kähler metric](../../../complex-geometry.md#kahler-metric). The three [Kähler covariant derivatives of a superpotential](../../../supersymmetry.md#kahler-covariant-derivative-of-a-superpotential) are

$$
D_SW=gP(1+x),\qquad D_uW=gS\left(v+\frac{\bar uP}{M^2}\right),\qquad D_vW=gS\left(u+\frac{\bar vP}{M^2}\right).
$$

Substituting, including the negative term rather than treating the potential as just a sum of squares, gives the exact answer

$$
\boxed{V_F=|g|^2e^{x+q/M^2}\left[(1-x+x^2)|uv-\zeta|^2+|S|^2\left(\left|v+\frac{\bar u(uv-\zeta)}{M^2}\right|^2+\left|u+\frac{\bar v(uv-\zeta)}{M^2}\right|^2\right)\right].}
$$

Here $(1+x)^2-3x=1-x+x^2$ explains the first coefficient. It is strictly positive for real $x$, since $1-x+x^2=(x-1/2)^2+3/4$. Thus this model's [scalar potential](../../../quantum-field-theory.md#scalar-potential) is nonnegative everywhere.

In the stated limit $q/M^2\ll1$, the exponential can be replaced by $e^x[1+O(q/M^2)]$. The other displayed terms retain the effects of the [Kähler covariant derivatives of a superpotential](../../../supersymmetry.md#kahler-covariant-derivative-of-a-superpotential). Small waterfall fields alone do not justify discarding $\zeta/M^2$ in those derivatives, or expanding in $x$. If also $|\zeta|/M^2\ll1$ and $x\ll1$, the leading result reduces to the global [F-term scalar potential](../../../supersymmetry.md#f-term-scalar-potential)

$$
V_{\mathrm{global}}=|g|^2\left(|uv-\zeta|^2+|S|^2q\right).
$$

No gauge sector or gauge coupling is supplied, so there is no specified [D-term](../../../supersymmetry.md#d-term) contribution to add.

The [supersymmetric vacuum manifold of a bilinear hybrid superpotential](../../../cosmic-inflation.md#supersymmetric-vacuum-manifold-of-a-bilinear-hybrid-superpotential) is

$$
\boxed{S=0,\qquad uv=\zeta,\qquad V_F=0.}
$$

Indeed $W=0$ and all three [Kähler covariant derivatives of a superpotential](../../../supersymmetry.md#kahler-covariant-derivative-of-a-superpotential) vanish there, so all [supergravity auxiliary fields](../../../supersymmetry.md#supergravity-auxiliary-field) vanish and [supersymmetry](../../../supersymmetry.md) is unbroken. The nonnegative [scalar potential](../../../quantum-field-theory.md#scalar-potential) makes this a global minimum. Conversely zero potential requires $uv=\zeta$, and then $|S|^2q=0$; for $\zeta\ne0$ this forces $S=0$. With just the supplied fields this is a complex [vacuum manifold](../../../quantum-field-theory.md#vacuum-manifold) before imposing any gauge quotient: the product is fixed but the ratio of $u$ and $v$ is not. More precisely, it is an F-flat vacuum manifold whether or not a gauge symmetry is specified. If one additionally gauges opposite charges, [D-flatness](../../../supersymmetry.md#d-flatness) typically imposes $|u|=|v|$, giving $|u|=|v|=\sqrt{|\zeta|}$ up to phases and gauge equivalence; that is an extra assumption, not a consequence of $K$ and $W$ alone.

The other familiar branch of [F-term hybrid inflation](../../../cosmic-inflation.md#f-term-hybrid-inflation) has $u=v=0$. Its nonzero derivative $D_SW=-g\zeta(1+x)$ establishes [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking), and its exact [scalar potential](../../../quantum-field-theory.md#scalar-potential) is

$$
\boxed{V_0(S)=|g\zeta|^2e^x(1-x+x^2).}
$$

The [canonical-Kähler correction to an F-term hybrid valley](../../../cosmic-inflation.md#canonical-kahler-correction-to-an-f-term-hybrid-valley) begins as

$$
V_0=|g\zeta|^2\left(1+\frac{x^2}{2}+O(x^3)\right).
$$

In particular the [inflaton](../../../cosmic-inflation.md#inflaton) quadratic mass cancels at this order; the first lift of the global flat valley is quartic in $|S|$.

To identify when this branch is a transverse minimum, rephase the waterfall fields so that $\zeta$ is real positive. To quadratic order in $u,v$, the global [scalar potential](../../../quantum-field-theory.md#scalar-potential) is

$$
|g\zeta|^2+|g|^2\left[|S|^2(|u|^2+|v|^2)-|\zeta|(uv+\bar u\bar v)\right].
$$

The normalized combinations $(u\pm\bar v)/\sqrt2$ diagonalize this quadratic form, with

$$
\boxed{m_\pm^2=|g|^2(|S|^2\pm|\zeta|)\quad\text{in the global approximation}.}
$$

Thus $|S|^2>|\zeta|$ gives a valley of transverse minima, while below the threshold the negative [eigenvalue](../../../linear-operator-theory.md#eigenvalue) produces the [waterfall instability in F-term hybrid inflation](../../../cosmic-inflation.md#waterfall-instability-in-f-term-hybrid-inflation).

The exact supergravity correction to this stability test is also available without taking $x$ small. Put $b=|\zeta|/M^2$. Expansion of the exact [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential) about $u=v=0$ gives equal diagonal coefficients $|g|^2M^2e^x[x+b^2(1+x^2)]$ and off-diagonal magnitude $|g|^2M^2e^xb(1+x+x^2)$. Hence

$$
m_\pm^2=|g|^2M^2e^x\left[x+b^2(1+x^2)\pm b(1+x+x^2)\right].
$$

For the usual sub-Planckian symmetry-breaking scale $0<b\ll1$, the lower [eigenvalue](../../../linear-operator-theory.md#eigenvalue) is $|g|^2M^2e^x(1-b)[x-b(1+x^2)]$. It is positive for the familiar sub-Planckian valley $b\ll x\ll1$, and changes sign near $x=b$.

**The printed assertion of two full minima requires qualification.** The broken branch is a transverse inflationary valley, not generally a second stationary minimum of the complete supergravity potential. In fact

$$
\frac{dV_0}{dx}=|g\zeta|^2e^xx(1+x)>0\qquad(x>0).
$$

Its only stationary point in $S$ is the origin. For $0<|\zeta|<M^2$ that point has a negative waterfall [eigenvalue](../../../linear-operator-theory.md#eigenvalue) $|g|^2(|\zeta|^2/M^2-|\zeta|)$. A direct counterexample is the path $S=0$, $u=v=a$ with real small $a$, after rephasing $\zeta>0$:

$$
V_F=|g|^2e^{2a^2/M^2}(a^2-\zeta)^2=|g|^2\zeta^2+2|g|^2\left(\frac{\zeta^2}{M^2}-\zeta\right)a^2+O(a^4).
$$

The negative quadratic coefficient proves it is not a minimum. No loop corrections or additional stabilizing interactions were specified that could create the requested second stationary vacuum. The mathematically supported interpretation is **a SUSY-breaking transverse valley and a zero-energy [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum) minimum manifold**. The limit on $u,v$ alone does not fix the parameter range $|\zeta|/M^2$; the familiar waterfall conclusion uses the sub-Planckian range just stated.

In the corresponding global theory the exponential prefactor, Kähler corrections to $D_iW$ and universal $-3|W|^2/M^2$ term are absent. Its $u=v=0$ valley has exactly constant tree-level energy $|g\zeta|^2$ for all $S$, whereas canonical [supergravity](../../../supersymmetry.md#supergravity) lifts it by the quartic correction above. The [supersymmetric vacuum](../../../supersymmetry.md#supersymmetric-vacuum) $S=0$, $uv=\zeta$ and its zero energy persist in both descriptions. If $\zeta=0$, the origin and the $S$ axis instead have vanishing F-terms; the broken-valley interpretation does not apply.

## 4

↑ **Parent:** [Paper 57](paper-57.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

Work in the supplied Planck units and write $t=T+\bar T>0$. The nonzero components of the [Kähler metric](../../../complex-geometry.md#kahler-metric) and its inverse are

$$
K_{T\bar T}=\frac3{t^2},\qquad K_{C\bar C}=1,\qquad K^{T\bar T}=\frac{t^2}3,\qquad K^{C\bar C}=1.
$$

The [Kähler covariant derivatives of a superpotential](../../../supersymmetry.md#kahler-covariant-derivative-of-a-superpotential) are

$$
D_TW=-\frac{3W}{t},\qquad D_CW=3C^2+\bar C(C^3+B).
$$

In the [supergravity F-term potential](../../../supersymmetry.md#supergravity-f-term-potential), $K^{T\bar T}|D_TW|^2=3|W|^2$ cancels its negative universal term. This is the [no-scale supergravity](../../../supersymmetry.md#no-scale-supergravity) identity. The exact answer is therefore

$$
\boxed{V=\frac{e^{|C|^2}}{t^3}\left|3C^2+\bar C(C^3+B)\right|^2\ge0.}
$$

In particular $C=0$ is a global minimum for every $T$ in the domain, with **zero vacuum energy**.

Use the standard convention for a [supergravity auxiliary field](../../../supersymmetry.md#supergravity-auxiliary-field), $F^i=-e^{K/2}K^{i\bar j}\overline{D_jW}$. In this convention

$$
F^T=e^{K/2}t\bar W,\qquad F^C=-e^{K/2}\left[3\bar C^2+C(\bar C^3+\bar B)\right].
$$

At the $C=0$ minimum these become

$$
\boxed{F^T=\frac{\bar B}{\sqrt t},\qquad F^C=0.}
$$

Thus [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) occurs if $B\ne0$, despite the vanishing vacuum energy. Indeed $K_{T\bar T}|F^T|^2=3|B|^2/t^3$ is precisely canceled by the negative [gravitino](../../../supersymmetry.md#gravitino) contribution. **For $B=0$ the asserted breaking does not occur:** both [supergravity auxiliary fields](../../../supersymmetry.md#supergravity-auxiliary-field) vanish at $C=0$, so this vacuum is supersymmetric.

For completeness, the full set of finite zero-energy minima includes additional branches. For $C=re^{i\theta}\ne0$, the condition $D_CW=0$ reduces, after factoring $re^{-i\theta}$, to

$$
r(3+r^2)e^{3i\theta}=-B.
$$

For every $B\ne0$ there is a unique positive solution of $r(3+r^2)=|B|$, since the left side increases strictly from zero to infinity. There are three associated phases,

$$
\boxed{r(3+r^2)=|B|,\qquad \theta=\frac{\arg(-B)+2\pi k}{3},\quad k=0,1,2.}
$$

These also give $V=0$, and on each branch $W=3B/(3+r^2)\ne0$. Consequently $F^C=0$ but $F^T\ne0$, so these are also [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) [no-scale vacua with a cubic matter superpotential](../../../supersymmetry.md#no-scale-vacuum-with-a-cubic-matter-superpotential). A supersymmetric finite vacuum would require $D_TW=0$, hence $W=0$, and then $D_CW=3C^2=0$; this is possible only at $C=0$ with $B=0$.

The [scalar potential](../../../quantum-field-theory.md#scalar-potential) is independent of $\operatorname{Im}T$ everywhere. On every zero-energy vacuum branch it is also independent of $\operatorname{Re}T$, so **both real components of $T$ are [flat directions of a scalar potential](../../../quantum-field-theory.md#flat-direction-of-a-scalar-potential) at the vacuum**. Away from $D_CW=0$, the real direction is not flat: $\partial_tV=-3V/t$, giving a runaway towards $t\to\infty$ rather than a finite positive-energy stationary point. The zero-energy branches have no continuous [flat direction of a scalar potential](../../../quantum-field-theory.md#flat-direction-of-a-scalar-potential) in $C$; their allowed $C$ values are isolated. This is why the vacuum does not select a unique numerical [gravitino](../../../supersymmetry.md#gravitino) mass: the modulus $t$ is unfixed.

The [gravitino mass from a superpotential](../../../supersymmetry.md#gravitino-mass-from-a-superpotential) is $m_{3/2}=e^{K/2}|W|$. On the conventional $C=0$ branch,

$$
\boxed{m_{3/2}=\frac{|B|}{(T+\bar T)^{3/2}},\qquad V_{\min}=0.}
$$

On a nonzero-$C$ branch it is instead

$$
\boxed{m_{3/2}=\frac{3|B|e^{r^2/2}}{(3+r^2)t^{3/2}}.}
$$

When $B=0$, the only finite zero-energy matter solution is $C=0$ and $m_{3/2}=0$, with unbroken [supersymmetry](../../../supersymmetry.md). These results exhibit the distinction between vanishing vacuum energy and vanishing [supersymmetry breaking](../../../supersymmetry.md#supersymmetry-breaking) [auxiliary fields](../../../supersymmetry.md#auxiliary-field) in a [no-scale supergravity](../../../supersymmetry.md#no-scale-supergravity) model.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2007](../../2007.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
