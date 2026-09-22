<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\varepsilon=\varepsilon_a t_a$ and $A_\mu=A_{\mu a}t_a$. The proposed [gauge-field transformation law](../../../../../gauge-field-transformation-law.md) becomes $\delta A_\mu=-\partial_\mu\varepsilon+[\varepsilon,A_\mu]$. Consequently

$$
\delta(D_\mu\phi)=\varepsilon\partial_\mu\phi+(\partial_\mu\varepsilon)\phi+\delta A_\mu\phi+A_\mu\varepsilon\phi=\varepsilon D_\mu\phi.
$$

Both $\phi$ and its [gauge covariant derivative](../../../../../gauge-covariant-derivative.md) therefore transform as the same multiplet, with no derivative of the local parameter left over. The original algebraic invariance of the [Lagrangian density](../../../../../lagrangian-density.md) now applies pointwise to $\mathcal L(\phi,D\phi)$, so this constructs the local symmetry.

Also transform $J$ by $\delta J=\varepsilon J$. Antisymmetry gives $(t_aJ)\cdot\phi+J\cdot(t_a\phi)=0$, so the [source](../../../../../source-quantum-field-theory.md) coupling is invariant. Let $S_{A_{\mu a}}$ denote the [functional derivative](../../../../../functional-derivative.md) at a point. Vary the [action functional](../../../../../action.md) and integrate the derivative of $\varepsilon_a$ by parts, taking the local parameter to have compact support:

$$
\delta S=\int d^dx\,\varepsilon_a\left[(t_a\phi)\cdot S_\phi+(t_aJ)\cdot S_J+\partial_\mu S_{A_{\mu a}}+f_{abc}A_{\mu b}S_{A_{\mu c}}\right].
$$

Since every $\varepsilon_a(x)$ is arbitrary, its coefficient vanishes. This proves the requested local identity, including the derivative sign and the order of the structure-constant indices.

For the [generating functional](../../../../../generating-functional.md), the integral of the first term is zero as a change-of-variable identity:

$$
\int\mathcal D\phi\,(t_a\phi)\cdot\frac{\delta}{\delta\phi}e^{iS}=0.
$$

The divergence of this vector field in field space is proportional to $\operatorname{tr}t_a=0$. Thus an invariant regulated [functional measure](../../../../../functional-measure.md), with no [gauge anomaly](../../../../../gauge-anomaly.md), leaves no Jacobian term. Inserting the classical identity into the integral gives

$$
\boxed{\left[(t_aJ)\cdot\frac{\delta}{\delta J}+\partial_\mu\frac{\delta}{\delta A_{\mu a}}+f_{abc}A_{\mu b}\frac{\delta}{\delta A_{\mu c}}\right]Z[J,A]=0.}
$$

The same first-order differential operator annihilates the [connected generating functional](../../../../../connected-generating-functional.md) $W$, because $Z=e^{iW}$. Its [source](../../../../../source-quantum-field-theory.md) term is $(t_aJ)\cdot\varphi$.

For the specified [Legendre transform](../../../../../convex-conjugate.md), vary $\Gamma=-W+\int J\varphi$. Since $W_J=\varphi$, the terms involving $\delta J$ cancel, leaving

$$
\delta\Gamma=\int J\cdot\delta\varphi-\int W_A\,\delta A,\qquad \Gamma_\varphi=J,\qquad \left.\Gamma_A\right|_\varphi=-\left.W_A\right|_J.
$$

Antisymmetry also gives $(t_aJ)\cdot\varphi=-J\cdot(t_a\varphi)$. Substitution in the identity for $W$, followed by multiplication by $-1$, proves the [background gauge invariance of a scalar effective action](../../../../../background-gauge-invariance-of-a-scalar-effective-action.md):

$$
\boxed{\left[(t_a\varphi)\cdot\frac{\delta}{\delta\varphi}+\partial_\mu\frac{\delta}{\delta A_{\mu a}}+f_{abc}A_{\mu b}\frac{\delta}{\delta A_{\mu c}}\right]\Gamma=0.}
$$

