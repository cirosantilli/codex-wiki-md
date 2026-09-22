<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Here $p_n(t)$ is the [probability](../../../../probability.md) of occupying state $n$, and $W_{nm}$ for $n\ne m$ is the transition rate from $m$ to $n$. More precisely, over $dt>0$ that transition has [probability](../../../../probability.md) $W_{nm}dt+o(dt)$. This is a time-homogeneous [continuous-time Markov chain](../../../../continuous-time-markov-chain-split.md): the present state contains all information needed for the next transition, the rates do not depend on time, and finite rates make multiple jumps have [probability](../../../../probability.md) $o(dt)$. In a physical rate description, untracked coherent dynamics or memory must be negligible on the timescale being modeled.

The [master equation](../../../../master-equation.md) separates incoming and outgoing terms:

$$
\dot p_n=\sum_{m\ne n}(W_{nm}p_m-W_{mn}p_n),\qquad\boxed{W_{nm}\ge0\ (n\ne m),\quad W_{mm}=-\sum_{n\ne m}W_{nm}.}
$$

Columns, rather than rows, sum to zero with this indexing. These conditions preserve normalization and nonnegative [probabilities](../../../../probability.md). For infinitely many states one also needs a well-defined nonexplosive process. [Detailed balance](../../../../detailed-balance.md) is an additional equilibrium condition, not a general requirement on a [master equation](../../../../master-equation.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
