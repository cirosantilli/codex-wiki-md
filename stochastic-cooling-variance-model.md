# Stochastic cooling variance model

↑ **Parent:** [Stochastic cooling](stochastic-cooling.md)

Let $x_n$ be a centered scalar beam-deviation coordinate in a deliberately controlled toy model. Let the readout be $s_n=x_n+\eta_n$, where the centered measurement [noise](noise-signal-processing.md) $\eta_n$ has [variance](variance-split.md) $N$ and is independent of $x_n$ and of earlier [noise](noise-signal-processing.md). Stipulate a correctly timed correction of strength $g$: $x_{n+1}=x_n-gs_n$. This scalar observation is a teaching surrogate, not a claim that real cooling measures each particle. From [variance additivity for independent random variables](variance-additivity-for-independent-random-variables.md),

$$
x_{n+1}=(1-g)x_n-g\eta_n,\qquad
V_{n+1}=(1-g)^2V_n+g^2N,\qquad V_n=\operatorname{Var}(x_n).
$$

For fixed current $V>0$ and $N\geq0$, differentiate the next-step [variance](variance-split.md) with respect to [feedback gain](feedback-gain.md):

$$
\frac{dV_{\rm next}}{dg}=-2V+2g(V+N),\qquad
\frac{d^2V_{\rm next}}{dg^2}=2(V+N)>0.
$$

The unique one-step minimizing [feedback gain](feedback-gain.md) and resulting [variance](variance-split.md) are

$$
g_* =\frac{V}{V+N},\qquad
V_{\rm next,min}=\frac{VN}{V+N}.
$$

The noisier the readout relative to the current spread, the smaller the useful correction. The exact one-step cooling condition follows by subtraction:

$$
V_{\rm next}-V=g\bigl[g(V+N)-2V\bigr]<0
\quad\Longleftrightarrow\quad
0<g<\frac{2V}{V+N}=2g_*.
$$

Thus excessive positive [feedback gain](feedback-gain.md) heats this model. The threshold depends on the current [variance](variance-split.md): a gain that initially cools can later heat if the beam has become narrower or the [noise](noise-signal-processing.md) has grown.

For chosen dimensionless $V_0=1$ and $N=1/4$, $g_*=0.8$ gives $V_1=0.20$. Taking $g=1.8$ instead gives $V_1=1.45$, larger than the initial spread. Holding $g=0.8$ fixed gives

$$
V_n=\frac16+\frac56(0.04)^n,
$$

so the [variance](variance-split.md) approaches the nonzero noise floor $1/6$. More generally, for $0<g<2$ the fixed-gain limit is $V_\infty=gN/(2-g)$. This long-run stability condition differs from the condition for cooling the current beam on the very next step.

If the toy [feedback gain](feedback-gain.md) is recomputed after every step and $N>0$, the reciprocal recurrence is even simpler:

$$
\frac1{V_{n+1}}=\frac1{V_n}+\frac1N,\qquad
V_n=\frac{V_0N}{N+nV_0}.
$$

With the chosen inputs, $V_5=1/21\simeq0.047619$. This ideal model has no additional diffusion, finite observation time or lost correlation; its indefinitely falling spread is not a prediction for an operating storage ring.

To expose the missing physics mathematically, replace $s=x+\eta$ by an arbitrary centered sample signal $s$. Defining $C=\operatorname{Cov}(x,s)$ and $S=\operatorname{Var}(s)>0$ gives

$$
\operatorname{Var}(x-gs)=V-2gC+g^2S,\qquad g_*=C/S.
$$

Unwanted contributions from other [particles](particle-physics.md) or electronics can enlarge $S$ without increasing useful $C$; poor timing or lost correlation can reduce $C$ or even reverse its sign. This is why real [stochastic cooling](stochastic-cooling.md) needs measured beam fluctuations, appropriate [beam mixing](beam-mixing.md) and correctly phased [feedback control](closed-loop-control.md), rather than an imagined catalogue of individual particle positions.

## ↑ Ancestors (6)

1. [Stochastic cooling](stochastic-cooling.md)
2. [Beam cooling](beam-cooling.md)
3. [Particle accelerator](particle-accelerator-split.md)
4. [Experimental apparatus](experimental-apparatus.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Stochastic cooling](stochastic-cooling.md)
