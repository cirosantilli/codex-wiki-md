<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Write $q=bu$, $\rho=\rho_\infty$ and $r=\rho-\rho_s>0$. The first balance is depth-integrated [momentum conservation](../../../../../momentum-conservation.md). Its left side is the downstream increase of horizontal [momentum](../../../../../momentum.md) flux. The wind contributes the applied [stress](../../../../../stress.md) $S$; the remaining term is the resultant hydrostatic force associated with the sloping base of the light layer. Because $\overline\rho-\rho<0$, that term opposes the wind when $b'>0$.

For a strip of unit alongshore width and length $dx$, let $E=q'$ be the entrained ocean-volume flux per unit area. Ocean entering the layer carries [temperature](../../../../../temperature.md) $T_\infty$ and [concentration](../../../../../concentration.md) $C_\infty$ but no horizontal [momentum](../../../../../momentum.md) in this model. Take the reference liquid [enthalpy](../../../../../enthalpy.md) at $T_\infty$ to be zero and set

$$
e=c_p(T-T_\infty)-L\phi.
$$

The latent term is negative because ice has lower [enthalpy](../../../../../enthalpy.md) than liquid at the same [temperature](../../../../../temperature.md). The incoming entrained water has zero relative [enthalpy](../../../../../enthalpy.md), and the outgoing minus incoming horizontal [enthalpy](../../../../../enthalpy.md) flux is $[eq]'dx$. Atmospheric heat loss therefore gives $[eq]'=-f$. Similarly, solute conservation gives

