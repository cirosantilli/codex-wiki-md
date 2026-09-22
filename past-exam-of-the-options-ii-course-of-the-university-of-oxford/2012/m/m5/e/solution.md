<h1 id="m/m5/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

After the third arrival, the future interarrival times are [independent](../../../../../independent-random-variables.md) of the first three interarrival times and again generate a rate-$\lambda$ [Poisson process](../../../../../poisson-process-split.md). Conditional on $T_3=t<2$, exactly three arrivals have occurred by time $t$, and the number of further arrivals before two is Poisson with mean $\lambda(2-t)$. Consequently, in the regular conditional-distribution sense at $t=1$,

$$
\boxed{N_2\mid(T_3=1)\ \sim\ 3+\operatorname{Poisson}(\lambda).}
$$

Explicitly its conditional [mass](../../../../../mass.md) is zero for $k<3$ and is

$$
\mathbb P(N_2=k\mid T_3=1)=e^{-\lambda}\frac{\lambda^{k-3}}{(k-3)!},\qquad k\geq3.
$$

This conditions on the third arrival time itself, rather than merely on the event that the third arrival has happened by time one.

## ↑ Ancestors (13)

1. [E](../e.md)
2. [M5](../../m5.md)
3. [M](../../../m.md)
4. [2012](../../../../2012-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
