# Weak acid mass and charge balances

↑ **Parent:** [Weak acid](weak-acid.md)

Consider only neutral $\mathrm{HA}$ added to pure [water](water.md), at fixed [temperature](temperature.md), with ideal dilute [thermodynamic activities](thermodynamic-activity.md), [water](water.md) [thermodynamic activity](thermodynamic-activity.md) approximated by one, and no added salts or other [chemical species](chemical-species.md). Normalize every [concentration](concentration.md) by $c^\circ=1\,\mathrm{mol\,L^{-1}}$:

$$
c=C_T/c^\circ,\qquad h=[\mathrm H_3\mathrm O^+]/c^\circ,\qquad x=[\mathrm A^-]/c^\circ,\qquad y=[\mathrm{HA}]/c^\circ,\qquad o=[\mathrm{OH}^-]/c^\circ.
$$

Conservation of acid units and zero net [electric charge](electric-charge.md), respectively, require

$$
x+y=c,\qquad h=x+o.
$$

The second equation balances positive [hydronium](hydronium.md) against negative [conjugate base](conjugate-base.md) and [hydroxide](hydroxide.md). It would need all additional [ions](ion.md) if salts or a [chemical base](base-chemistry.md) were added. Together with [acid dissociation constant](acid-dissociation-constant.md) $K_a=hx/y$ and the [self-ionization of water](self-ionization-of-water.md) relation $K_w=ho$, these give

$$
x=\frac{K_ac}{K_a+h},\qquad y=\frac{hc}{K_a+h},\qquad o=\frac{K_w}{h},\qquad
h-\frac{K_w}{h}-\frac{K_ac}{K_a+h}=0.
$$

This is exact within the stated ideal model, including depletion and [self-ionization of water](self-ionization-of-water.md). Multiplication by $h(K_a+h)$ yields the [cubic equation](cubic-equation.md)

$$
h^3+K_ah^2-(K_w+K_ac)h-K_aK_w=0.
$$

For positive $K_a,K_w,c$, the unmultiplied left-hand side increases strictly from negative to positive values as $h$ increases from zero to infinity; its [derivative](derivative.md) is $1+K_w/h^2+K_ac/(K_a+h)^2>0$. There is therefore exactly one positive [root of a polynomial](root-of-a-polynomial.md). A [bisection method](bisection-method.md) can find it without choosing an unphysical [root of a polynomial](root-of-a-polynomial.md).

If $K_w/h^2\ll1$, neglect [hydroxide](hydroxide.md), so $h\approx x$ and the [quadratic equation](quadratic-equation.md) retaining acid depletion gives

$$
\frac{x^2}{c-x}=K_a,\qquad
x=\frac{\sqrt{K_a^2+4K_ac}-K_a}{2}
=\frac{2K_ac}{\sqrt{K_a^2+4K_ac}+K_a}.
$$

The last form avoids subtracting nearly equal numbers. If also $x/c\ll1$, neglect depletion to obtain

$$
h\approx x\approx\sqrt{K_ac},\qquad
[\mathrm H_3\mathrm O^+]\approx\sqrt{K_a c^\circ C_T}.
$$

Check both conditions after computing: $x/c$ measures the fraction lost from the initial undissociated [weak acid](weak-acid.md) inventory, while $K_w/h^2$ measures the omitted [hydroxide](hydroxide.md) contribution to [electric charge](electric-charge.md) balance. A $5\%$ depletion criterion is a chosen tolerance, not a universal boundary. Keeping depletion does not cure the neglect of [self-ionization of water](self-ionization-of-water.md). These [weak acid mass and charge balances](weak-acid-mass-and-charge-balances.md) also explain why the [square root](square-root.md) estimate cannot be extended to arbitrarily dilute [chemical solutions](solution-chemistry.md).

**Table of contents**

- [Analytical concentration](analytical-concentration.md)

## ↑ Ancestors (5)

1. [Weak acid](weak-acid.md)
2. [Acid (chemistry)](acid-chemistry.md)
3. [Acid-base chemistry](acid-base-chemistry.md)
4. [Chemistry](chemistry-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Acid dissociation constant](acid-dissociation-constant.md)
- [Conjugate base](conjugate-base.md)
- [Weak acid dissociation fraction](weak-acid-dissociation-fraction.md)
- [Weak acid mass and charge balances](weak-acid-mass-and-charge-balances.md)
