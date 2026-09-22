<h1 id="d/d4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) says that if measurable $f_n\to f$ almost everywhere and $|f_n|\le g$ for an integrable $g$, then $f$ is integrable, $\int|f_n-f|\to0$, and consequently $\int f_n\to\int f$.

First derive [Fatou's lemma](../../../../../fatou-s-lemma.md) from monotone convergence. For nonnegative $u_n$, the measurable functions $v_n=\inf_{j\ge n}u_j$ increase to $\liminf u_n$, and $\int v_n\le\inf_{j\ge n}\int u_j$. Monotone convergence therefore yields $\int\liminf u_n\le\liminf\int u_n$.

Now $f$ is measurable and $|f|\le g$ almost everywhere, so is integrable. Apply [Fatou's lemma](../../../../../fatou-s-lemma.md) to $u_n=2g-|f_n-f|\ge0$, which converges almost everywhere to $2g$:

$$
\int2g\le\liminf_n\left(\int2g-\int|f_n-f|\right)
=\int2g-\limsup_n\int|f_n-f|.
$$

The last integrals are nonnegative, so they tend to zero. Finally $|\int f_n-\int f|\le\int|f_n-f|\to0$. This argument also works for complex-valued functions.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D4](../../d4.md)
3. [D](../../../d.md)
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
