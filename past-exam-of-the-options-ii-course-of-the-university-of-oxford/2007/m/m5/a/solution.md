<h1 id="m/m5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Poisson process](../../../../../poisson-process-split.md) of rate $\lambda$ is a counting process starting at zero with independent stationary increments, with $N(t)-N(s)$ Poisson of mean $\lambda(t-s)$ for $t\ge s$, and right-continuous paths with unit jumps. Equivalently the small-interval probabilities are $\lambda h+o(h)$ for one event and $o(h)$ for two or more.

[Independence](../../../../../independent-random-variables.md) of the two processes makes their joint increments over disjoint intervals independent. On an interval of length $h$, the sum of their independent Poisson increments has [probability generating function](../../../../../probability-generating-function.md)

$$
e^{\alpha h(z-1)}e^{\beta h(z-1)}=e^{(\alpha+\beta)h(z-1)},
$$

so it is Poisson with mean $(\alpha+\beta)h$. Simultaneous arrivals have probability zero, so the sum retains unit jumps. It is therefore a [Poisson process](../../../../../poisson-process-split.md) of rate $\alpha+\beta$.

The first arrival times are independent exponential variables of rates $\alpha$ and $\beta$. For positive rates,

$$
\boxed{\mathbb P(\text{first arrival red})=\int_0^\infty\alpha e^{-\alpha t}e^{-\beta t}\,dt=\frac\alpha{\alpha+\beta}}.
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [M5](../../m5.md)
3. [M](../../../m.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
