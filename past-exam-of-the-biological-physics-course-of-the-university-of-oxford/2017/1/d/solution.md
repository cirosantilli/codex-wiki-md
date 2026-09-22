<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use steady or initial-rate conditions with effectively clamped [substrate](../../../../substrate-biochemistry.md) [concentrations](../../../../concentration.md). For either [substrate](../../../../substrate-biochemistry.md) $X\in\{S,R\}$, put $U_X=[AX]$ and $V_X=[AX^*]$. The intermediate balances are

$$
0=k_+^X[A][X]-(k_-^X+m)U_X,\qquad
0=mU_X-(l_-^{X*}+V_A)V_X.
$$

The [product flux](../../../../reaction-rate.md) is therefore

$$
J_X=V_AV_X=
\frac{k_+^X[A][X]\,mV_A}{(k_-^X+m)(l_-^{X*}+V_A)}.
$$

The [free enzyme](../../../../enzyme-split.md) [concentration](../../../../concentration.md) is common to the two competing pathways, so it cancels even when [enzyme](../../../../enzyme-split.md) sequestration changes its magnitude. Consequently

$$
\boxed{F=\frac{J_R}{J_S}=
\frac{[R]}{[S]}\frac{k_+^R}{k_+^S}
\frac{k_-^S+m}{k_-^R+m}
\frac{l_-^{S*}+V_A}{l_-^{R*}+V_A}.}
$$

Each post-binding factor is the ratio of [probabilities](../../../../probability.md) of proceeding rather than dissociating at that stage. The expression assumes positive common forward rates and no significant product back reaction. Without the steady/intermediate-balance or initial-rate assumption, the ratio can depend on intermediate populations and observation time; binding and [dissociation](../../../../dissociation-rate-constant.md) constants alone would not determine a unique transient ratio.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
