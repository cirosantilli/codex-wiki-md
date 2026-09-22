# Buffer capacity of a monoprotic acid

↑ **Parent:** [Buffer capacity](buffer-capacity.md)

Assume an ideal dilute aqueous [chemical solution](solution-chemistry.md) with just one [monoprotic acid](monoprotic-acid.md) pair $\mathrm{HA}/\mathrm A^-$, [self-ionization of water](self-ionization-of-water.md), and other [ions](ion.md) that balance [electric charge](electric-charge-split.md) without undergoing further [chemical reactions](chemical-reaction-split.md). Hold the [analytical concentration](analytical-concentration.md) $C=[\mathrm{HA}]+[\mathrm A^-]$ constant. Keep the [acid dissociation constant](acid-dissociation-constant.md) $K_a$ and the [self-ionization of water](self-ionization-of-water.md) constant $K_w$ [dimensionless](dimensionless-quantity.md), consistently with [pH](ph.md):

$$
c^\circ=1\,\mathrm{mol\,L^{-1}},\qquad H=10^{-\mathrm{pH}}=\frac{[\mathrm H^+]}{c^\circ},\qquad K_w=\frac{[\mathrm H^+][\mathrm{OH}^-]}{(c^\circ)^2}.
$$

Thus $H$ denotes normalized [hydrogen ion](hydrogen-ion.md) [concentration](concentration.md), not a dimensional [concentration](concentration.md). The [chemical equilibrium](chemical-equilibrium.md) and conserved [analytical concentration](analytical-concentration.md) give

$$
[\mathrm A^-]=\frac{C K_a}{K_a+H},\qquad [\mathrm{OH}^-]=\frac{c^\circ K_w}{H},\qquad [\mathrm H^+]=c^\circ H.
$$

Adding [chemical base](base-chemistry.md) converts [weak acid](weak-acid.md) to [conjugate base](conjugate-base.md), increases free [hydroxide](hydroxide.md), and decreases free [hydrogen ion](hydrogen-ion.md) [concentration](concentration.md). Balancing [electric charge](electric-charge-split.md), including the added reagent's accompanying [ions](ion.md), gives the signed dose relative to any initial [chemical equilibrium](chemical-equilibrium.md) at $p_0$:

$$
b(p)-b(p_0)=Q(p)-Q(p_0),\qquad Q(p)=[\mathrm A^-]+[\mathrm{OH}^-]-[\mathrm H^+].
$$

Differentiate with respect to [pH](ph.md), using $\mathrm dH/\mathrm dp=-(\ln10)H$. The result is

$$
\boxed{\beta=(\ln10)\left(\frac{C K_a H}{(K_a+H)^2}+c^\circ H+\frac{c^\circ K_w}{H}\right).}
$$

The first term is the [monoprotic acid](monoprotic-acid.md) pair's contribution, $\beta_{\mathrm{pair}}$; the remaining terms are the free [hydrogen ion](hydrogen-ion.md) and [hydroxide](hydroxide.md) contributions, $\beta_{\mathrm{water}}$. Each has units $\mathrm{mol\,L^{-1}}$ per [pH](ph.md). Equivalently, with dimensional $H_c=[\mathrm H^+]$, $K_{a,c}=c^\circ K_a$ and $K_{w,c}=(c^\circ)^2K_w$, the expression is $(\ln10)(C K_{a,c}H_c/(K_{a,c}+H_c)^2+H_c+K_{w,c}/H_c)$. Mixing the dimensional and [dimensionless](dimensionless-quantity.md) conventions would give incorrect units.

For $r=K_a/H=10^{\mathrm{pH}-\mathrm pK_a}$,

$$
\beta_{\mathrm{pair}}=(\ln10)C\frac{r}{(1+r)^2}\leq\frac{\ln10}{4}C,
$$

because $(1+r)^2-4r=(1-r)^2\geq0$. Equality occurs at $r=1$: equal [weak acid](weak-acid.md) and [conjugate base](conjugate-base.md) [concentrations](concentration.md), or [pH](ph.md) equal to [pKa](pka.md). This is the exact maximum of the pair contribution in this model. The full [buffer capacity](buffer-capacity.md) need not have its maximum there: free [hydrogen ions](hydrogen-ion.md) and [hydroxide](hydroxide.md) make it grow toward the acidic and alkaline extremes. When these contributions are small, the central peak lies close to [pKa](pka.md).

## ↑ Ancestors (5)

1. [Buffer capacity](buffer-capacity.md)
2. [Buffer solution](buffer-solution.md)
3. [Acid-base chemistry](acid-base-chemistry-split.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)
