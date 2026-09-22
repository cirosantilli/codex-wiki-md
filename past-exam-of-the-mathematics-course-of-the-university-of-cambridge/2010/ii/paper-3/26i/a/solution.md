<h1 id="26i/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume the first-fork choices are independent Bernoulli routings, as in [Poisson thinning](../../../../../../poisson-thinning.md). Put $r=2\lambda/3$. Cars assigned to A form a [Poisson process](../../../../../../poisson-process.md) of rate $\lambda/3$, also an ordinary [renewal process](../../../../../../renewal-process.md) with independent exponential holding times of rate $\lambda/3$. The stream to the second fork is an independent [Poisson process](../../../../../../poisson-process.md) of rate $r$.

B receives its odd-numbered arrivals. Its initial delay is exponential of rate $r$, followed by independent [Erlang distributions](../../../../../../erlang-distribution.md) of shape two and rate $r$ between successive B arrivals. Thus **B is a delayed [renewal process](../../../../../../renewal-process.md)**, not Poisson. C receives the even-numbered arrivals: its first and all subsequent holding times are independent Erlang$(2,r)$, so **C is an ordinary [renewal process](../../../../../../renewal-process.md)**, not Poisson. Their holding-time density and survivor are $r^2t e^{-rt}$ and $e^{-rt}(1+rt)$. Both have asymptotic rate $r/2=\lambda/3$; equality of these mean rates with A does not make the processes Poisson.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26I](../../26i.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