The derivatives of the [quantum effective action](../../../../../effective-action.md) are proper, amputated [one-particle-irreducible vertices](../../../../../one-particle-irreducible-vertex.md). At each [loop order](../../../../../loop-order.md) they receive contributions from [one-particle-irreducible Feynman diagrams](../../../../../one-particle-irreducible-feynman-diagram.md) with the indicated external scalar legs, including tree vertices and the required [counterterms](../../../../../counterterm.md). Diagrams which disconnect after cutting one internal line are not additional proper-vertex contributions. Translation invariance supplies the overall momentum-conserving delta function factored out in the definition. The signs of these vertices must follow the chosen overall convention for $\Gamma$.

Differentiate the effective-action identity twice with respect to $\varphi_i(y)$ and $\varphi_j(z)$ and set $\varphi=A=0$. In an invariant zero-field vacuum this gives the [Ward identity contact terms](../../../../../ward-identity-contact-terms.md)

$$
\partial_\mu\Gamma^\mu_{a,ij}(x;y,z)+(t_a)_{ki}\delta(x-y)\Gamma^{(2)}_{kj}(x,z)+(t_a)_{kj}\delta(x-z)\Gamma^{(2)}_{ki}(x,y)=0.
$$

The term proportional to $A$ vanishes. With the printed Fourier factors $e^{ip_rx_r}$, integration by parts turns $\partial_\mu$ into $-ip_{1\mu}$. The first delta function combines $p_1$ with $p_2$, and the second combines $p_1$ with $p_3$. Using $(t_a)_{ki}=-(t_a)_{ik}$ and symmetry of the scalar two-point kernel then yields

$$
\boxed{p_{1\mu}\widehat\tau^\mu_{a,ij}=i(t_a)_{ik}\widehat\tau_{kj}(p_1+p_2,p_3)-\widehat\tau_{ik}(p_2,p_3+p_1)i(t_a)_{kj}.}
$$

This derivation fixes the relative signs independently of any vertex rule.

There is an overall-sign inconsistency in the final printed example. At tree level, stationarity of the [source](../../../../../source-quantum-field-theory.md) integral gives $W=S_0[\varphi,A]+\int J\varphi$, hence **the specified transform gives $\Gamma_{\mathrm{tree}}=-S_0$**. For the free scalar multiplet this implies, after factoring out the delta function,

$$
\widehat\tau_{ij}(p,-p)=(p^2+m^2)\delta_{ij},\qquad \boxed{\widehat\tau^\mu_{a,ij}=+i(p_2-p_3)^\mu(t_a)_{ij}.}
$$

The mixed result follows by expanding $-S_0$ to first order in $A$: its contribution is $\int A_{\mu a}(\partial^\mu\varphi_i)(t_a)_{ij}\varphi_j$. The two scalar derivatives yield $i p_2^\mu(t_a)_{ij}+i p_3^\mu(t_a)_{ji}$. [Momentum conservation](../../../../../momentum-conservation.md) gives

$$
p_1\cdot(p_2-p_3)=p_3^2-p_2^2,
$$

so both sides of the [Ward identity](../../../../../ward-identity.md) equal $i(p_3^2-p_2^2)(t_a)_{ij}$. Because the scalar theory is Gaussian for prescribed $A$, its fluctuation determinant depends on $A$ but not on $\varphi$; it cannot add further two-scalar vertices. Thus this quadratic verification is sufficient, not merely the first term of an omitted scalar-loop correction.

The printed mixed vertex instead has a minus sign. It satisfies the same [Ward identity](../../../../../ward-identity.md) if one uses the opposite effective-action convention $\Gamma_{\mathrm{alt}}=W-\int J\varphi=S_0$ at tree level, because its two-point vertex is then $-(p^2+m^2)\delta_{ij}$ as well. **Either overall convention works, but the printed [Legendre transform](../../../../../convex-conjugate.md) and printed mixed vertex cannot both be used unchanged.** For example, with $p_2^2\ne p_3^2$ and a nonzero generator, they give opposite sides of the claimed identity.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
