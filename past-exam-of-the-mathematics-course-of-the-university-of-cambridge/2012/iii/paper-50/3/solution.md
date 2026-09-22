<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Loop integrals require a subtraction prescription. Even when the classical [coupling constant](../../../../../coupling-constant-physics.md) is dimensionless and there is no mass, specifying its renormalized value means specifying a [momentum](../../../../../momentum.md) or length scale at which it is measured. Dimensionless logarithms then involve that [renormalization scale](../../../../../renormalization-scale.md) $\mu$. Changing $\mu$ changes the renormalized [coupling constant](../../../../../coupling-constant-physics.md) and [wave-function renormalization](../../../../../wave-function-renormalization.md) while leaving bare quantities fixed. In a theory whose [renormalization-group beta function](../../../../../beta-function-physics.md) and [anomalous dimension](../../../../../anomalous-dimension.md) both vanish, this scale dependence may disappear; the generic statement concerns the interacting renormalized theory.

Write $\phi_B=Z_\phi^{1/2}\phi_R$ and $G_{n,R}=Z_\phi^{-n/2}G_{n,B}$. Define

$$
\beta(g)=\left.\mu\frac{dg}{d\mu}\right|_{\mathrm{bare}},\qquad
\gamma_\phi(g)=\left.\frac12\mu\frac{d\log Z_\phi}{d\mu}\right|_{\mathrm{bare}}.
$$

Bare [correlation functions](../../../../../correlation-function.md) do not depend on the arbitrary subtraction scale. Differentiating their relation to renormalized [correlation functions](../../../../../correlation-function.md) gives the [Callan-Symanzik equation](../../../../../callan-symanzik-equation.md)

$$
\boxed{\left(\mu\partial_\mu+\beta(g)\partial_g+n\gamma_\phi(g)\right)G_{n,R}=0.}
$$

It expresses the compensation between explicit scale dependence, [running coupling](../../../../../running-coupling.md) and [wave-function renormalization](../../../../../wave-function-renormalization.md). In this convention the field [scaling dimension](../../../../../scaling-dimension.md) is its [engineering dimension](../../../../../engineering-dimension.md) plus $\gamma_\phi$ at a fixed point; the critical-exponent notation $\eta$ often used for the [anomalous dimension](../../../../../anomalous-dimension.md) equals $2\gamma_\phi$.

