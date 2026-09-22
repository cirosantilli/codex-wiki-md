<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For the [relativistic particle phase-space action](../../../../../relativistic-particle-phase-space-action.md), the [first-class constraint](../../../../../first-class-constraint.md) $\varphi=(p^2+m^2)/2$ generates

$$
\boxed{\delta x^m=\epsilon(t)p^m,\qquad
\delta p_m=0,\qquad\delta e=\dot\epsilon(t).}
$$

Indeed the integrand varies by $\tfrac12\,d[\epsilon(p^2-m^2)]/dt$. The [canonical gauge transformation](../../../../../canonical-gauge-transformation.md) is an invariance when the gauge parameter vanishes at fixed temporal endpoints, or when all fields and the parameter are periodic. The boundary restriction matters for the [proper-time modulus](../../../../../proper-time-modulus.md).

Normalize the [worldline](../../../../../world-line.md) interval to $[0,1]$. Then

$$
s=\int_0^1 e(t)\,dt
$$

is invariant because $\delta s=\epsilon(1)-\epsilon(0)=0$. Every allowed $e$ in its orbit can be written $e(t)=s+\dot\epsilon(t)$: set $\epsilon(t)=\int_0^t[e(u)-s]du$. Thus **$s$ remains a gauge-invariant integration variable**, not another removable nonconstant mode. For a [worldline](../../../../../world-line.md) circle the constant gauge parameter is a residual zero mode. Without the endpoint restriction, the assertion that $s$ is invariant would not hold.

The [worldline gauge-orbit determinant](../../../../../worldline-gauge-orbit-determinant.md) is the Jacobian from gauge-orbit coordinates $\epsilon$ to the nonconstant part of $e$ is the [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) of $\partial_t$. Equivalently, the gauge-fixing identity has the form

$$
1=\Delta_{\mathrm{FP}}[e]\int\mathcal D\epsilon\,
\delta\big(e^\epsilon-s\big),\qquad
\Delta_{\mathrm{FP}}=\det{}'\partial_t.
$$

The determinant is taken between the appropriate boundary-condition spaces, with the modulus removed; on a circle the prime also removes the constant parameter. [Gauge fixing](../../../../../gauge-fixing.md) therefore leaves a factor $\det{}'\partial_t$ and a modulus measure, after division by any residual gauge volume. Even though this determinant is field independent in the present Abelian example, it is the required change-of-variables Jacobian. A [Grassmann integral](../../../../../berezin-integral.md) over the [Faddeev-Popov ghosts](../../../../../faddeev-popov-ghost.md) exponentiates it:

$$
\det{}'\partial_t\ \propto\ \int\mathcal Db\,\mathcal Dc\,e^{iI_{\mathrm{gh}}},\qquad
I_{\mathrm{gh}}=i\int_0^1dt\,b\dot c.
$$

The overall determinant phase depends on the integration convention and can be absorbed into normalization. Zero modes and the same endpoint restrictions must be treated separately rather than included in an invertible determinant.

For the free-ended [open string](../../../../../open-string.md), take $0\leq\sigma\leq\pi$. A canonical cosine expansion at a fixed time is

$$
X^m(\sigma)=x^m+\frac{i}{\sqrt{\pi T}}\sum_{n\ne0}\frac{\alpha_n^m}{n}\cos(n\sigma),\qquad
P_m(\sigma)=\frac{p_m}{\pi}+\sqrt{\frac T\pi}\sum_{n\ne0}\alpha_{nm}\cos(n\sigma).
$$

It implements the [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) and has $\alpha_n^\dagger=\alpha_{-n}$. With $\alpha_0^m=p^m/\sqrt{\pi T}$, its [Nambu-Goto phase-space action](../../../../../nambu-goto-phase-space-action.md), up to a total time derivative, is

$$
I=\int dt\left[p_m\dot x^m+\sum_{n>0}\frac{i}{n}\dot\alpha_n\cdot\alpha_{-n}
-\sum_{n\in\mathbb Z}\lambda_{-n}L_n^{\mathrm{cl}}\right],\qquad
L_n^{\mathrm{cl}}=\frac12\sum_{k\in\mathbb Z}\alpha_{n-k}\cdot\alpha_k.
$$

Reality requires $\lambda_{-n}=\lambda_n^*$. Numerical factors can be absorbed into these [Lagrange multipliers](../../../../../lagrange-multiplier.md). In this [covariant quantization of the bosonic string](../../../../../covariant-quantization-of-the-bosonic-string.md) the oscillators retain all $D$ spacetime components, in contrast to the transverse oscillators in the preceding solution. The [canonical commutation relations](../../../../../canonical-commutation-relation.md) are

$$
[x^m,p_n]=i\delta^m_n,\qquad
[\alpha_m^r,\alpha_n^s]=m\eta^{rs}\delta_{m+n,0}.
$$

The [oscillator vacuum](../../../../../oscillator-vacuum.md) $|0;p\rangle$ is annihilated by $\alpha_n^m$ for $n>0$. Its [momentum](../../../../../momentum.md) label will sometimes be suppressed.

Define the matter [Virasoro algebra](../../../../../virasoro-algebra.md) generators using [normal ordering](../../../../../normal-ordering.md):

