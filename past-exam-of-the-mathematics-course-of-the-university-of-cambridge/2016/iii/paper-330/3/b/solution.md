<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For identical suspended particles, [reduced gravity](../../../../../../reduced-gravity-split.md) is proportional to [particle volume fraction](../../../../../../particle-volume-fraction.md). If particles settle through the bed at speed $v_s$ and are not resuspended, the downward [particle deposition flux](../../../../../../particle-deposition-flux.md) removes a buoyancy-equivalent amount $v_sg'$ per unit bed area. The depth-integrated scalar [mass conservation](../../../../../../mass-conservation.md) equation is

$$
\boxed{\partial_t(g'h)+\partial_xB=-v_sg',\qquad B=ug'h.}
$$

For a steady [particle-laden gravity current](../../../../../../particle-laden-gravity-current.md), $B_x=-v_sB/(uh)$. If $v_s/u\ll1$, with fixed positive $E$ and drag/slope coefficients, the locally adjusted leading solution of the momentum and volume equations is $u\sim\beta_*B^{1/3}$ and $h\sim h_0+E(x-x_0)$. The [weak-settling attenuation of a sloping gravity current](../../../../../../weak-settling-attenuation-of-a-sloping-gravity-current.md) then gives

$$
\frac d{dx}B^{1/3}\sim-\frac{v_s}{3\beta_*[h_0+E(x-x_0)]},
$$

and hence

$$
\boxed{B(x)\sim\left[B_o^{1/3}-\frac{v_s}{3\beta_*E}\ln\left(1+\frac{E(x-x_0)}{h_0}\right)\right]^3.}
$$

For an inlet at $x_0=0$ this has the requested logarithmic form. If the inlet is genuinely at $x_0\ne0$, the argument must contain $x-x_0$ in order to satisfy the specified inlet condition.

The speed factor must be the $\beta_*$ derived in the previous part. The printed $\beta$ omits the factor one-half multiplying $E\cos\theta$ and uses an undefined uppercase $C$ instead of the governing equation's $c$. Taking $C=c$ still leaves a nonzero leading momentum residual $-\tfrac12E(B/u)\cos\theta$ for the printed speed; this discrepancy cannot be repaired by a correction of order $v_s/u$. **With the given hydrostatic momentum equation, the logarithmic law is valid with $\beta_*$, not the printed speed factor.**

A controlled local approximation also needs $v_s/(Eu)\ll1$ if $E$ is allowed to become small. Indeed the exact volume balance is $h_x=E-hu_x/u$; under $u\sim\beta_*B^{1/3}$ its second term is $v_s/(3u)$. The neglected depth and acceleration corrections become significant as $B$ approaches zero.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 330](../../../paper-330-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
