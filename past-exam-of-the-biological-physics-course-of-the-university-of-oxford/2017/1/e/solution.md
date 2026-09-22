<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

With equal [substrate](../../../../substrate-biochemistry.md) abundance and association rates, let $a=k_-^S<b=k_-^R$ and $c=l_-^{S*}<d=l_-^{R*}$. Then

$$
F(m,V_A)=\frac{a+m}{b+m}\frac{c+V_A}{d+V_A}.
$$

Both factors increase with their forward rate: for example $\partial_m[(a+m)/(b+m)]=(b-a)/(b+m)^2>0$. Thus maximum discrimination requires enough waiting at each stage for the less stable incorrect complex to be rejected. In the slow-forward limit,

$$
\boxed{m\ll k_-^S,k_-^R,\quad V_A\ll l_-^{S*},l_-^{R*},\qquad
F\longrightarrow\frac{k_-^S}{k_-^R}\frac{l_-^{S*}}{l_-^{R*}}.}
$$

The two rejection stages multiply their discrimination. Fast modification or fast product formation bypasses the corresponding [dissociation](../../../../dissociation-rate-constant.md) test and drives that factor towards one.

There is a [kinetic proofreading fidelity-throughput tradeoff](../../../../kinetic-proofreading-fidelity-throughput-tradeoff.md): taking either forward rate literally to zero gives zero [product flux](../../../../reaction-rate.md), not a useful finite-output optimum. If [dissociation](../../../../dissociation-rate-constant.md) rates are well separated, a practical high-yield discrimination window is $k_-^S\ll m\ll k_-^R$ and $l_-^{S*}\ll V_A\ll l_-^{R*}$. Correct complexes then usually pass both stages while incorrect complexes usually dissociate; its fidelity is not the mathematical infimum obtained with vanishing forward rates. The irreversible modification represents a driven, energy-consuming step, permitting successive nonequilibrium checks rather than merely repeating one equilibrium binding comparison. No finite positive optimum can be selected from minimization of $F$ alone without a speed or yield requirement.

## ↑ Ancestors (12)

1. [E](../e.md)
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
