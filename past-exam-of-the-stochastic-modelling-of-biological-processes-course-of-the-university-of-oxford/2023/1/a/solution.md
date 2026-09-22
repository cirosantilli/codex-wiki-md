<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $n=n_1$ and $m=n_2$. The three [stoichiometric vectors](../../../../stoichiometric-vector.md) are $(1,0)$, $(0,1)$ and $(-1,-1)$. The [law of mass action](../../../../law-of-mass-action.md) gives the respective [reaction propensity functions](../../../../reaction-propensity-function.md)

$$
a_1(n,m)=2,\qquad a_2(n,m)=\frac n2,\qquad a_3(n,m)=nm.
$$

In particular, producing the second [chemical species](../../../../chemical-species.md) does not consume the first [chemical species](../../../../chemical-species.md). Since the two reactants in the third [chemical reaction](../../../../chemical-reaction-split.md) are different [chemical species](../../../../chemical-species.md), the number of possible pairs is $nm$.

For each [Markov chain state](../../../../markov-chain-state.md), the [chemical master equation](../../../../chemical-master-equation.md) adds incoming [probability](../../../../probability.md) flux and subtracts outgoing [probability](../../../../probability.md) flux:

$$
\boxed{\begin{aligned}
\frac{\partial p(n,m,t)}{\partial t}
={}&2p(n-1,m,t)+\frac n2p(n,m-1,t)\\
&+(n+1)(m+1)p(n+1,m+1,t)\\
&-\left(2+\frac n2+nm\right)p(n,m,t).
\end{aligned}}
$$

Here $p(n,m,t)=0$ if either index is negative, and the [initial condition](../../../../initial-condition.md) is $p(n,m,0)=\mathbf1_{\{n=m=0\}}$. These conventions also give the correct [chemical master equation](../../../../chemical-master-equation.md) on the coordinate axes: for example, the third [chemical reaction](../../../../chemical-reaction-split.md) has zero outgoing [reaction propensity function](../../../../reaction-propensity-function.md) when either [chemical species](../../../../chemical-species.md) is absent.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the stochastic modelling of biological processes course of the University of Oxford](../../../split.md)
5. [Stochastic modelling of biological processes course of the University of Oxford](../../../../stochastic-modelling-of-biological-processes-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
