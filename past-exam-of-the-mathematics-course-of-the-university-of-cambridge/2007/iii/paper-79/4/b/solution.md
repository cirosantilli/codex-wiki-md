<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $V=U-c$ and suppose a growing [normal mode](../../../../../../normal-mode.md) has $\operatorname{Im}c=c_i>0$, taking $\alpha>0$ without loss of generality. Since $V$ never vanishes on the real channel, choose a continuous square-root branch and write $\phi=V^{1/2}H$. Direct differentiation gives

$$
\phi'=V^{1/2}H'+\frac{U'}{2V^{1/2}}H,
$$



$$
\phi''=V^{1/2}H''+\frac{U'}{V^{1/2}}H'+\left(\frac{U''}{2V^{1/2}}-\frac{U'^2}{4V^{3/2}}\right)H.
$$

Substitution into the [Taylor–Goldstein equation](../../../../../../taylor-goldstein-equation.md) and division by $V^{1/2}$ gives

$$
VH''+U'H'-\alpha^2VH-\frac12U''H+\frac{J-U'^2/4}{V}H=0.
$$

Thus the required transformation is

$$
\boxed{D(V DH)-\left(\alpha^2V+\frac12U''+\frac{U'^2/4-J}{V}\right)H=0.}
$$

The impermeable walls give $\phi(\pm1)=0$, hence $H(\pm1)=0$. Multiply by $\overline H$, integrate across the channel, and use [integration by parts](../../../../../../integration-by-parts.md). With the boundary term zero, the resulting [power-transformed Taylor–Goldstein energy identity](../../../../../../power-transformed-taylor-goldstein-energy-identity.md) is

$$
\int_{-1}^1\left[V\left(|H'|^2+\alpha^2|H|^2\right)+\frac12U''|H|^2+\frac{U'^2/4-J}{V}|H|^2\right]dy=0.
$$

Both $U''$ and $J$ are real. Since $\operatorname{Im}V=-c_i$ and $\operatorname{Im}(1/V)=c_i/|V|^2$, its [imaginary part](../../../../../../imaginary-part.md), divided by $-c_i$, is

$$
\int_{-1}^1\left[|H'|^2+\alpha^2|H|^2+\frac{J-U'^2/4}{|U-c|^2}|H|^2\right]dy=0.
$$

If $J\ge U'^2/4$ everywhere, the integrand is nonnegative and the first two terms have positive integral for any nonzero mode. This contradicts the identity. Therefore instability requires

$$
\boxed{J(y)<\frac14U'(y)^2\quad\text{somewhere in the channel}.}
$$

This is the necessary instability condition of the [Miles–Howard theorem](../../../../../../miles-howard-theorem.md). Where $U'\ne0$, it says that the [gradient Richardson number](../../../../../../gradient-richardson-number.md) $J/U'^2$ must be below $1/4$ somewhere. It is not a sufficient condition for instability, and the conclusion concerns exponential normal-mode growth, not exclusion of the algebraic [lift-up effect](../../../../../../lift-up-effect.md) in part (a). The algebra uses the given nondimensional $J$; in dimensional notation its counterpart is the squared [buoyancy frequency](../../../../../../buoyancy-frequency.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
