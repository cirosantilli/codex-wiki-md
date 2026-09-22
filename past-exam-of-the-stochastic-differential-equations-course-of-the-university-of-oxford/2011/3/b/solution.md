<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define $\mathbb Q$ on $\mathcal F_t$ by density $Z_t$. Nonnegativity and [countable additivity](../../../../countable-additivity.md) of the integral make it a measure, and $\mathbb Q(\Omega)=\mathbb E_PZ_t=1$. Strict positivity of $Z_t$ also makes the two measures equivalent. The [Radon-Nikodym derivative](../../../../radon-nikodym-derivative.md) identity gives $\mathbb E_Q[\mathbf1_AY]=\mathbb E_P[\mathbf1_AYZ_t]$, first for simple variables and then for every Q-integrable $Y$ by approximation.

Write $U=\mathbb E_Q[Y\mid\mathcal F_s]$. The density on $\mathcal F_s$ is $Z_s=\mathbb E_P[Z_t\mid\mathcal F_s]$. For every $A\in\mathcal F_s$,

$$
\mathbb E_P[\mathbf1_AZ_sU]=\mathbb E_Q[\mathbf1_AU]
=\mathbb E_Q[\mathbf1_AY]=\mathbb E_P[\mathbf1_AYZ_t].
$$

Moreover $Z_sU$ is P-integrable because $\mathbb E_P[Z_s|U|]=\mathbb E_Q|U|<\infty$. Uniqueness in the definition of [conditional expectation](../../../../conditional-expectation.md) proves

$$
\boxed{Z_s\mathbb E_Q[Y\mid\mathcal F_s]=\mathbb E_P[YZ_t\mid\mathcal F_s].}
$$

This is [conditional expectation under a martingale density](../../../../conditional-expectation-under-a-martingale-density.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the stochastic differential equations course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations course of the University of Oxford](../../../../stochastic-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
