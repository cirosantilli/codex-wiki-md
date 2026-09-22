<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $u$ be the infection time and $s=t-u\geq0$ its incubation delay, with independent delays having [probability density function](../../../../../../probability-density-function.md) $f(s)$. Each infection contributes to the symptom-onset intensity according to its delay density. [Back-calculation of infection incidence](../../../../../../back-calculation-of-infection-incidence.md) uses the [convolution](../../../../../../convolution.md)

$$
\boxed{\mu(t)=\int_{-\infty}^{t}h(u)f(t-u)\,du
=\int_0^\infty h(t-s)f(s)\,ds.}
$$

**Observed onset intensity is infection intensity convolved with the incubation distribution.** If infections begin at a known $t_0$, take $h(u)=0$ for $u<t_0$, reducing the first integral's lower limit to $t_0$. Otherwise past infections must be included; the observation window's start need not be the infection process's start.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
