<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $x=e^{-\beta J}$. Factoring out the [ground state](../../../../ground-state.md) [Boltzmann factor](../../../../boltzmann-factor.md) from the exact [canonical partition function](../../../../canonical-partition-function.md) gives

$$
Z=e^{\beta JL}\left\{[1+(Q-1)x]^L+(Q-1)(1-x)^L\right\}.
$$

At fixed finite $L$, the [binomial theorem](../../../../binomial-theorem.md) gives

$$
\begin{aligned}
[1+(Q-1)x]^L+(Q-1)(1-x)^L
&=1+(Q-1)\\
&\quad+[L(Q-1)-(Q-1)L]x\\
&\quad+\binom L2[(Q-1)^2+Q-1]x^2+O_{L,Q}(x^3)\\
&=Q\left[1+\binom L2(Q-1)x^2+O_{L,Q}(x^3)\right].
\end{aligned}
$$

Taking the [logarithm](../../../../logarithm.md) yields the [finite-ring low-temperature expansion](../../../../finite-ring-low-temperature-expansion.md) of the [Helmholtz free energy](../../../../helmholtz-free-energy.md),

$$
\boxed{F=-JL-\frac{\log Q}{\beta}
-\frac{L(L-1)(Q-1)}{2\beta}e^{-2\beta J}
+O_{L,Q}\!\left(\frac{e^{-3\beta J}}{\beta}\right).}
$$

The constant term is the [ground state](../../../../ground-state.md) [energy](../../../../energy-split.md). The term $-\beta^{-1}\log Q$ is the contribution of the [ground state](../../../../ground-state.md) [degeneracy factor](../../../../degeneracy-factor.md). The first thermal correction follows directly by retaining the [first excited state](../../../../first-excited-state.md) manifold:

$$
Z=e^{-\beta E_0}\left[d_0+d_1e^{-2\beta J}+\cdots\right],
\qquad \frac{d_1}{d_0}=\binom L2(Q-1).
$$

Each pair of [domain walls](../../../../domain-wall.md) costs $2J$, explaining the absence of an $e^{-\beta J}$ term. For $Q=2$, every configuration has an even number of [domain walls](../../../../domain-wall.md), so the displayed remainder improves to $O_L(e^{-4\beta J}/\beta)$.

This is an expansion for fixed $L$, not a uniform [thermodynamic limit](../../../../thermodynamic-limit.md). In particular, the small correction requires $\binom L2(Q-1)x^2\ll1$, with higher terms also controlled as $x\to0$ at fixed $L,Q$. Taking $L\to\infty$ first instead selects $\lambda_+$ and gives

$$
\lim_{L\to\infty}\frac FL=-J-\frac1\beta\log[1+(Q-1)x].
$$

Its leading correction is of order $x$. The finite-ring pair constraint and the extensive population of [domain walls](../../../../domain-wall.md) in an arbitrarily long chain explain the different ordering of these two limits.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
