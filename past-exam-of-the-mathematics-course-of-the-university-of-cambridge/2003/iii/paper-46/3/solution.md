<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Changing the [ultraviolet cutoff](../../../../../ultraviolet-cutoff.md) changes which fluctuations remain explicit. Integrating out a shell of [Fourier modes](../../../../../fourier-mode.md) shifts the coefficients of all symmetry-allowed operators and a field-independent constant. Hence the cutoff-dependent coefficients are chosen so that the remaining [partition function](../../../../../canonical-partition-function.md) and long-distance observables reproduce the same microscopic system. This is the [Wilsonian coarse-grained statistical Hamiltonian](../../../../../wilsonian-coarse-grained-statistical-hamiltonian.md); retaining only the printed operators is a [local derivative expansion](../../../../../local-derivative-expansion.md), not an exact closure.

In a massive symmetric phase, the quadratic long-wavelength inverse [two-point function](../../../../../two-point-correlation-function.md) has the form $\alpha^{-1}p^2+m^2$. Its [Landau scalar correlation length](../../../../../landau-scalar-correlation-length.md) satisfies $\xi^{-2}=\alpha m^2$ in this approximation. For [canonical normalization of a scalar gradient term](../../../../../canonical-normalization-of-a-scalar-gradient-term.md), set $\phi=\sqrt\alpha\,\psi$; then the mass and quartic coefficients become $r=\alpha m^2$ and $g_c=\alpha^2g$. With this normalization the infrared mass is the inverse [correlation length](../../../../../correlation-length.md), $m_R=\xi^{-1}$, within the massive quadratic or one-loop approximation. More generally the decay rate is a [pole mass](../../../../../pole-mass.md), whereas the zero-momentum inverse [magnetic susceptibility](../../../../../magnetic-susceptibility.md) is a curvature mass; an [anomalous dimension](../../../../../anomalous-dimension.md) or nontrivial momentum dependence can distinguish them. In the ordered phase one must first expand about a selected stable [equilibrium magnetization](../../../../../equilibrium-magnetization.md), rather than identify a negative quadratic coefficient at the unstable origin with a squared inverse [correlation length](../../../../../correlation-length.md). Thus the intended mass identification includes a field normalization and a stable-phase qualification.

For [momentum-shell renormalization group](../../../../../momentum-shell-renormalization-group.md), split $\phi=\phi_<+\phi_>$, retaining $|p|<\Lambda/b$ and eliminating $\Lambda/b<|p|<\Lambda$. Define

$$
e^{-H_{\mathrm{eff}}[\phi_<]}=\int\mathcal D\phi_>\,e^{-H[\phi_<+\phi_>]}.
$$

Taking a logarithm gives the [cumulant expansion of a coarse-grained free energy](../../../../../cumulant-expansion-of-a-coarse-grained-free-energy.md). For a centered fast [Gaussian measure](../../../../../gaussian-measure.md) with $G_>(0)=\langle\phi_>^2\rangle$, the first quartic cumulant is

$$
\frac g{4!}\int d^Dx\,\langle(\phi_<+\phi_>)^4\rangle_>
=\frac g{24}\int d^Dx\,[\phi_<^4+6G_>(0)\phi_<^2+3G_>(0)^2].
$$

