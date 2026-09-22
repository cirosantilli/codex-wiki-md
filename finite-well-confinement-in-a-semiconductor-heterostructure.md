# Finite-well confinement in a semiconductor heterostructure

↑ **Parent:** [Quantum well](quantum-well.md)

Consider an original one-dimensional [effective mass](band-effective-mass.md) model with $V(x)=0$ for $|x|<a$ and $V(x)=V_0>0$ outside. Take the same positive [effective mass](band-effective-mass.md) $m^*$ everywhere, an abrupt interface, and no interactions. The [wavefunction](wave-function-split.md) represents a transverse envelope; free motion parallel to the layer is outside this calculation. A [double heterostructure laser](double-heterostructure-laser.md) need not be thin enough for this quantization to dominate its operation.

Set $s=x/a$, $\epsilon=\hbar^2/(2m^*a^2)$, $z_0^2=V_0/\epsilon$, $z^2=E/\epsilon$ and $w=\sqrt{z_0^2-z^2}$. The time-independent [Schrödinger equation](schrodinger-equation.md) becomes

$$
-\frac{d^2\phi}{ds^2}+u(s)\phi=z^2\phi,\qquad
u(s)=\begin{cases}0&|s|<1,\\z_0^2&|s|>1.\end{cases}
$$

Here $u(s)$ denotes the dimensionless potential; a [bound state](bound-state.md) has $0<z<z_0$. Matching the [wavefunction](wave-function-split.md) and its [derivative](derivative.md) at $s=1$ gives

$$
z\tan z=w\quad\text{(even)},\qquad
-z\cot z=w\quad\text{(odd)}.
$$

For the even [bound state](bound-state.md), the interior solution is $A\cos(zs)$ and the exterior solution is $A\cos z\,e^{-w(|s|-1)}$. For the odd [bound state](bound-state.md), replace $\cos(zs)$ by $\sin(zs)$ and $\cos z$ by $\operatorname{sgn}(s)\sin z$. The physical [wavefunction](wave-function-split.md) is $\psi(x)=\phi(x/a)/\sqrt a$.

[Wavefunction normalization](wavefunction-normalization.md) includes both exterior tails, not just the active layer. Direct integration gives

$$
A_{\rm even}^{-2}=1+\frac{\sin(2z)}{2z}+\frac{\cos^2 z}{w},\qquad
A_{\rm odd}^{-2}=1-\frac{\sin(2z)}{2z}+\frac{\sin^2 z}{w}.
$$

The first two terms are the interior integral; the last is the total exterior integral. Thus the interior [probability](probability.md) is $P_{\rm in}=A^2[1\pm\sin(2z)/(2z)]$, with the upper sign for even [parity](parity.md).

Choose $z_0=2$. There is one even root in $(0,\pi/2)$ and one odd root in $(\pi/2,2)$; higher branches start beyond $z_0$. Each left-hand side increases on its stated interval while $\sqrt{4-z^2}$ decreases, proving uniqueness there. Numerically,

$$
\begin{array}{c|ccc}
\text{parity}&z&E/V_0&P_{\rm in}\\\hline
\text{even}&1.029867&0.265156&0.902317\\
\text{odd}&1.895494&0.898225&0.451648
\end{array}
$$

These are calculated values of the chosen [finite square well](finite-square-well.md). The excited [bound state](bound-state.md) lies closer to the barrier and has a longer exterior tail: being bound does not mean having unit [probability](probability.md) inside the well.

<a id="image-two-normalized-bound-states-in-a-chosen-semiconductor-quantum-well"></a>
![](semiconductor-quantum-well-bound-state-confinement.png)

**[Figure 6](#image-two-normalized-bound-states-in-a-chosen-semiconductor-quantum-well). Two normalized bound states in a chosen semiconductor quantum well**. [Source](semiconductor-quantum-well-bound-state-confinement.py). Original dimensionless calculation at $z_0=2$. Left: [energy levels](energy-level.md) and signed normalized envelope [wavefunctions](wave-function-split.md), vertically offset for display. Right: [probability densities](probability-density.md) and integrated interior [probabilities](probability.md). Shading marks $|x|<a$; exterior tails remain part of the [wavefunction normalization](wavefunction-normalization.md).

This model demonstrates electronic confinement, not optical [refractive index](refractive-index.md) confinement or a complete [laser](laser-split.md). Unequal [effective masses](band-effective-mass.md), [band bending](band-bending.md), interface disorder and interactions require a more detailed model. In particular, continuity of the ordinary [derivative](derivative.md) above uses the chosen constant [effective mass](band-effective-mass.md) assumption.

## ↑ Ancestors (5)

1. [Quantum well](quantum-well.md)
2. [Semiconductor heterostructure](semiconductor-heterostructure.md)
3. [Semiconductor](semiconductor-split.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)
