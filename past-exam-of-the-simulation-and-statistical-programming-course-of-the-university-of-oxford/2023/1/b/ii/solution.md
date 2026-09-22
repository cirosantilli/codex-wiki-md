<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Stop [rejection sampling](../../../../../rejection-sampling.md) when exactly $N=66{,}564$ target draws have been accepted. The total proposal count $T_N$ is a sum of $N$ [independent](../../../../../independent-random-variables.md) waiting times with [geometric distribution](../../../../../geometric-distribution.md), equivalently a [negative binomial distribution](../../../../../negative-binomial-distribution.md) counting trials. Consequently

$$
\boxed{\mathbb ET_N=MN=66{,}564M,\qquad\operatorname{Var}(T_N)=NM(M-1).}
$$

The accepted-sample [Monte Carlo estimator](../../../../../monte-carlo-estimator.md) then has the approximate $99\%$ precision from (a)(iii). The displayed proposal cost is an [expected value](../../../../../expected-value-split.md), which need not be an integer. Spending this many proposals in advance does not ensure that $N$ target draws will have been accepted.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
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
