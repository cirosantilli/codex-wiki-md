<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For positive rates the three states communicate, so the finite [continuous-time Markov chain](../../../../continuous-time-markov-chain-split.md) has a unique stationary [probability](../../../../probability.md) vector. The first and third components of $Wp^{\rm st}=0$ give

$$
f_1p_0^{\rm st}=f_4p_A^{\rm st},\qquad
f_2p_A^{\rm st}=f_3p_B^{\rm st}.
$$

These two edge-balance relations and [normalization](../../../../normalization.md) yield, with $D=f_3f_4+f_1f_3+f_1f_2$,

$$
\boxed{p_0^{\rm st}=\frac{f_3f_4}{D},\qquad
p_A^{\rm st}=\frac{f_1f_3}{D},\qquad
p_B^{\rm st}=\frac{f_1f_2}{D}.}
$$

Their sum is one and each is nonnegative. The middle balance equation then follows from the other two, as expected from [probability](../../../../probability.md) conservation. A line graph has no cycle that could carry a nonzero stationary circulation: each edge's forward and backward stationary traffic balances even if the bare rates differ. If some rates vanish, the process need not be an [irreducible Markov chain](../../../../irreducible-markov-chain.md) and its stationary distribution need not be unique. The displayed expression remains valid when its denominator is nonzero and its limits select the communicating class reached, but it must not be used as a unique late-time law when disconnected closed classes retain dependence on the initial state.

## ↑ Ancestors (12)

1. [C](../c.md)
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