$$
[\overline Cq]'=C_\infty E=C_\infty q',
\qquad\boxed{[(\overline C-C_\infty)q]'=0.}
$$

These are the second and third balances. Their reference-flux form has already subtracted the heat and solute brought in by [entrainment](../../../../../fluid-entrainment.md); those fluxes must not be subtracted again.

There is a dimensional normalization to make explicit. With the printed _specific_ $c_p,L$, the physical heat-flux balance is $\rho[eq]'=-F_{\rm phys}$. Thus $f=F_{\rm phys}/\rho$. The displayed exam equation uses its symbol $F$ for $f$, or implicitly works with density-normalized [heat flux](../../../../../heat-flux-density.md). The derivation below uses $f$ to keep these two meanings distinct.

With no incoming coastal jet or ice source, the conditions at $x=0$ are

$$
q\longrightarrow0,\qquad \rho bu^2\longrightarrow0,\qquad
eq\longrightarrow0,\qquad (\overline C-C_\infty)q\longrightarrow0.
$$

The regular emerging layer also has $T\to T_\infty$, $\phi\to0$, $\overline C\to C_\infty$ and $b\to0$. Prescribed nonzero inlet fluxes would replace these conditions and destroy the coast-origin power law. A zero-thickness coast does not justify independently prescribing an arbitrary nonzero velocity there.

Integration of the solute and [enthalpy](../../../../../enthalpy.md) balances yields $\overline C=C_\infty$ wherever $q>0$, and $eq=-fx$. Local phase equilibrium now gives

$$
C=\frac{C_\infty}{1-\phi},\qquad
T=-\frac{mC_\infty}{1-\phi},\qquad
\left[L+\frac{c_pmC_\infty}{1-\phi}\right]\phi q=fx.
$$

For $\phi\ll1$, put

$$
H=L+c_pmC_\infty,\qquad K=\frac fH,\qquad J=\frac{3S}{4\rho}.
$$

To leading order, $\phi q=Kx$. The potential-energy closure implies $rg\phi bb'=S/4$, and substituting it in the [momentum](../../../../../momentum.md) equation gives

$$
\rho(bu^2)'=S-rg\phi bb'=\frac{3S}{4},
\qquad bu^2=Jx.
$$

Dividing the ice flux by this last relation gives $\phi=(K/J)u$. If $b\propto x^p$, $u\propto x^q$, [momentum](../../../../../momentum.md) gives $p+2q=1$, while the potential-energy balance gives $2p+q=1$. Thus $p=q=1/3$. Substitution fixes the coefficients:

$$
\boxed{
 u=\left(\frac{rgK}{\rho}x\right)^{1/3},\qquad
 b=\frac{Jx}{u^2},\qquad
 \phi=\frac KJ u.
}
$$

This is the [dilute frazil polynya similarity solution](../../../../../dilute-frazil-polynya-similarity-solution.md). In particular, all three variables grow as $x^{1/3}$, $q$ grows as $x^{2/3}$, and the solution stops being dilute when $\phi$ is no longer small. [Density](../../../../../density.md) differences have been retained in [buoyancy](../../../../../buoyancy.md), but not in inertia or the normalized heat capacity.

To account for upward settling, one must distinguish retained suspension from crystals that leave it. A consistent depth-averaged extension has an upward exported ice-volume flux $R$ and an [entrainment](../../../../../fluid-entrainment.md) flux $E$. If all phases retain the same mean horizontal velocity within the layer, its balances become

$$
\begin{aligned}
q'&=E-R,\\
[\overline Cq]'&=C_\infty E,\\
[eq]'&=-f-R e_s,\qquad e_s=c_p(T-T_\infty)-L,\\
\rho(qu)'&=S-rg\phi bb'-\rho R u.
\end{aligned}
$$

The last term removes the [momentum](../../../../../momentum.md) carried out by the ice; its [density](../../../../../density.md) may be restored to $\rho_s$ outside the Boussinesq approximation. Consequently

$$
\boxed{[(\overline C-C_\infty)q]'=C_\infty R,}
$$

so one may no longer set $\overline C=C_\infty$. The local equilibrium relations are unchanged, but use the new bulk [concentration](../../../../../concentration.md). The [frazil export enthalpy balance](../../../../../frazil-export-enthalpy-balance.md) also shows why a simple replacement $-f\mapsto-f-LR$ has the wrong sign: exported ice carries negative relative [enthalpy](../../../../../enthalpy.md).

A slip speed $w$ requires a vertical particle-flux closure, for example $R=w\phi$ for a well-mixed top boundary. A nonuniform suspension instead requires its [surface](../../../../../topological-surface.md) [concentration](../../../../../concentration.md) and [buoyancy](../../../../../buoyancy.md) moment. The potential-energy closure must then include the gravitational energy released by rising light crystals, with scale $rgw\phi b$, and any energy and [buoyancy](../../../../../buoyancy.md) moment carried through the boundaries. For example, a well-mixed closure that transfers a fraction $\eta$ of this released power to [entrainment](../../../../../fluid-entrainment.md) and neglects additional boundary potential-energy transport would replace the original work balance by

$$
\frac14Su+\eta rgw\phi b=rg\phi bu b'.
$$

The allocation $\eta$ and exported potential-energy flux are extra closure information, not supplied constants of the original model. The original work balance cannot be retained unchanged while treating settling as an additional loss of suspended ice. Phase-dependent horizontal speeds would also replace $q\phi$ and $q(1-\phi)$ by their separate phase fluxes.

It is important to compare _total production_, not merely the retained ice flux. Let

$$
I(x)=\phi q,\qquad R_*(x)=\int_0^xR(\xi)d\xi,\qquad
P(x)=I(x)+R_*(x).
$$

Integrated solute conservation gives $C(q-I)=C_\infty(q+R_*)$, hence

$$
C-C_\infty=\frac{C_\infty P}{q-I}
=\frac{C_\infty P}{q}+\text{higher dilute-order terms}.
$$

Integrating the heat balance, and neglecting products of the small [concentration](../../../../../concentration.md) departure with the exported flux, gives

$$
\boxed{HP=fx,\qquad P'=f/H}
$$

to dilute order, provided the total processed fraction $P/q$, not only the retained fraction $\phi$, remains small. Thus upward settling reduces retained suspension, **but does not increase the leading-order total production at fixed atmospheric heat loss**. Beyond that order, efficient removal can reduce the subsequent sensible cooling of crystals and enhance mixing of ocean water; the usual expectation is a larger latent-heat fraction and hence greater production. Its amount, or an unconditional larger/smaller claim, needs the settling, mixing and surface-export closures just identified. At fixed $f$, energy conservation bounds the production by the available heat loss; it must not be inferred simply by observing fewer suspended crystals.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
