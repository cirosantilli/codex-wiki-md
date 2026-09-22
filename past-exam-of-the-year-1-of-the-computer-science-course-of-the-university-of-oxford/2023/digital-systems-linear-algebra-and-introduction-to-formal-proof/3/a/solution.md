<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use a [three-sample run detector](../../../../../three-sample-run-detector.md). Just before [clock edge](../../../../../clock-edge.md) $t$, let two stored [bits](../../../../../bit.md) $p$ and $q$ hold the input values at edges $t-1$ and $t-2$. Initialise both to zero. With input $a_t$, define

$$
\boxed{w_t=a_t\land p\land q,\qquad p'=a_t,\qquad q'=p.}
$$

Primes denote the next stored state, with all assignments simultaneous at the [clock edge](../../../../../clock-edge.md). The output is the [logical conjunction](../../../../../logical-conjunction.md) of the present input and its two preceding samples. By induction on [clock edges](../../../../../clock-edge.md), the stated interpretation of $p,q$ is maintained, proving the required behaviour. Two [bits](../../../../../bit.md) of state suffice.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Digital systems](../../digital-systems.md)
4. [Digital systems, linear algebra and introduction to formal proof](../../../digital-systems-linear-algebra-and-introduction-to-formal-proof-split.md)
5. [2023](../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
