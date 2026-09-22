<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write

$$
H_t=(A_1,X_1,\ldots,A_{t-1},X_{t-1})
$$

for the observed history just before $A_t$. A sufficient condition is [sequential exchangeability](../../../../../../sequential-exchangeability.md)

$$
Y(a_1,\ldots,a_T)\mathrel\perp A_t\mid H_t,
\qquad t=1,\ldots,T,
$$

for every treatment regime, together with [consistency of potential outcomes](../../../../../../consistency-in-causal-inference.md) and [positivity in causal inference](../../../../../../positivity-assumption.md). Repeated conditioning then gives the longitudinal [G-formula](../../../../../../g-computation.md)

$$
\boxed{
\mathbb E[Y(\bar a_T)]
=\sum_{x_1,\ldots,x_{T-1}}
\mathbb E[X_T\mid \bar A_T=\bar a_T,\bar X_{T-1}=\bar x_{T-1}]
\prod_{t=1}^{T-1}
\mathbb P(X_t=x_t\mid\bar A_t=\bar a_t,\bar X_{t-1}=\bar x_{t-1})}.
$$

Graphically, it is enough that each $A_t$ be [D-separated](../../../../../../d-separation.md) from the final counterfactual under the specified regime after conditioning on its observed past. The two independences used in part b are precisely the $T=2$ instance.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
