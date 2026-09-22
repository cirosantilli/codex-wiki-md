# Wheatstone bridge balance

↑ **Parent:** [Wheatstone bridge](wheatstone-bridge.md)

First disconnect the detector. Each side is a [voltage divider](voltage-divider.md). [Ohm's law](ohm-s-law.md) and [Kirchhoff's voltage law](kirchhoff-cycle-law.md) give the open-circuit intermediate [electric potentials](electric-potential.md) and their difference:

$$
V_B=V_s\frac{R_2}{R_1+R_2},\qquad
V_C=V_s\frac{R_x}{R_3+R_x},\qquad
V_{\mathrm{oc}}=V_B-V_C
=V_s\left(\frac{R_2}{R_1+R_2}-\frac{R_x}{R_3+R_x}\right).
$$

Setting this difference to zero and cross-multiplying gives

$$
R_2R_3=R_1R_x,\qquad
\frac{R_1}{R_2}=\frac{R_3}{R_x},\qquad
R_x=R_3\frac{R_2}{R_1}.
$$

The balance compares ratios, not necessarily equal arm values or equal branch [electric currents](electric-current.md). At balance the detector carries no [electric current](electric-current.md), so [Kirchhoff's current law](kirchhoff-node-law.md) again makes the [electric current](electric-current.md) constant along each two-arm path.[PHYWE, Wheatstone bridge, P2410200, p. 4, Theory (1/3)–(2/3), equations (1)–(4): divider potentials and balance](wheatstone-bridge-by-phywe-p2410200.md)

For a worked [null measurement](null-measurement.md), suppose $R_1=1.000\,\mathrm{k\Omega}$ and $R_2=2.000\,\mathrm{k\Omega}$, and the detector null occurs at adjustable $R_3=1.500\,\mathrm{k\Omega}$. Then

$$
R_x=(1.500\,\mathrm{k\Omega})\frac{2.000\,\mathrm{k\Omega}}{1.000\,\mathrm{k\Omega}}
=3.000\,\mathrm{k\Omega}.
$$

For $V_s=3.000\,\mathrm V$, both intermediate [electric potentials](electric-potential.md) are $2.000\,\mathrm V$. The left branch carries $1.000\,\mathrm{mA}$ and the right branch $0.6667\,\mathrm{mA}$: the zero detector reading does not mean that the unknown carries no [electric current](electric-current.md). These are stipulated ideal values illustrating the calculation, not experimental observations.

## ↑ Ancestors (5)

1. [Wheatstone bridge](wheatstone-bridge.md)
2. [Resistance bridge](resistance-bridge.md)
3. [Electrical measurement](electrical-measurement.md)
4. [Electrical engineering](electrical-engineering-split.md)
5. [Codex Wiki](split.md)