$$
L_n=\frac12\sum_k:\!\alpha_{n-k}\cdot\alpha_k\!:,qquad
\boxed{L_0=\alpha'p^2+\sum_{k>0}\alpha_{-k}\cdot\alpha_k,quad
\alpha'=\frac1{2\pi T}.}
$$

No additive intercept is included in this definition of $L_0$. For $n>0$ the indices of the two factors in each term add to $n$; they cannot both be negative. After [normal ordering](../../../../../normal-ordering.md) there is a positive-mode [annihilation operator](../../../../../annihilation-operator.md) on the right, possibly accompanied by the zero mode. Hence **$L_n|0;p\rangle=0$ for every $n>0$**. In $L_0$, commuting positive modes past negative modes formally adds $\tfrac D2\sum_{k>0}k$. This divergent constant needs a prescription, and a finite shift is an ordering ambiguity. Our convention instead puts the physical [string intercept](../../../../../normal-ordering-constant-of-a-string.md) into the constraint $L_0-a$.

With this convention the matter [Virasoro algebra](../../../../../virasoro-algebra.md) is

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}
+\frac D{12}(m^3-m)\delta_{m+n,0}.}
$$

A different additive constant in $L_0$ would change the linear-in-$m$ central term, so stating the convention is essential.

For the [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md), use

$$
\{b_m,c_n\}=\delta_{m+n,0},\qquad
\{b_m,b_n\}=\{c_m,c_n\}=0,
$$

and choose a [ghost oscillator vacuum](../../../../../ghost-oscillator-vacuum.md) with

$$
b_n|0\rangle_{\mathrm{gh}}=c_n|0\rangle_{\mathrm{gh}}=0\quad(n>0),\qquad
b_0|0\rangle_{\mathrm{gh}}=0.
$$

Then $c_0|0\rangle_{\mathrm{gh}}\ne0$ since $\{b_0,c_0\}=1$. This choice specifies the ghost zero-mode doublet; it is not a claim that both zero modes annihilate one state. With the printed [ghost Virasoro zero-mode convention](../../../../../ghost-virasoro-zero-mode-convention.md), $L_0^{\mathrm{gh}}|0\rangle_{\mathrm{gh}}=0$ and $L_m^{\mathrm{gh}}|0\rangle_{\mathrm{gh}}=0$ for $m>0$. The latter follows by putting positive ghost modes on the right; a possible contraction requires $m=0$ and is absent here.

Apply the supplied [BRST charge](../../../../../brst-charge.md) to the matter state times this [ghost oscillator vacuum](../../../../../ghost-oscillator-vacuum.md). Terms with a rightmost $c_m$, $m>0$, vanish, as do the positive-mode ghost generators. Thus

$$
Q_{\mathrm{BRST}}(|\Psi\rangle\otimes|0\rangle_{\mathrm{gh}})
=(L_0-1)|\Psi\rangle\otimes c_0|0\rangle_{\mathrm{gh}}
+\sum_{m>0}L_m|\Psi\rangle\otimes c_{-m}|0\rangle_{\mathrm{gh}}.
$$

These one-ghost states are independent, as can also be seen by applying $b_0,b_m$. Therefore the [BRST physical-state constraints of an open string](../../../../../brst-physical-state-constraints-of-an-open-string.md) are

$$
\boxed{(L_0-1)|\Psi\rangle=0,\qquad L_m|\Psi\rangle=0\quad(m>0).}
$$

For the matter [oscillator vacuum](../../../../../oscillator-vacuum.md), $L_0=\alpha'p^2$, so $p^2=1/\alpha'$ and **$M^2=-1/\alpha'=-2\pi T$**: the physical ground state is a [tachyon](../../../../../tachyon.md). The [momentum](../../../../../momentum.md) must satisfy this equation; the zero-momentum [oscillator vacuum](../../../../../oscillator-vacuum.md) by itself would not be [BRST-closed](../../../../../brst-closed-operator.md).

Matter and ghost generators commute with one another. Add their two algebras and write $\mathcal L_m=L_m+L_m^{\mathrm{gh}}$. The given ghost constant must be retained:

$$
\boxed{[\mathcal L_m,\mathcal L_n]
=(m-n)(\mathcal L_{m+n}-\delta_{m+n,0})
+\frac{D-26}{12}(m^3-m)\delta_{m+n,0}.}
$$

Define the shifted generators $\widehat{\mathcal L}_m=\mathcal L_m-\delta_{m,0}$. Then

$$
[\widehat{\mathcal L}_m,\widehat{\mathcal L}_n]
=(m-n)\widehat{\mathcal L}_{m+n}
+\frac{D-26}{12}(m^3-m)\delta_{m+n,0}.
$$

[BRST nilpotence](../../../../../brst-nilpotence.md) requires cancellation of the anomalous central term in this shifted [constraint algebra](../../../../../constraint-algebra.md), together with the intercept one already present in the charge. At $m=2,n=-2$ the remaining anomalous coefficient is $(D-26)/2$, so **$D=26$**. At this value the shifted total generators obey the [Witt algebra](../../../../../witt-algebra.md). The unshifted $\mathcal L_m$ still have the displayed linear zero-mode shift; it must not be silently discarded.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