The [Wick contractions](../../../../../wick-contraction.md) give a mass shift $\Delta r=gG_>(0)/2$ and an identity-operator contribution, while leaving the quartic term at this order. The second cumulant produces higher interactions and a quartic correction. After the length and field rescalings $x=bx'$ and $\phi_<(x)=b^{-(D-2)/2}\phi'(x')$, the gradient coefficient remains one, and

$$
r'=b^2\left[r+\frac g2G_>(0)+O(g^2)\right],\qquad
g'=b^{4-D}g+O(g^2),\qquad v'=b^{6-2D}v+\cdots.
$$

The [one-loop shell mass renormalization in scalar quartic theory](../../../../../one-loop-shell-mass-renormalization-in-scalar-quartic-theory.md) explicitly shows why the critical bare mass is shifted by fluctuations.

Assume short-range interactions, an analytic even local potential, a positive gradient coefficient, and a weak-coupling trajectory in the basin of the [Gaussian fixed point](../../../../../gaussian-fixed-point.md). Above four dimensions the quartic interaction has negative [engineering dimension](../../../../../engineering-dimension.md) and its dimensionless strength decreases under coarse graining; higher local powers and higher derivative terms also decrease. After absorbing analytic short-distance shifts into the coefficients, long-wavelength fluctuations are small compared with the ordered [order parameter](../../../../../order-parameter.md). The remaining coarse [Landau free energy](../../../../../landau-free-energy.md) can therefore be evaluated at its stable saddle:

$$
\mathcal F_{\mathrm L}[M]=\int d^Dx\left[\frac12(\nabla M)^2+\frac12r_R(T)M^2+\frac{g_R}{4!}M^4-hM+\cdots\right].
$$

The quartic stabilizer must still be retained for the ordered minimum even though it is [dangerously irrelevant](../../../../../dangerously-irrelevant-coupling.md). Stationarity, $r_RM+g_RM^3/6=h$, gives the ordinary [Landau-Ginzburg theory](../../../../../landau-ginzburg-theory.md) and its [mean-field critical exponents](../../../../../mean-field-critical-exponent.md). This derives the saddle approximation from decreasing fluctuation strength under the stated RG assumptions; it does not assume that every exact coarse-grained functional becomes a quartic polynomial. Below four dimensions the quartic coupling grows, long-wavelength loop corrections cease to be small, and the argument fails. At four dimensions the interaction is marginal and generates logarithmic corrections. The tuned sextic theory has the analogous boundary at three dimensions.

Use a consistent [Fourier transform](../../../../../fourier-transform.md) pair for the [connected correlation function](../../../../../connected-correlation-function.md):

$$
\widetilde G(p)=\int d^Dx\,e^{-ip\cdot x}G_c(x),\qquad
G_c(x)=\int\frac{d^Dp}{(2\pi)^D}e^{ip\cdot x}\widetilde G(p).
$$

The printed forward-transform expression integrates over $p$ while leaving $x$ free; that integration variable is an error. The above convention resolves it and produces the loop measure used below. At zero [magnetization](../../../../../magnetization.md), $G_c(x)=\langle\phi(0)\phi(x)\rangle$; otherwise the disconnected product of expectations must be subtracted.

In the inverse-propagator identity used here, the truncated two-point function means the full [one-particle-irreducible two-point vertex](../../../../../one-particle-irreducible-two-point-vertex.md), including its free quadratic part. This convention differs from using “truncated” for a connected cumulant. To derive the inverse relation, introduce $W[J]=\log Z[J]$, $\varphi=\delta W/\delta J$ and the [effective action](../../../../../effective-action.md) $\Gamma[\varphi]=\int J\varphi-W[J]$. Then $\delta\Gamma/\delta\varphi=J$ and the chain rule gives $\Gamma^{(2)}W^{(2)}=1$. Since $W^{(2)}$ is the [connected correlation function](../../../../../connected-correlation-function.md), translation invariance gives **$\widetilde\Gamma(p)=\widetilde G(p)^{-1}$**.

Now use canonically normalized coefficients, denoting the cutoff mass by $m_b^2=m^2(\Lambda,T)$ and the renormalized infrared mass by $m_R^2=m^2(0,T)$. Choose the free [propagator](../../../../../propagator.md) $\widetilde G_0(p)=(p^2+m_R^2)^{-1}$ and put $\delta m^2=m_b^2-m_R^2$ in the interaction as a quadratic [counterterm](../../../../../counterterm.md). With the Euclidean [self-energy](../../../../../self-energy.md) convention in which an insertion changes the connected propagator by $-G_0\Sigma G_0$, the perturbative series begins

$$
\widetilde G=\widetilde G_0-\widetilde G_0(\delta m^2+\Sigma)\widetilde G_0+\cdots,
\qquad
\boxed{\widetilde\Gamma(p)=p^2+m_R^2+\delta m^2+\Sigma(p).}
$$

The [self-energy](../../../../../self-energy.md) sums one-particle-irreducible loop insertions; the explicit mass [counterterm](../../../../../counterterm.md) is kept separate. Repeated insertions generate the geometric [Dyson resummation](../../../../../dyson-resummation.md), which explains why reducible chains occur in $G$ but not as independent terms in its inverse. Beyond one loop a momentum-dependent [self-energy](../../../../../self-energy.md) and [wave-function renormalization](../../../../../wave-function-renormalization.md) must also be included.

At one loop the only quartic two-point graph is the [tadpole diagram](../../../../../tadpole-diagram.md). At a $g\phi^4/4!$ vertex, attaching the two labeled external fields uses $4\cdot3=12$ choices and contracts the remaining two fields together. The factor is $12/4!=1/2$. Equivalently this is the same quadratic term in the shell [cumulant expansion](../../../../../cumulant-expansion.md) above. Thus

$$
\Sigma^{(1)}(p)=\frac g2 I_D(m_R^2;\Lambda),\qquad
I_D(R;\Lambda)=\int_{|k|<\Lambda}\frac{d^Dk}{(2\pi)^D}\frac1{k^2+R}.
$$

It is positive for $g>0$ and independent of external momentum, so there is no one-loop gradient renormalization. The condition $\widetilde\Gamma(0)=m_R^2$ implies $\delta m^2+\Sigma(0)=0$, hence

$$
\boxed{m_R^2=m_b^2+\frac g2\int_{|k|<\Lambda}\frac{d^Dk}{(2\pi)^D}\frac1{k^2+m_R^2}+O(g^2).}
$$

The cutoff is necessary: the unregulated integral is ultraviolet divergent for $D\geq2$. Using the renormalized mass internally is a self-consistent one-loop organization, not an exact resummation of all critical fluctuations. With nonunit $\alpha$, this formula instead applies to $r=\alpha m^2$, $g_c=\alpha^2g$ after [canonical normalization of a scalar gradient term](../../../../../canonical-normalization-of-a-scalar-gradient-term.md).

To test a linear thermal mass, approach the ordinary transition from the symmetric side and set $R=m_R^2>0$. For $D>2$ the massless tadpole is infrared finite. Subtract its critical value, absorb regular temperature dependence of the coupling into a nonzero thermal coefficient $A$, and write $m_b^2(T)-m_b^2(T_C)=A(T-T_C)+\cdots$. The [one-loop critical-mass subtraction](../../../../../one-loop-critical-mass-subtraction.md) gives

$$
R=A(T-T_C)+\frac g2[I_D(R)-I_D(0)],\qquad
\boxed{R\left[1+\frac g2J_D(R)\right]=A(T-T_C),}
$$

where

$$
J_D(R)=\int_{|k|<\Lambda}\frac{d^Dk}{(2\pi)^D k^2(k^2+R)}
=c_D\int_0^\Lambda\frac{k^{D-3}}{k^2+R}\,dk,\qquad
c_D=\frac{S_{D-1}}{(2\pi)^D}.
$$

For $D>4$, $J_D(0)=c_D\Lambda^{D-4}/(D-4)$ is finite, so the bracket tends to a finite constant and $R\propto T-T_C$ is self-consistent. At $D=4$,

$$
J_4(R)=\frac{1}{16\pi^2}\log\frac{\Lambda^2+R}{R},
$$

and the growing logarithm obstructs an asymptotically constant linear coefficient at nonzero coupling. For $2<D<4$, put $k=\sqrt R\,q$ to obtain

$$
J_D(R)\sim c_D R^{(D-4)/2}\int_0^\infty\frac{q^{D-3}}{1+q^2}\,dq
=c_D R^{(D-4)/2}\frac\pi2\csc\frac{\pi(D-2)}2.
$$

The divergent bracket then invalidates the assumed linear thermal mass. The [radial critical-mass subtraction in dimensions three to five](../../../../../radial-critical-mass-subtraction-in-dimensions-three-to-five.md) gives explicit checks of all three behaviors. For $D\leq2$, the massless tadpole subtraction itself is infrared divergent; that failure of the Gaussian expansion does not prove absence of an interacting transition. Therefore the ordinary **[upper critical dimension](../../../../../upper-critical-dimension.md) is $D_C=4$**, with the unmodified [Landau-Ginzburg theory](../../../../../landau-ginzburg-theory.md) asymptotically justified by this test only for $D>4$. Exponents inferred by solving the self-consistent one-loop equation below four dimensions would not be exact interacting exponents.

For a [tricritical point](../../../../../tricritical-point.md) the renormalized quartic coefficient must be tuned to zero, and a positive sextic interaction stabilizes the [order parameter](../../../../../order-parameter.md). The gradient term gives the [scalar field](../../../../../scalar-field.md) [engineering dimension](../../../../../engineering-dimension.md) $(D-2)/2$. A coefficient of $\phi^6$ therefore has dimension $D-6(D-2)/2=6-2D$, which becomes marginal at $D=3$. This gives **$D_C^{\mathrm{tri}}=3$**. A direct [Ginzburg criterion](../../../../../ginzburg-criterion.md) reaches the same result: long-wavelength variance in a [correlation volume](../../../../../correlation-volume.md) is

$$
\langle(\delta M)^2\rangle_\xi\sim\int_{|k|\lesssim\xi^{-1}}\frac{d^Dk}{k^2+\xi^{-2}}
\sim\xi^{2-D}\sim |r|^{(D-2)/2},
$$

while the tricritical saddle has $M^2\sim|r|^{1/2}$. Their ratio scales as $|r|^{(D-3)/2}$, vanishing only above three dimensions. At three dimensions it is marginal; below three it grows. In contrast the ordinary saddle $M^2\sim|r|/g$ gives a ratio $g|r|^{(D-4)/2}$. Both calculations assume the thermal mass is measured relative to its shifted critical value. A sextic interaction generates quartic terms under coarse graining, so tricriticality requires tuning the renormalized quartic scaling field as well as the mass.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
