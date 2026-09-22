<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $h_{\mu\nu}=\partial_\mu X^a\partial_\nu X_a$ be the [induced worldvolume metric](../../../../../induced-worldvolume-metric.md) and write $H=\gamma^{\mu\nu}h_{\mu\nu}$. Varying the embedding in the [auxiliary-metric brane action](../../../../../auxiliary-metric-brane-action.md) and integrating by parts gives

$$
\boxed{\partial_\mu\!\left(\sqrt{-\gamma}\,\gamma^{\mu\nu}\partial_\nu X^a\right)=0.}
$$

The boundary contribution, including its relative factor, is

$$
\delta I\big|_{\partial\Sigma}
=2\int_{\partial\Sigma}\sqrt{|\gamma_\partial|}\,
n_\mu\gamma^{\mu\nu}\partial_\nu X_a\,\delta X^a.
$$

At initial and final times one fixes the endpoint configurations or uses variations of compact support. At a spatial boundary, free target directions require [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) $n_\mu\gamma^{\mu\nu}\partial_\nu X^a=0$; fixed directions require [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) $\delta X^a=0$. Mixed conditions must make this boundary pairing vanish. A closed [brane](../../../../../brane.md) has no spatial boundary. Since the [auxiliary worldvolume metric](../../../../../auxiliary-worldvolume-metric.md) enters without [derivatives](../../../../../derivative.md), its variation produces no extra boundary term.

Using $\delta\sqrt{-\gamma}=-(1/2)\sqrt{-\gamma}\gamma_{\mu\nu}\delta\gamma^{\mu\nu}$, variation of the inverse [worldvolume metric](../../../../../auxiliary-worldvolume-metric.md) gives

$$
\boxed{h_{\mu\nu}-\frac12\gamma_{\mu\nu}\{H-(p-1)\}=0.}
$$

Taking the trace yields $(p-1)(H-p-1)=0$. For $p\ne1$, this forces $H=p+1$, and substitution gives $\gamma_{\mu\nu}=h_{\mu\nu}$. For a nondegenerate timelike embedding, eliminating the [auxiliary worldvolume metric](../../../../../auxiliary-worldvolume-metric.md) therefore gives twice the [worldvolume](../../../../../worldvolume.md) area, with the overall physical [brane tension](../../../../../brane-tension.md) supplied by the action normalization.

For $p=1$, the traced metric equation is an identity, and the remaining equation only says $h_{\mu\nu}=(H/2)\gamma_{\mu\nu}$. It fixes the [worldsheet metric](../../../../../worldsheet-metric.md) up to a [Weyl transformation](../../../../../weyl-transformation.md), rather than determining it uniquely. Indeed $\sqrt{-\gamma}\gamma^{\mu\nu}$ is Weyl invariant precisely in two [worldvolume](../../../../../worldvolume.md) dimensions, and the constant term vanishes precisely at $p=1$. This is the [Weyl-invariance exception for the string among branes](../../../../../weyl-invariance-exception-for-the-string-among-branes.md). In a nondegenerate interior it gives the familiar [classical equivalence of Polyakov and Nambu–Goto actions](../../../../../classical-equivalence-of-polyakov-and-nambu-goto-actions.md); degeneracies at a free string endpoint must be treated through the original equations.

For the [open string](../../../../../open-string.md), choose [conformal gauge](../../../../../conformal-gauge.md) $\gamma_{\mu\nu}=\operatorname{diag}(-1,1)$ on $0\leq\sigma\leq\pi$. The embedding equation is the [wave equation](../../../../../wave-equation-split.md), and NN means $\partial_\sigma X^a=0$ at both spatial endpoints. For these operator formulas restore the conventional overall normalization $S=-TI/2$, with $T=(2\pi\alpha\prime)^{-1}$; the overall factor does not change the preceding classical equations. Its [open-string mode expansion](../../../../../open-string-mode-expansion.md) is

