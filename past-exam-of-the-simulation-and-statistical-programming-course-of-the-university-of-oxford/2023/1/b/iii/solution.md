<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With a fixed budget of $n$ [independent](../../../../../independent-random-variables.md) proposal trials, the accepted count $K_n$ has [binomial distribution](../../../../../binomial-distribution.md) with success [probability](../../../../../probability.md) $1/M$. Hence

$$
\mathbb EK_n=\frac nM,
\qquad
\operatorname{Var}(K_n)=\frac{n(M-1)}{M^2}.
$$

For $M>1$, the [central limit theorem](../../../../../central-limit-theorem.md) gives the one-sided approximation

$$
\mathbb P(K_n\geq N)\approx
\Phi\!\left(\frac{n-MN}{\sqrt{n(M-1)}}\right).
$$

Use $z=2.33$, since now only the lower tail of the accepted count matters. Requiring $n-MN\geq z\sqrt{n(M-1)}$ and solving the resulting [quadratic equation](../../../../../quadratic-equation.md) in $t=\sqrt n$ gives the [one-sided normal approximation for a rejection proposal budget](../../../../../one-sided-normal-approximation-for-a-rejection-proposal-budget.md)

$$
\boxed{
n_0=\left\lceil
\left(\frac{z\sqrt{M-1}+\sqrt{z^2(M-1)+4MN}}2\right)^2
\right\rceil.}
$$

Equivalently, before rounding, this is $MN+z^2(M-1)/2+(z/2)\sqrt{(M-1)[z^2(M-1)+4MN]}$. For the value in (a)(iii),

$$
\boxed{
n_0=\left\lceil
\left(\frac{2.33\sqrt{M-1}+\sqrt{5.4289(M-1)+266256M}}2\right)^2
\right\rceil.}
$$

When $M=1$, every proposal is accepted and $\boxed{n_0=N=66{,}564}$ exactly. Otherwise the positive safety margin above $MN$ allows for random fluctuations in the number accepted. The average cost in (b)(ii) describes stopping at the $N$th acceptance; this answer chooses a deterministic budget that reaches that acceptance with approximately $99\%$ [probability](../../../../../probability.md).

The approximation requires a sufficiently accurate [normal distribution](../../../../../normal-distribution.md) approximation to the [binomial distribution](../../../../../binomial-distribution.md). An exact $99\%$ budget can instead be found from its tail probabilities. Also, a $99\%$ chance of enough accepted draws and approximate $99\%$ precision conditional on obtaining them are separate claims: their intersection is not automatically a $99\%$ event.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
