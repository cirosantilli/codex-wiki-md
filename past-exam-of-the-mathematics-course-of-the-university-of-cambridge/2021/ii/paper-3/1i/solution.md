<h1 id="1i/solution">Solution</h1>

↑ **Parent:** [1I](../1i.md)

Starting with $\theta_0=\theta$, define

$$
a_n=\lfloor\theta_n\rfloor,
\qquad
\theta_{n+1}=\frac1{\theta_n-a_n}
$$

while the denominator is nonzero. This gives the [simple continued fraction](../../../../../continued-fraction.md)

$$
\theta=[a_0;a_1,a_2,\ldots].
$$

A finite expansion is rational by evaluating it from the bottom. Conversely, for rational $\theta$, these steps are the [Euclidean algorithm](../../../../../euclidean-algorithm.md) applied to numerator and denominator, so the remainders eventually vanish.

Define convergents by

$$
p_{-2}=0, p_{-1}=1,quad q_{-2}=1, q_{-1}=0,
$$



$$
p_n=a_np_{n-1}+p_{n-2},\qquad
q_n=a_nq_{n-1}+q_{n-2}.
$$

The recurrence gives

$$
p_nq_{n-1}-p_{n-1}q_n
=-(p_{n-1}q_{n-2}-p_{n-2}q_{n-1}),
$$

so induction yields

$$
\boxed{p_nq_{n-1}-p_{n-1}q_n=(-1)^{n-1}}.
$$

In particular,

$$
\left|\frac{p_{n+1}}{q_{n+1}}-\frac{p_n}{q_n}\right|
=\frac1{q_nq_{n+1}}.
$$

Since an irrational $\theta$ lies strictly between these convergents, the two approximation errors sum to this distance. If both displayed bounds in the question failed, their sum would be at least

$$
\frac1{2q_n^2}+\frac1{2q_{n+1}^2}
\geq\frac1{q_nq_{n+1}},
$$

by the arithmetic-geometric mean inequality, contradicting strict betweenness. Thus at least one bound holds.

## ↑ Ancestors (10)

1. [1I](../1i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
