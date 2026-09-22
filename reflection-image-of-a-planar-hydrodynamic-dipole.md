# Reflection image of a planar hydrodynamic dipole

↑ **Parent:** [Complex potential of a two-dimensional potential flow](complex-potential-of-a-two-dimensional-potential-flow.md)

For a [complex potential](complex-potential-of-a-two-dimensional-potential-flow.md) $w(z)=m/(z-a)$, reflection in the straight wall through zero at angle $\theta$ is $Rz=e^{2i\theta}\bar z$. The image construction $W(z)=w(z)+\overline{w(Rz)}$ gives

$$
W(z)=\frac{m}{z-a}+\frac{e^{2i\theta}\bar m}{z-e^{2i\theta}\bar a}.
$$

On the wall $Rz=z$, this is real, so its [stream function](stream-function.md) is constant there. This proves the [impermeability condition](no-penetration-boundary-condition.md). Thus the image position is $a'=e^{2i\theta}\bar a$ and its moment is $m'=e^{2i\theta}\bar m$. If the point dipole is advected by the regular image flow, the [complex velocity](complex-velocity.md) convention $W'=u-iv$ gives

$$
\frac{d\bar a}{dt}=-\frac{m'}{(a-a')^2}=\frac{\bar m}{4d^2},
$$

where $d=\operatorname{Im}(e^{-i\theta}a)$ is its signed distance from the wall. The last equality follows from $a-a'=2ie^{i\theta}d$. It applies when $d\ne0$.

## ↑ Ancestors (6)

1. [Complex potential of a two-dimensional potential flow](complex-potential-of-a-two-dimensional-potential-flow.md)
2. [Potential flow](potential-flow.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
