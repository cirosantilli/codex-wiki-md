<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The sequence has five characters, while the four [match states](../../../../../match-state.md) account for four compulsory emissions. Consequently exactly one [insertion state](../../../../../insertion-state.md) emission is needed. An insertion at $I_3$ would have to emit T, which has probability zero there. The only nonzero hidden path is therefore

$$
\mathrm{Start},\ M_1(\mathrm C),\ M_2(\mathrm G),\ I_2(\mathrm T),\ M_3(\mathrm T),\ M_4(\mathrm A),\ \mathrm{End}.
$$

Multiply its [transition probabilities](../../../../../transition-probability.md) and [emission probabilities](../../../../../emission-probability.md), including the probability of exiting $I_2$ immediately and bypassing $I_3$:

$$
\begin{aligned}
P(\texttt{CGTTA})
&=1\cdot\frac14\cdot1\cdot\frac34\cdot\frac34\cdot\frac12\cdot\frac34\cdot1\cdot\frac12\cdot\frac14\cdot1\\
&=\boxed{\frac{27}{4096}\approx0.00659180}.
\end{aligned}
$$

Normally the [forward algorithm](../../../../../forward-algorithm.md) sums over all compatible paths. Here all other paths have probability zero, so this single path gives the full sequence probability.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
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
