<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Literal absence of new [interaction vertices](../../../../../../interaction-vertex.md) in the full [quantum effective action](../../../../../../effective-action.md) holds only for [Gaussian field theories](../../../../../../gaussian-field-theory.md).**

For every interacting $n\geq3$, the [one-loop scalar effective action](../../../../../../one-loop-scalar-effective-action.md) already contains counterexamples. On a constant background, with a positive auxiliary mass $\mu$ to control [infrared divergences](../../../../../../infrared-divergence.md), its field-dependent part is

$$
\Gamma_1[\phi]=\frac12\operatorname{Tr}\log\left[1+\frac{\lambda\phi^{n-2}}{(n-2)!(-\partial^2+\mu^2)}\right].
$$

The term of order $\lambda^V$ has $E=(n-2)V$ external [scalar fields](../../../../../../scalar-field.md) and is a one-loop polygon [one-particle-irreducible Feynman diagram](../../../../../../one-particle-irreducible-feynman-diagram.md). Choose $V>n/(n-2)$ and $2V>d$. Then $E>n$, its [loop momentum](../../../../../../loop-momentum.md) integral is ultraviolet convergent, and its coefficient is nonzero. Removing the [ultraviolet cutoff](../../../../../../ultraviolet-cutoff.md) does not remove this [finite higher-point scalar vertex](../../../../../../finite-higher-point-scalar-vertex.md). For $d>2$, generic nonexceptional external momenta give the same conclusion without retaining the auxiliary mass. In $d\leq2$, the massless theory still needs an infrared prescription; removing the ultraviolet cutoff does not remove that need or the induced vertices. Hence there are **no interacting pairs $(n,d)$ under the literal wording**. For $n=2$ the [functional determinant](../../../../../../functional-determinant.md) is field independent; $n=1$ merely shifts a [Gaussian integral](../../../../../../gaussian-integral.md) when an infrared prescription exists.

There is a different conventional interpretation: absence of new independent divergent [counterterms](../../../../../../counterterm.md). The [superficial degree of divergence](../../../../../../superficial-degree-of-divergence.md) of a connected diagram is

$$
D=dL-2I=d-\frac{d-2}{2}E-V[\lambda].
$$

The standard perturbative [counterterm closure](../../../../../../counterterm-closure.md) criterion is $[\lambda]\geq0$, with the same pairs as in part ii, provided one includes all symmetry-allowed lower-degree potential terms, the [kinetic term](../../../../../../kinetic-term.md), and the [vacuum energy](../../../../../../vacuum-energy.md). A pure monomial family need not itself have [counterterm closure](../../../../../../counterterm-closure.md): a sextic interaction in three dimensions generates a quartic [counterterm](../../../../../../counterterm.md), and a quartic interaction generates a [mass counterterm](../../../../../../mass-counterterm.md). This interpretation concerns the local divergent part or the continuum defining action, not the complete [quantum effective action](../../../../../../effective-action.md) with its finite [interaction vertices](../../../../../../interaction-vertex.md) and [derivative expansion](../../../../../../derivative-expansion.md).

For the massive four-dimensional [quartic scalar field theory](../../../../../../quartic-interaction.md), write $\lambda_B$ for the bare quartic coupling, $\lambda_R$ for its renormalized value, and $m>0$ for the mass held fixed by a [renormalization condition](../../../../../../renormalization-condition.md). Define the [scalar bubble integral](../../../../../../scalar-bubble-integral.md)

$$
B_\Lambda(P)=\int_{|q|<\Lambda}\frac{d^4q}{(2\pi)^4}\frac{1}{(q^2+m^2)((q+P)^2+m^2)}.
$$

The quartic [one-particle-irreducible correlation function](../../../../../../one-particle-irreducible-correlation-function.md), defined as a derivative of the Euclidean [quantum effective action](../../../../../../effective-action.md), is

$$
\Gamma_B^{(4)}(p_1,p_2,p_3,p_4)=\lambda_B-\frac{\lambda_B^2}{2}\left[B_{\Lambda_0}(p_1+p_2)+B_{\Lambda_0}(p_1+p_3)+B_{\Lambda_0}(p_1+p_4)\right]+O(\lambda_B^3),
\qquad \sum_i p_i=0.
$$

There are three [bubble diagrams](../../../../../../bubble-diagram.md), one for each pairing of external momenta, and each has [Feynman-diagram symmetry factor](../../../../../../feynman-diagram-symmetry-factor.md) $2$. The minus sign follows equivalently from the quadratic term in the [functional determinant](../../../../../../functional-determinant.md) $\tfrac12\operatorname{Tr}\log[1+(\lambda_B/2)(-\partial^2+m^2)^{-1}\phi^2]$.

Radial [integration](../../../../../../integral.md) at zero external momentum gives

