# A solvable infrared renormalization flow

↑ **Parent:** [Renormalization group](renormalization-group.md)

Take the following bounded analytic example for a dimensionless positive coupling $g$, with fixed $\epsilon>0$ and $g(0)=g_0>0$:

$$
\frac{dg}{d\ell}=\epsilon g-g^2,\qquad
\ell=\log b=\log(L/a).
$$

Increasing $\ell$ means increasing observation length $L$, hence motion toward the [infrared fixed point](infrared-fixed-point.md). This convention matters: if the inverse-length scale is $\mu=\mu_0e^{-\ell}$, the same trajectory has [renormalization-group beta function](beta-function-physics.md) $\beta_\mu(g)=\mu\,dg/d\mu=-\epsilon g+g^2$. The two derivatives have opposite signs.

To solve the equation, set $v=1/g$. It obeys $dv/d\ell=-\epsilon v+1$, a linear [ordinary differential equation](ordinary-differential-equation.md). Therefore

$$
g(\ell)=\frac{\epsilon}{1+(\epsilon/g_0-1)e^{-\epsilon\ell}}.
$$

For $\ell\geq0$ its denominator is positive, and $g$ stays between $g_0$ and $\epsilon$. Thus the trajectory is bounded on this domain. The [renormalization-group fixed points](renormalization-group-fixed-point.md) are $g=0$ and $g_*=\epsilon$. The derivative of the length-flow right-hand side is $\epsilon-2g$: zero is repulsive from positive $g$, whereas $g_*$ has [eigenvalue](eigenvalue.md) $-\epsilon$ and attracts positive trajectories. Linearization gives $g-g_*\propto e^{-\epsilon\ell}=b^{-\epsilon}$ near $g_*$. The inverse-length [beta function](beta-function.md) has positive derivative at the same infrared-attractive point.

For the chosen $\epsilon=1/5$, take two starting models with $g_0=1/20$ and $g_0=3/5$. At $b=1024$, $e^{-\epsilon\ell}=1/4$, so their couplings are respectively $4/35$ and $6/25$. Both move toward $1/5$, from opposite sides. They are still visibly different: slow decay of an [irrelevant operator](irrelevant-operator.md) can leave substantial corrections at accessible lengths. The case $g_0=0$ stays exactly zero and is outside this positive-coupling basin.

## ↑ Ancestors (6)

1. [Renormalization group](renormalization-group.md)
2. [Critical phenomenon](critical-phenomenon-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
