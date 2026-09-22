<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat $p_n(t)$ as the [probability](../../../../probability.md) of the complete coarse-grained state $n$ at time $t$, with $p_n\geq0$ and $\sum_np_n=1$. In the column-vector convention of the [master equation](../../../../master-equation.md), $W_{nm}$ for $n\ne m$ is the transition rate **from $m$ to $n$**. The short-time transition law is

$$
P(n,t+dt\mid m,t)=\delta_{nm}+W_{nm}dt+o(dt).
$$

Nonnegative transition [probabilities](../../../../probability.md) and conservation of total [probability](../../../../probability.md) require

$$
\boxed{W_{nm}\geq0\ (n\ne m),\qquad
\sum_nW_{nm}=0,\qquad W_{mm}=-\sum_{n\ne m}W_{nm}\leq0.}
$$

For a [finite state space](../../../../finite-state-space.md) these conditions define a [continuous-time Markov chain](../../../../continuous-time-markov-chain-split.md). The [Markov property](../../../../markov-property.md) means that, conditional on the present state, no further history affects the transition [probabilities](../../../../probability.md). A time-independent $W$ additionally assumes time-homogeneous rates; the waiting time in a state is exponential, and multiple jumps in an infinitesimal interval contribute beyond first order. A reduced description that omits relevant slow variables can retain memory and need not obey this closed equation. [Quantum coherences](../../../../quantum-coherence-in-a-specified-basis.md) are likewise absent from this classical population model. For infinite state spaces one also needs conditions preventing infinitely many jumps in finite time. Neither equal forward/backward rates nor [detailed balance](../../../../detailed-balance.md) is required merely to conserve [probability](../../../../probability.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
