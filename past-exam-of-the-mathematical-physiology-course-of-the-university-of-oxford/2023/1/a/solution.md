<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $a=[\mathrm A]$, $b=[\mathrm B]$ and $c=[\mathrm C]$ for the three [concentrations](../../../../concentration.md). The letters denote [chemical species](../../../../chemical-species.md); the forward arrow represents association of one [molecule](../../../../molecule-split.md) of each reactant into one complex, and the reverse arrow represents dissociation. The positive constants $k_+$ and $k_-$ are the respective [reaction rate constants](../../../../rate-constant.md). For an elementary [chemical reaction](../../../../chemical-reaction-split.md), the [law of mass action](../../../../law-of-mass-action.md) gives forward and reverse [reaction rates](../../../../reaction-rate.md)

$$
R_+=k_+ab,\qquad R_-=k_-c.
$$

Every forward event removes one [molecule](../../../../molecule-split.md) of each reactant and adds one complex; a reverse event reverses those changes. Thus the [reaction-rate equations](../../../../rate-equation.md) are

$$
\boxed{\dot a=-k_+ab+k_-c,\qquad
\dot b=-k_+ab+k_-c,\qquad
\dot c=k_+ab-k_-c.}
$$

The units of $k_+$ are inverse [concentration](../../../../concentration.md) per unit time, whereas $k_-$ has units of inverse time. Adding the equations gives the independent [conservation laws](../../../../conservation-law.md)

$$
\boxed{a+c=a(0)+c(0),\qquad b+c=b(0)+c(0).}
$$

In particular $a-b$ is constant, but this is a consequence of those two [conservation laws](../../../../conservation-law.md). The total $a+b+c$ need not be constant: association changes the number of separate [molecules](../../../../molecule-split.md).

For the general [stoichiometry](../../../../stoichiometry.md), take $p,q$ to be positive [integers](../../../../integer-split.md). The net [reaction rate](../../../../reaction-rate.md) and [stoichiometric vector](../../../../stoichiometric-vector.md) are

$$
R=k_+a^pb^q-k_-c,\qquad \boldsymbol\nu=(-p,-q,1)^{\mathsf T}.
$$

Consequently

$$
\boxed{\dot a=-pR,\qquad \dot b=-qR,\qquad \dot c=R.}
$$

The factors $p,q$ outside $R$ count [molecules](../../../../molecule-split.md) consumed per event; the powers inside $R$ express the [law of mass action](../../../../law-of-mass-action.md). The corresponding [conservation laws](../../../../conservation-law.md) are $a+pc=\text{constant}$ and $b+qc=\text{constant}$. No [factorial](../../../../factorial.md) is required in this deterministic convention for the [reaction rate constant](../../../../rate-constant.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical physiology course of the University of Oxford](../../../split.md)
5. [Mathematical physiology course of the University of Oxford](../../../../mathematical-physiology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