A [renormalization-group fixed point](../../../../../renormalization-group-fixed-point.md) satisfies $\beta(g_*)=0$. It is ultraviolet attractive if the flow approaches it as $\mu\to\infty$, and infrared attractive if the flow approaches it as $\mu\to0$. For a simple isolated zero, $\delta g\propto\mu^{\beta'(g_*)}$: a negative derivative gives ultraviolet attraction, a positive derivative infrared attraction. Marginal zeros, such as a cubic [renormalization-group beta function](../../../../../beta-function-physics.md) at the origin, require looking at the first nonzero nonlinear term.

Put $z=p^2/\mu^2>0$, $t=\tfrac12\log z$, and write the dimensionless [quantum field theory propagator](../../../../../propagator.md) factor as $d(z,g)$. The two-point [Callan-Symanzik equation](../../../../../callan-symanzik-equation.md) becomes

$$
\left(-\partial_t+\beta(g)\partial_g+2\gamma_\phi(g)\right)d(e^{2t},g)=0.
$$

Let $\bar g(0)=g$ and $d\bar g/dt=\beta(\bar g)$. The [renormalization-group characteristic solution for a two-point function](../../../../../renormalization-group-characteristic-solution-for-a-two-point-function.md) is

$$
\boxed{d(e^{2t},g)=d(1,\bar g(t))
\exp\left[2\int_0^t\gamma_\phi(\bar g(s))\,ds\right].}
$$

Where $\beta\ne0$, the exponent is $2\int_g^{\bar g(t)}\gamma_\phi(u)/\beta(u)\,du$. Thus the ultraviolet behavior depends on where the [running coupling](../../../../../running-coupling.md) goes and on the [anomalous dimension](../../../../../anomalous-dimension.md) accumulated along the flow. A weak [ultraviolet fixed point](../../../../../ultraviolet-fixed-point.md) or asymptotically free limit permits perturbative evaluation; a flow to large values of the [coupling constant](../../../../../coupling-constant-physics.md) does not.

For $\beta(g)=-bg^3$ and $\gamma_\phi=cg^2$, $b>0$,

$$
\bar g(t)^2=\frac{g^2}{1+2bg^2t},\qquad
2\int_0^t c\bar g(s)^2\,ds=\frac cb\log(1+2bg^2t).
$$

Consequently

$$
\boxed{d(z,g)=d(1,\bar g(\tfrac12\log z))\,[1+bg^2\log z]^{c/b}.}
$$

For large positive $z$, the [coupling constant](../../../../../coupling-constant-physics.md) tends to zero. If the normalization function $d(1,g)$ has a finite nonzero free-field limit $d(1,0)$, then $d(z,g)\sim d(1,0)[bg^2\log z]^{c/b}$. Equivalently, with $\Lambda=\mu\exp[-1/(2bg^2)]$,

$$
\bar g^2=\frac1{b\log(p^2/\Lambda^2)},\qquad
d(z,g)\sim d(1,0)\left[\frac{\log(p^2/\Lambda^2)}{\log(\mu^2/\Lambda^2)}\right]^{c/b}.
$$

The positive exponent follows from the sign of $+n\gamma_\phi$ in the printed RG equation; changing the [field-renormalization anomalous dimension](../../../../../field-renormalization-anomalous-dimension.md) convention would change both signs together.

For the quintic [renormalization-group beta function](../../../../../beta-function-physics.md), set $B=-b>0$ and rename its positive quintic coefficient $A$ to avoid confusion with the later gauge-theory [coupling constant](../../../../../coupling-constant-physics.md). Then $\beta(g)=g^3(B-Ag^2)$ has a nonzero fixed point

$$
g_*^2=\frac BA,\qquad \beta'(g_*)=-\frac{2B^2}{A}<0.
$$

Every nonzero positive [running coupling](../../../../../running-coupling.md) in the perturbative basin approaches this **[ultraviolet fixed point](../../../../../ultraviolet-fixed-point.md)**, rather than approaching zero. The zero [coupling constant](../../../../../coupling-constant-physics.md) is infrared attractive. If the same $\gamma_\phi=cg^2$ is retained, the large-momentum factor is $d(z,g)\sim C z^{cB/A}$, assuming a regular nonzero matching factor at the fixed point. More generally the exponent is $\gamma_\phi(g_*)$. A fixed point at a large [coupling constant](../../../../../coupling-constant-physics.md) inferred from a truncated [renormalization-group beta function](../../../../../beta-function-physics.md) is only a formal extrapolation; perturbative control requires $B/A$ small.

For the gauge theory use the supplied convention $a=g^2/(16\pi^2)$ and evolution variable $L=\log\mu^2$. Asymptotic freedom requires $\beta_0>0$, or $n<11N/2$. To one-loop accuracy,

$$
\frac{da}{dL}=-\beta_0a^2,\qquad
\boxed{a(\mu^2)=\frac1{\beta_0\log(\mu^2/\Lambda^2)}.}
$$

The integration constant $\Lambda$ is an example of [dimensional transmutation](../../../../../dimensional-transmutation.md). With two loops this is the leading asymptotic expression, not an exact equality: if $\mathcal L=\log(\mu^2/\Lambda^2)$ is large,

$$
a=\frac1{\beta_0\mathcal L}
\left[1-\frac{\beta_1}{\beta_0^2}\frac{\log\mathcal L}{\mathcal L}+O(\mathcal L^{-1})\right].
$$

The expansion presumes fixed coefficients and a scale high enough to enter the ultraviolet regime.

Choose $n=11N/2-\delta$ with $0<\delta\ll N$, respecting integer flavor counts. The supplied coefficients become

$$
\beta_0=\frac23\delta,\qquad
\beta_1=-\frac{25}{2}N^2+\frac{11}{2}
+\left(\frac{13}{3}N-\frac1N\right)\delta.
$$

Thus $\beta_1<0$ for sufficiently small $\delta/N$, and the two-loop flow has the [Banks-Zaks fixed point](../../../../../banks-zaks-fixed-point.md)

$$
\boxed{a_*=-\frac{\beta_0}{\beta_1}\simeq\frac{4\delta}{75N^2}.}
$$

Both $a_*$ and the loop-counting combination $Na_*$ are small. Its slope is $\beta'(a_*)=-\beta_0^2/\beta_1>0$, so it is **infrared attractive**. For even large $N$, taking $n=11N/2-1$ provides an explicit integer sequence with the desired parametric hierarchy. As a finite example, $N=3,n=16$ gives $\beta_0=1/3$, $\beta_1=-302/3$ and $a_*=1/302$. The fermion-count convention is the one encoded by the given coefficients.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 50](../../paper-50-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
