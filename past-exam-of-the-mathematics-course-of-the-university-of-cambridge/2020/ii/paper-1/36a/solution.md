<h1 id="36a/solution">Solution</h1>

↑ **Parent:** [36A](../36a.md)

Let two systems exchange energy inside an otherwise isolated composite system, so $E_1+E_2=E$ is fixed. By the [Second law of thermodynamics](../../../../../second-law-of-thermodynamics.md), equilibrium maximizes the total [entropy](../../../../../entropy.md)

$$
S_{\rm tot}(E_1)=S_1(E_1)+S_2(E-E_1).
$$

At an interior maximum,

$$
0=\frac{dS_{\rm tot}}{dE_1}
=\frac{\partial S_1}{\partial E_1}
-\frac{\partial S_2}{\partial E_2}
=\frac1{T_1}-\frac1{T_2}.
$$

Thus $T_1=T_2$, which is [entropy maximization under thermal contact](../../../../../entropy-maximization-under-thermal-contact.md) and the condition for [thermal equilibrium](../../../../../thermal-equilibrium.md).

Stability requires this entropy maximum to be locally strict, so each ordinary subsystem has a concave entropy-energy relation. Since

$$
\frac{\partial^2S}{\partial E^2}
=\frac\partial{\partial E}\left(\frac1T\right)
=-\frac1{T^2}\frac{\partial T}{\partial E}<0,
$$

one has $\partial T/\partial E>0$, or equivalently

$$
\boxed{\frac{\partial E}{\partial T}>0.}
$$

This is the [entropy concavity and positive heat capacity](../../../../../entropy-concavity-and-positive-heat-capacity.md) criterion.

Now let $N_\uparrow=\alpha N$ and $N_\downarrow=(1-\alpha)N$. Because the spins are distinguishable, the number of microstates is the [binomial coefficient](../../../../../binomial-coefficient.md)

$$
\Omega=\binom{N}{\alpha N}
=\frac{N!}{(\alpha N)!((1-\alpha)N)!}.
$$

The [Boltzmann entropy](../../../../../boltzmann-s-entropy-formula.md) $S=k_B\log\Omega$ and the [Stirling formula](../../../../../stirling-formula.md) give, to leading order for large $N$,

$$
\boxed{
S(\alpha)=-Nk_B\left[\alpha\log\alpha
+(1-\alpha)\log(1-\alpha)\right].
}
$$

The total energy is

$$
\boxed{E(\alpha)=N\bigl(\alpha\epsilon-(1-\alpha)\epsilon\bigr)
=N\epsilon(2\alpha-1).}
$$

Therefore

$$
\frac1T=\frac{dS/d\alpha}{dE/d\alpha}
=\frac{k_B}{2\epsilon}\log\left(\frac{1-\alpha}{\alpha}\right).
$$

Solving for the up-spin fraction gives the [independent spin-one-half two-level system](../../../../../independent-spin-one-half-two-level-system.md) result

$$
\boxed{
\alpha(T)=\frac1{1+e^{2\epsilon/(k_BT)}}.
}
$$

For ordinary positive absolute temperature,

$$
\boxed{0\leq\alpha<\frac12,}
$$

with $\alpha\to0$ as $T\to0^+$ and $\alpha\to1/2$ as $T\to+\infty$. Since the spectrum is bounded above, the population-inverted range $1/2<\alpha\leq1$ is also mathematically possible and corresponds to [negative temperature](../../../../../negative-temperature.md); $\alpha=1/2$ is the infinite-temperature state.

Substitution gives

$$
E(T)=-N\epsilon\tanh\left(\frac\epsilon{k_BT}\right),
$$

and direct differentiation yields

$$
\boxed{
\frac{dE}{dT}
=\frac{N\epsilon^2}{k_BT^2}
\operatorname{sech}^2\left(\frac\epsilon{k_BT}\right)>0.
}
$$

**Thus the energy increases with temperature throughout either finite-temperature branch, in particular throughout the required positive-temperature range.**

## ↑ Ancestors (10)

1. [36A](../36a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
