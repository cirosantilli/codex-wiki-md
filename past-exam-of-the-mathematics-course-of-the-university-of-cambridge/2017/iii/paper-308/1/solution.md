<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Take $\lambda>0$, $m>0$, use metric $(+,-)$ and set $\kappa=\sqrt{2\lambda}\,m$. The two [scalar-field vacua](../../../../../scalar-field-vacuum.md) are $\phi=\pm m$; the positive [kink](../../../../../scalar-field-kink.md) joins $-m$ at the left end to $m$ at the right. The [square completion for a one-dimensional kink](../../../../../square-completion-for-a-one-dimensional-kink.md) gives

$$
E=\frac12\int_{\mathbb R}\left[\phi_x-\sqrt{2\lambda}(m^2-\phi^2)\right]^2dx+\sqrt{2\lambda}\left[m^2\phi-\frac{\phi^3}{3}\right]_{-\infty}^{+\infty}.
$$

Thus its [Bogomolny bound](../../../../../bogomolny-bound.md) is $E\geq4\sqrt{2\lambda}m^3/3$. Equality requires $\phi_x=\sqrt{2\lambda}(m^2-\phi^2)$; separating variables, or differentiating the resulting [hyperbolic tangent](../../../../../hyperbolic-tangent.md), gives

$$
\boxed{\phi_K(x)=m\tanh\!\bigl[\kappa(x-X)\bigr],\qquad M=E_K=\frac43\sqrt{2\lambda}\,m^3.}
$$

$X$ is the translational [collective coordinate](../../../../../collective-coordinate-of-a-soliton.md). The [antikink](../../../../../antikink.md) is $-\phi_K$ for the centered odd profile. Differentiating the first-order equation gives the static [Euler-Lagrange field equation](../../../../../euler-lagrange-field-equation.md) $\phi_{xx}=4\lambda\phi(\phi^2-m^2)$. Hence the [Bogomolny equation](../../../../../bogomolny-equations.md) really does solve the second-order theory. The two distinct vacua and the above [kink](../../../../../scalar-field-kink.md) require the positive parameters; the degenerate case $m=0$, or the unstable negative-$\lambda$ potential, does not have this topological [kink](../../../../../scalar-field-kink.md) sector.

For a slowly moving [kink](../../../../../scalar-field-kink.md), put $\phi(x,t)=\phi_K(x-X(t))$. The saturated first-order equation implies $V(\phi_K)=\phi_K'^2/2$, so

$$
\int_{\mathbb R}\phi_K'^2dx=E_K=M.
$$

The [stress-energy tensor](../../../../../stress-energy-tensor.md) has $T^{00}=\phi_t^2/2+\phi_x^2/2+V$ and $T^{01}=-\phi_t\phi_x$. Using $\phi_t=-v\phi_K'$ in the approximate translate therefore gives $E=M+Mv^2/2$ and $P=Mv$. Equivalently, substitution into the action gives the [collective-coordinate effective Lagrangian](../../../../../collective-coordinate-effective-lagrangian-for-a-soliton.md) $L_{\rm eff}=-M+M\dot X^2/2$. These are the [translational dynamics of a phi-four kink](../../../../../translational-dynamics-of-a-phi-four-kink.md), with

$$
\boxed{E=M+\frac12Mv^2+O(v^4),\qquad P=Mv+O(v^3).}
$$

The displayed remainder orders refer to the exact constant-velocity solution. The uncontracted translated profile is only an approximation: its error as a field starts at $O(v^2)$, but the static profile is an [energy](../../../../../energy.md) stationary point, so the corresponding static-energy error starts at $O(v^4)$ and does not change the displayed $v^2$ coefficient.

Since the relativistic action is invariant under [Lorentz transformations](../../../../../lorentz-transformation.md), a [Lorentz boost](../../../../../lorentz-boost.md) gives the exact moving [kink](../../../../../scalar-field-kink.md), for $|v|<1$,

$$
\boxed{\phi(x,t)=m\tanh\!\left[\kappa\gamma_v(x-X-vt)\right],\qquad \gamma_v=(1-v^2)^{-1/2}.}
$$

Its conserved [energy](../../../../../energy.md) and [momentum](../../../../../momentum.md) are $E=\gamma_v M$ and $P=\gamma_v Mv$, whose expansions agree with the preceding calculation. The width contraction is essential to solving the exact time-dependent equation.

Use the centered profile $K(x)=m\tanh(\kappa x)$. An appropriate approximate separated-lump initial condition is

$$
\boxed{\phi(x,0)=K(x+a)-K(x)+K(x-a),\qquad \phi_t(x,0)=0.}
$$

It tends to $-m$ as $x\to-\infty$ and $m$ as $x\to+\infty$. Near $-a$ and $a$ it is a positive [kink](../../../../../scalar-field-kink.md), and near zero it is an [antikink](../../../../../antikink.md); the other two tails cancel to exponentially small accuracy. The condition $\kappa a\gg1$ makes these interpretations accurate. This sum is legitimate smooth initial data, not an exact static multi-kink solution. Its [topological charge](../../../../../topological-charge.md) is

$$
Q=\frac{\phi(+\infty)-\phi(-\infty)}{2m}=1,
$$

and its [energy](../../../../../energy.md) is close to $3M$, with exponentially small interactions.

Adjacent [kink](../../../../../scalar-field-kink.md)–[antikink](../../../../../antikink.md) pairs attract: the [kink–antikink attraction from the stress tensor](../../../../../kink-antikink-attraction-from-the-stress-tensor.md) gives a negative midpoint pressure and hence an inward force on each outside [kink](../../../../../scalar-field-kink.md). Direct overlap of the two outer [kink](../../../../../scalar-field-kink.md) tails is exponentially smaller than each adjacent [kink](../../../../../scalar-field-kink.md)–[antikink](../../../../../antikink.md) overlap. The initial field is odd and its velocity zero, so the equation's reflection-plus-sign symmetry preserves $\phi(-x,t)=-\phi(x,t)$. The central zero remains at $x=0$ and the outer cores move in symmetrically. They collide with the central [antikink](../../../../../antikink.md). Excess [energy](../../../../../energy.md) can excite localized [kink](../../../../../scalar-field-kink.md) oscillations and outgoing radiation; the usual relaxational outcome is a remaining centered [kink](../../../../../scalar-field-kink.md) plus radiation after transient collisions or oscillations. On an infinite line radiation can carry [energy](../../../../../energy.md) away from the core even though total [energy](../../../../../energy.md) is conserved. Conservation of $Q=1$ prevents complete disappearance into vacuum, but it does not determine every bounce or exclude a temporarily re-emerging [kink](../../../../../scalar-field-kink.md)–[antikink](../../../../../antikink.md) pair. The nonintegrable collision should not be described as exact elastic passage of all three solitons.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
