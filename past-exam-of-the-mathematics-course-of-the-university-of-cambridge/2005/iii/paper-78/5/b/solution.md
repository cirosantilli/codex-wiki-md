<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $\dot\gamma=(2D:D)^{1/2}>0$, differentiation in the symmetric [tensor](../../../../../../tensor.md) space gives $\partial\dot\gamma/\partial D_{ij}=2D_{ij}/\dot\gamma$. Therefore the [Bingham fluid](../../../../../../bingham-plastic.md) [viscous dissipation potential](../../../../../../viscous-dissipation-potential.md) gives

$$
\boxed{\sigma'_{ij}
=2\left(\frac{\tau_0}{\dot\gamma}+\mu_0\right)D_{ij}.}
$$

The [deviatoric stress](../../../../../../deviatoric-stress.md) is trace free since $D$ is trace free; an arbitrary [pressure](../../../../../../pressure.md) reaction completes the [Cauchy stress tensor](../../../../../../cauchy-stress-tensor.md).

At $D=0$ the yield term is not differentiable, and the correct relation is the [subdifferential](../../../../../../subdifferential.md) condition. A symmetric trace-free [stress](../../../../../../stress.md) $S$ is admissible there if

$$
S:E\leq\tau_0(2E:E)^{1/2}\qquad
\text{for every symmetric trace-free }E.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) shows that this is equivalent to $\|S\|_F\leq\sqrt2\tau_0$; necessity follows by choosing $E$ proportional to $S$. Hence the no-strain-rate restriction is

$$
\boxed{\left(\frac12\sigma'_{ij}\sigma'_{ij}\right)^{1/2}\leq\tau_0.}
$$

The quadratic term has zero derivative at zero and does not change this restriction. This is the unyielded part of the [Bingham plastic](../../../../../../bingham-plastic.md) law.

For flow along the plates, write $y=x_2$, $v=(u(y),0,0)$ and take $G=-p_{,1}>0$ as the pressure-drop magnitude. The only nonzero [rate-of-strain tensor](../../../../../../strain-rate-tensor.md) entries are $D_{12}=D_{21}=u'/2$, so $\dot\gamma=|u'|$ and the yielded [shear stress](../../../../../../shear-stress.md) law is

$$
\sigma_{12}=\tau_0\operatorname{sign}u'+\mu_0u'.
$$

[Force balance](../../../../../../force-balance.md) gives $G+\sigma_{12,y}=0$. The prescribed odd, continuous shear [stress](../../../../../../stress.md) fixes its integration constant to zero, proving

$$
\boxed{\sigma_{12}(y)=-Gy.}
$$

For $\mu_0>0$ the inverse shear law is

$$
u'(y)=
\begin{cases}
0,&|Gy|\leq\tau_0,\\
(-Gy+\tau_0\operatorname{sign}y)/\mu_0,&|Gy|>\tau_0.
\end{cases}
$$

The original PDF also calls $u$ odd. That assumption is inconsistent with a nonzero flow between identical fixed plates: the inverse shear law makes $u'$ odd, whereas the derivative of an odd $u$ is even. Both can hold only if $u'=0$, and the no-slip wall values then give $u=0$. Thus **with the literal odd-velocity requirement, there is no admissible flowing solution when $Gh>\tau_0$**. The standard pressure-driven [velocity](../../../../../../velocity.md) is even; replacing that erroneous parity yields the intended profile below.

If $Gh\leq\tau_0$, the whole gap is unyielded and the fixed no-slip walls force $u=0$. Otherwise let $y_0=\tau_0/G<h$. The [plug flow of a yield-stress fluid](../../../../../../plug-flow-of-a-yield-stress-fluid.md) occupies $|y|\leq y_0$. In the upper yielded layer $u'=(-Gy+\tau_0)/\mu_0$, and integration from $u(h)=0$ gives

$$
u(y)=\frac G{2\mu_0}\left[(h-y_0)^2-(y-y_0)^2\right]
\qquad(y_0\leq y\leq h).
$$

In the plug the [velocity](../../../../../../velocity.md) is the constant $G(h-y_0)^2/(2\mu_0)$, and reflection gives the lower layer. The complete [plane Poiseuille flow of a Bingham fluid](../../../../../../plane-poiseuille-flow-of-a-bingham-fluid.md) answer is

$$
\boxed{\text{Nonzero flow requires }G>\tau_0/h,\qquad
u(y)=\frac G{2\mu_0}\left[(h-y_0)^2-(|y|-y_0)_+^2\right].}
$$

The profile is continuous with continuous first derivative at the plug boundaries, vanishes at both walls and tends to the ordinary parabolic profile when $\tau_0=0$. If signed [pressure](../../../../../../pressure.md) gradients of either direction are allowed, the threshold is $|G|h>\tau_0$, and reversing the gradient reverses the [velocity](../../../../../../velocity.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
