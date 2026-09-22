# Constant-input firing rate of a leaky integrate-and-fire neuron

↑ **Parent:** [Leaky integrate-and-fire model](leaky-integrate-and-fire-model.md)

For $C_m\dot V=-g_L(V-V_L)+I$, reset $V_0<V_\theta$ and no explicit refractory interval, define $I_c=g_L(V_\theta-V_L)$ and $\tau_m=C_m/g_L$. Constant current gives

$$
r(I)=\begin{cases}0,&I\leq I_c,\\\bigl[\tau_m\log((I-g_L(V_0-V_L))/(I-I_c))\bigr]^{-1},&I>I_c.\end{cases}
$$

The threshold is approached only asymptotically at $I=I_c$. At large current, $r\sim I/[C_m(V_\theta-V_0)]$. Adding an absolute [neuronal refractory period](neuronal-refractory-period.md) changes the denominator to $T(I)+t_{\rm ref}$ and makes the firing rate saturate rather than grow without bound.

## ↑ Ancestors (5)

1. [Leaky integrate-and-fire model](leaky-integrate-and-fire-model.md)
2. [Computational neuroscience](computational-neuroscience.md)
3. [Neuroscience](neuroscience.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-84/3/d/solution.md)