$$
X^a=x^a+2\alpha'p^a\tau+
i\sqrt{2\alpha'}\sum_{n\ne0}\frac{\alpha_n^a}{n}e^{-in\tau}\cos(n\sigma),
\qquad \alpha_0^a=\sqrt{2\alpha'}p^a.
$$

Reality requires $(\alpha_n^a)^\dagger=\alpha_{-n}^a$. [Canonical quantization](../../../../../canonical-quantization.md) gives

$$
[x^a,p^b]=i\eta^{ab},\qquad
[\alpha_m^a,\alpha_n^b]=m\eta^{ab}\delta_{m+n,0}.
$$

The metric equation is the vanishing of the [worldsheet stress tensor](../../../../../worldsheet-stress-energy-tensor.md): $(\partial_\tau X+\partial_\sigma X)^2=(\partial_\tau X-\partial_\sigma X)^2=0$. The two endpoint-compatible mode expansions contain the same [string oscillator](../../../../../string-oscillator.md) family. Their quadratic coefficients are the classical [Virasoro constraints](../../../../../virasoro-constraint.md).

For the operators, use [normal ordering](../../../../../normal-ordering.md) with positive-index [string oscillators](../../../../../string-oscillator.md) as annihilators:

$$
L_m=\frac12\sum_{n\in\mathbb Z}:\alpha_{m-n}\cdot\alpha_n:,
\qquad
L_0=\alpha'p^2+\sum_{n>0}\alpha_{-n}\cdot\alpha_n.
$$

Thus $(\partial_\tau X\pm\partial_\sigma X)^2$ has modes $4\alpha'L_m$ before the quantum ordering correction. The [physical-state Virasoro conditions for an open string](../../../../../physical-state-virasoro-conditions-for-an-open-string.md) are

$$
\boxed{L_m|\Phi\rangle=0\quad(m>0),\qquad
(L_0-a)|\Phi\rangle=0.}
$$

One imposes only the positive modes on kets, with the adjoint conditions on bras, as in [Gupta-Bleuler quantization](../../../../../gupta-bleuler-formalism.md). Requiring every positive and negative mode to annihilate the same state would conflict with the [Virasoro central extension](../../../../../virasoro-central-extension.md). The intercept $a$ is the zero-mode ordering constant. The standard critical [bosonic string theory](../../../../../bosonic-string-theory.md) has $d=26$ and $a=1$; in [light-cone gauge in string theory](../../../../../light-cone-gauge-in-string-theory.md) the transverse [zero-point energy](../../../../../zero-point-energy.md) gives $a=(d-2)/24$, while full anomaly-free Lorentz or [BRST quantization](../../../../../brst-quantization.md) fixes the critical values. The mass constraint is then $\alpha'M^2=N-a$, with $N=\sum_{n>0}\alpha_{-n}\cdot\alpha_n$.

To compute the [Virasoro algebra](../../../../../virasoro-algebra.md), commute a quadratic generator with one [string oscillator](../../../../../string-oscillator.md):

$$
[L_m,\alpha_n^a]=-n\alpha_{m+n}^a,\qquad [L_m,x^a]=-i\sqrt{2\alpha'}\alpha_m^a.
$$

These identities and the [Jacobi identity](../../../../../jacobi-identity.md) imply that $[L_m,L_n]-(m-n)L_{m+n}$ commutes with every [string oscillator](../../../../../string-oscillator.md) and with the center-of-mass coordinates and momenta. Mode number permits a scalar term only for $m+n=0$. Its coefficient follows from the formal zero-momentum [Fock vacuum](../../../../../fock-vacuum.md), on which $L_0=0$. For $m>0$,

$$
L_{-m}|0\rangle=\frac12\sum_{r=1}^{m-1}
\alpha_{-r}\cdot\alpha_{-(m-r)}|0\rangle.
$$

The two possible [string oscillator](../../../../../string-oscillator.md) contractions give

$$
\langle0|L_mL_{-m}|0\rangle
=\frac d2\sum_{r=1}^{m-1}r(m-r)
=\frac d{12}(m^3-m).
$$

The timelike target coordinate still contributes one to this [central charge](../../../../../central-charge.md): its two metric signs cancel in $\eta_{ab}\eta^{ab}=d$. Consequently

$$
\boxed{[L_m,L_n]=(m-n)L_{m+n}
+\frac d{12}m(m^2-1)\delta_{m+n,0}.}
$$

This is the [free-boson Virasoro central term](../../../../../free-boson-virasoro-central-term.md). It vanishes for the three global conformal modes $m=0,\pm1$.

To keep the intercept convention separate, define $\mathcal L_m=L_m-a\delta_{m,0}$. The [Virasoro zero-mode shift](../../../../../virasoro-zero-mode-shift.md) changes the displayed central term to

$$
[\mathcal L_m,\mathcal L_n]=(m-n)\mathcal L_{m+n}
+\left\{\frac d{12}m(m^2-1)+2am\right\}\delta_{m+n,0}.
$$

The matter [central charge](../../../../../central-charge.md) here is $d$, not $d-2$. Covariant [worldsheet ghost fields](../../../../../worldsheet-ghost-field.md) contribute $-26$; their inclusion cancels the anomaly at $d=26$, while the intercept is handled by the appropriate zero-mode and physical-state convention.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
