<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $p(a)$ be the true [seroprevalence](../../../../../seroprevalence.md) at age $a$, and $\lambda(a)$ the [force of infection](../../../../../force-of-infection.md), meaning the instantaneous rate of a first infection among people still uninfected. In an irreversible [serocatalytic model](../../../../../serocatalytic-model.md), people begin seronegative and retain detectable antibodies after infection. Their seronegative fraction $s(a)=1-p(a)$ obeys

$$
\frac{ds}{da}=-\lambda(a)s(a),\qquad s(0)=1.
$$

Hence

$$
\boxed{p(a)=1-\exp\left[-\int_0^a\lambda(u)\,du\right]}.
$$

Equivalently, where differentiation is possible, $\lambda(a)=p'(a)/[1-p(a)]$. This identifies the [force of infection](../../../../../force-of-infection.md) as a [hazard function](../../../../../hazard-function.md) and $1-p(a)$ as the [survival function](../../../../../survival-function.md) for remaining uninfected. For constant exposure $\lambda$, **$p(a)=1-e^{-\lambda a}$**. A single calendar-time survey reflects each birth cohort's accumulated exposure; interpreting the same age curve as a timeless age effect requires assumptions about historical transmission.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
