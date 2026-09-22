<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) on the multiples of $6,8,11$ in $\{1,\ldots,527\}$. The pairwise [least common multiples](../../../../../least-common-multiple.md) are $24,66,88$, and the triple [least common multiple](../../../../../least-common-multiple.md) is $264$. Therefore the count is

$$
\begin{aligned}
&\left\lfloor\frac{527}6\right\rfloor+
\left\lfloor\frac{527}8\right\rfloor+
\left\lfloor\frac{527}{11}\right\rfloor-
\left\lfloor\frac{527}{24}\right\rfloor-
\left\lfloor\frac{527}{66}\right\rfloor-
\left\lfloor\frac{527}{88}\right\rfloor+
\left\lfloor\frac{527}{264}\right\rfloor\\
&=87+65+47-21-7-5+2=\boxed{167}.
\end{aligned}
$$

The endpoint $528$ is excluded, which is why the numerators are $527$ rather than $528$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
