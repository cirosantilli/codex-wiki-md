<h1 id="d/4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) states: if measurable $f_n$ converge almost everywhere to $f$ and $|f_n|\le g$ almost everywhere for an integrable $g\ge0$, then $f$ is integrable and $\int f_n\to\int f$. In fact $\int|f_n-f|\to0$.

To derive it from the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md), first prove [Fatou's lemma](../../../../../fatou-s-lemma.md). For nonnegative measurable $h_n$, the functions $k_N=\inf_{n\ge N}h_n$ increase to $\liminf h_n$ and satisfy $\int k_N\le\inf_{n\ge N}\int h_n$. [Monotone convergence](../../../../../monotone-convergence-theorem.md) yields $\int\liminf h_n\le\liminf\int h_n$.

Now $|f|\le g$ almost everywhere, so $f$ is integrable. Apply [Fatou's lemma](../../../../../fatou-s-lemma.md) to the nonnegative functions $2g-|f_n-f|$, which converge almost everywhere to $2g$:

$$
2\int g\le2\int g-\limsup_n\int|f_n-f|.
$$

Hence $\int|f_n-f|\to0$, and $|\int f_n-\int f|\le\int|f_n-f|$ proves the assertion. Common exceptional null sets may be removed at the beginning since the sequence is countable.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [4](../../4.md)
3. [D](../../../d.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