$$
B_\Lambda(0)=\frac{1}{16\pi^2}\left[\log\left(1+\frac{\Lambda^2}{m^2}\right)+\frac{m^2}{\Lambda^2+m^2}-1\right].
$$

**The bare quartic vertex is not finite at fixed bare coupling.** Its logarithmic [ultraviolet divergence](../../../../../../ultraviolet-divergence.md) must be subtracted. Impose the [momentum-subtraction scheme](../../../../../../momentum-subtraction-scheme.md) condition $\Gamma_R^{(4)}(0,0,0,0)=\lambda_R$. To one loop this requires

$$
\lambda_B=\lambda_R+\frac{3\lambda_R^2}{2}B_{\Lambda_0}(0)+O(\lambda_R^3).
$$

For the finite difference, a [Feynman parameter](../../../../../../feynman-parameter.md) and a shift of [loop momentum](../../../../../../loop-momentum.md) give

$$
\lim_{\Lambda\to\infty}[B_\Lambda(P)-B_\Lambda(0)]=-\frac{1}{16\pi^2}\int_0^1du\,\log\left[1+\frac{u(1-u)P^2}{m^2}\right].
$$

The boundary error due to shifting a sharp cutoff vanishes in this limit. Substitution yields the finite [renormalized quartic scalar vertex](../../../../../../renormalized-quartic-scalar-vertex.md)

$$
\boxed{\Gamma_R^{(4)}=\lambda_R+\frac{\lambda_R^2}{32\pi^2}\sum_{P=p_1+p_2,\,p_1+p_3,\,p_1+p_4}\int_0^1du\,\log\left[1+\frac{u(1-u)P^2}{m^2}\right]+O(\lambda_R^3).}
$$

Thus finiteness requires holding the renormalized coupling fixed and allowing the bare coupling to depend on $\Lambda_0$. The unsubtracted assertion would be false.

The same [one-loop scalar effective action](../../../../../../one-loop-scalar-effective-action.md) explains the other effective interactions. For a constant background its expansion is

$$
\frac{\Gamma_1}{\mathrm{Vol}}=\sum_{r\geq1}\frac{(-1)^{r+1}}{2r}\left(\frac{\lambda_R}{2}\right)^r\phi^{2r}I_r(\Lambda_0),\qquad
I_r(\Lambda)=\int_{|q|<\Lambda}\frac{d^4q}{(2\pi)^4}\frac{1}{(q^2+m^2)^r}.
$$

The $r=1$ [tadpole diagram](../../../../../../tadpole-diagram.md) gives a mass correction $\delta m^2=\lambda_R I_1/2$, with

$$
I_1(\Lambda)=\frac{1}{16\pi^2}\left[\Lambda^2-m^2\log\left(1+\frac{\Lambda^2}{m^2}\right)\right].
$$

It requires a [mass counterterm](../../../../../../mass-counterterm.md). The field-independent [vacuum energy](../../../../../../vacuum-energy.md) also requires subtraction. The $r=2$ term is the quartic logarithm already treated. There is no one-loop [wave-function renormalization](../../../../../../wave-function-renormalization.md) from the quartic [tadpole diagram](../../../../../../tadpole-diagram.md).

For $r\geq3$ the polygon diagrams generate [finite higher-point scalar vertices](../../../../../../finite-higher-point-scalar-vertex.md), with

$$
\boxed{I_r(\infty)=\frac{\Gamma(r-2)}{16\pi^2\Gamma(r)}m^{4-2r}\quad(r\geq3).}
$$

For example, the induced sextic term in the [effective potential](../../../../../../effective-potential.md) is $+\lambda_R^3\phi^6/(768\pi^2m^2)$, or a six-point [interaction vertex](../../../../../../interaction-vertex.md) $15\lambda_R^3/(16\pi^2m^2)$ when normalized by $6!$. These finite terms survive the removal of the [ultraviolet cutoff](../../../../../../ultraviolet-cutoff.md) at fixed $m,\lambda_R$.

The external-momentum dependence of the [bubble diagrams](../../../../../../bubble-diagram.md) also generates a [derivative expansion](../../../../../../derivative-expansion.md) of quartic interactions. At small $P$, the subtracted [scalar bubble integral](../../../../../../scalar-bubble-integral.md) is $-P^2/(96\pi^2m^2)+O(P^4/m^4)$, giving finite derivative couplings. At order $\lambda_R^2$ these are the new field-dependent interactions beyond the mass and quartic terms; the sextic and higher [interaction vertices](../../../../../../interaction-vertex.md) require higher powers of $\lambda_R$, though they still occur at one loop. Such coefficients are suppressed by powers of the physical mass or external momentum, not by powers of $\Lambda_0$. The calculation establishes an order-by-order perturbative limit; it does not establish a nonperturbative interacting [continuum limit of a quantum field theory](../../../../../../continuum-limit-of-a-quantum-field-theory.md) in four dimensions.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 304](../../../paper-304-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
