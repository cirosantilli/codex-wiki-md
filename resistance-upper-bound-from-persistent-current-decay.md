# Resistance upper bound from persistent-current decay

↑ **Parent:** [Persistent current in a superconducting loop experiment](persistent-current-in-a-superconducting-loop-experiment.md)

Suppose a calibrated measurement bounds the fractional loss of a nonzero [superconducting persistent current](persistent-current-superconductivity.md) by $\epsilon$, with $0<\epsilon<1$, over a duration $T>0$. Take $I_0>0$ by choosing the circulation direction. Under the constant-$L$, constant-$R$, undriven [RL circuit](rl-circuit.md) model,

$$
\frac{I(T)}{I_0}\geq1-\epsilon
\quad\Longrightarrow\quad
0\leq R\leq-\frac{L}{T}\ln(1-\epsilon)
\simeq\frac{L\epsilon}{T}.
$$

The inequality follows because the [logarithm](logarithm.md) is increasing. The final approximation requires $\epsilon\ll1$ and slightly understates the exact upper bound. If $L$ is uncertain, an independently established upper bound on $L$ gives the conservative [electrical resistance](electrical-resistance.md) bound. The uncertainty in the initial reading, the final reading, background subtraction and drift must all be included in $\epsilon$; a display resolution alone does not provide it.

<a id="image-an-illustrative-exponential-decay-its-logarithmic-slope-and-the-resulting-resistance-bound"></a>
![](persistent-superconducting-current-decay-bound.png)

**[Figure 2](#image-an-illustrative-exponential-decay-its-logarithmic-slope-and-the-resulting-resistance-bound). An illustrative exponential decay, its logarithmic slope and the resulting resistance bound**. Chosen numerical model, not historical data: fixed [self-inductance](self-inductance.md) $L=1\,\mathrm{\mu H}$ and no external drive. The final panel assumes a calibrated fractional-loss bound of $0.001$ at each chosen observation duration. Longer observation tightens the bound only while that fractional uncertainty remains controlled.

For an original illustrative example, let $L=1\,\mathrm{\mu H}$ and suppose the corrected [electric current](electric-current.md) ratio after $T=3\,\mathrm h=10800\,\mathrm s$ is at least $0.999$. Then

$$
R\leq9.264\times10^{-14}\,\Omega,\qquad
\tau\geq1.07946\times10^7\,\mathrm s\simeq124.94\,\mathrm{days}.
$$

These are conditional bounds for stipulated parameters, not values attributed to the 1914 apparatus. With the same $L$ but $R=10^{-11}\,\Omega$, the model instead gives $\tau=10^5\,\mathrm s$ and $I(24\,\mathrm h)/I_0=e^{-0.864}\simeq0.42147$: a readily visible loss on the chosen scale.

A resolved decay can be checked using its [logarithm](logarithm.md):

$$
\ln\frac{I(t)}{I_0}=-\frac{R}{L}t,\qquad
R=-L\frac{d\ln|I|}{dt}.
$$

A straight line supports this constant-parameter model; curvature or jumps demand a different account. If an effective [electrical resistance](electrical-resistance.md) varies with time while $L$ remains fixed and the loop remains undriven, only its time average is constrained:

$$
I(T)=I_0\exp\!\left[-\frac{1}{L}\int_0^T R(t)\,dt\right],\qquad
\frac{1}{T}\int_0^T R(t)\,dt\leq-\frac{L}{T}\ln(1-\epsilon).
$$

This does not bound every instantaneous value of $R(t)$. Changing [self-inductance](self-inductance.md) or external linked [magnetic flux](magnetic-flux.md) adds terms to the circuit equation, so an uncorrected magnetic signal cannot simply be substituted for $I(t)$. Nonobservation of decay leaves arbitrarily small positive constant [electrical resistance](electrical-resistance.md) compatible with a finite observation: it is not a logical proof that $R=0$.

## ↑ Ancestors (6)

1. [Persistent current in a superconducting loop experiment](persistent-current-in-a-superconducting-loop-experiment.md)
2. [Superconductivity](superconductivity-split.md)
3. [Statistical physics](statistical-physics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
