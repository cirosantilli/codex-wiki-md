# Pomeranchuk entropy-balance model

↑ **Parent:** [Pomeranchuk cooling](pomeranchuk-cooling.md)

An original deliberately local model makes the cooling quantitative. Fix a total amount $n$ of material, let $x$ be the mole fraction of [solid](solid.md), and stipulate molar [entropies](entropy-split.md)

$$
S_l(T)=aT,\qquad S_s(T)=b,\qquad a,b>0,
\qquad \frac{S_{\rm total}}n=(1-x)aT+xb.
$$

The constants $a$ and $b$ have units of molar [entropy](entropy-split.md) per [temperature](temperature-split.md) and molar [entropy](entropy-split.md), respectively. Ignore their [pressure](pressure-split.md) dependence and the cell's own [heat capacity](heat-capacity.md). This is a local [thermodynamics](thermodynamics-split.md) model, not an extrapolation to zero [temperature](temperature-split.md). A constant positive $b$ cannot remain valid once the [solid](solid.md)'s [spins](spin.md) order.

For a [reversible thermodynamic process](reversible-thermodynamic-process.md) with no [heat](heat-split.md) exchange, total [entropy](entropy-split.md) is constant. Differentiating gives

$$
(1-x)a\,dT+(b-aT)\,dx=0,
\qquad \frac{dT}{dx}=-\frac{b-aT}{a(1-x)}<0
$$

when $b>aT$ and $x<1$. Define $T_0=b/a$; solving between two states gives

$$
T(x)=\frac{b}{a}-\frac{(1-x_0)(b-aT_i)}{a(1-x)}.
$$

In particular, stipulate $x_0=0$, $T_i=T_0/4$ and $x=1/8$. Then

$$
\frac{T}{T_0}=\frac17,\qquad
\frac{S_{\rm total}}{nb}=\frac14,\qquad
\frac{Q_{l\to s}}{bT_0}=\frac{T}{T_0}\left(1-\frac{T}{T_0}\right)=\frac6{49}.
$$

The last expression is the local reversible [heat](heat-split.md) requirement per mole frozen at the final state, divided by $bT_0$; it is not the [heat](heat-split.md) exchanged during the isolated compression. That compression exchanges no [heat](heat-split.md). This distinction separates the latent-[heat](heat-split.md) sign from the actual boundary [heat](heat-split.md) budget.

<a id="image-why-freezing-can-cool-an-idealized-pomeranchuk-cooling-entropy-balance"></a>
![](helium-three-pomeranchuk-entropy-balance.png)

**[Figure 8](#image-why-freezing-can-cool-an-idealized-pomeranchuk-cooling-entropy-balance). Why freezing can cool: an idealized Pomeranchuk cooling entropy balance**. Original model in arbitrary units, not data. Left: stipulated $S_l=aT$ and $S_s=b$. Right: the isolated reversible path from $x=0$, $T/T_0=1/4$ to $x=1/8$, $T/T_0=1/7$, with fixed $S_{\rm total}/(nb)=1/4$. Only the illustrated local regime is modeled.

The utility of the model is its explicit condition: $S_s>S_l$ makes $dT/dx<0$, while positive total [heat capacity](heat-capacity.md) supplies a stable thermal response. More generally, for molar [entropies](entropy-split.md) depending only on [temperature](temperature-split.md), let $C_l,C_s$ be the molar [heat capacities](heat-capacity.md). Then $dT/dx=-T(S_s-S_l)/[(1-x)C_l+xC_s]$. Incoming [heat](heat-split.md) or [entropy production](entropy-production.md) adds terms to the balance and can overwhelm the ideal cooling. Neither the numerical ratios above nor the straight [entropy](entropy-split.md) lines are measurements of [helium-3](helium-3.md).

## ↑ Ancestors (7)

1. [Pomeranchuk cooling](pomeranchuk-cooling.md)
2. [Helium-3 superfluidity](helium-3-superfluidity.md)
3. [Superfluidity](superfluidity.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
