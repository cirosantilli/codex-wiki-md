<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For the same uniform background and base-two [log-likelihood ratio](../../../../../log-likelihood-ratio.md), replace every [emission probability](../../../../../emission-probability.md) $b_i(x)$ by $e_i(x)=\log_2[b_i(x)/(1/4)]$. The background specifies independent letters, not a competing hidden-state process. Its single emitting state has continuation factor one when scoring a fixed-length word, so each model transition contributes $s_{ij}=\log_2 a_{ij}$; dividing every transition by $1/4$ would incorrectly count the background twice.

The complete transition-score diagram is

$$
\begin{gathered}
\mathrm{Start}\xrightarrow{0}M_1\xrightarrow{0}M_2\xrightarrow{-2}M_3\xrightarrow{-1}M_4\xrightarrow{0}\mathrm{End},\\
M_2\xrightarrow{\log_2(3/4)}I_2\xrightarrow{\log_2(3/4)}M_3,\qquad I_2\xrightarrow{-2}I_2,\\
M_3\xrightarrow{-1}I_3\xrightarrow{0}M_4.
\end{gathered}
$$

Every omitted transition has score $-\infty$. Silent Start and End supply no emission score. The complete table of emission scores is

$$
\begin{array}{c|rrrr}
\text{state}&\mathrm A&\mathrm T&\mathrm G&\mathrm C\\\hline
M_1&1&-\infty&0&0\\
M_2&-\infty&-\infty&\log_2 3&0\\
I_2&0&1&0&-\infty\\
M_3&-\infty&2&-\infty&-\infty\\
I_3&-\infty&-\infty&-\infty&2\\
M_4&0&-\infty&\log_2 3&-\infty
\end{array}.
$$

For the unique nonzero path identified in (b), add the five emission scores and all transition scores:

$$
\begin{aligned}
\text{score}
&=\underbrace{0+\log_2 3+1+2+0}_{\text{emissions}}+\underbrace{2\log_2(3/4)-1}_{\text{transitions}}\\
&=\log_2 27-2=\boxed{\log_2(27/4)}.
\end{aligned}
$$

This equals (c). For a sequence with several nonzero hidden paths, the full [log-likelihood ratio](../../../../../log-likelihood-ratio.md) is the [log-sum-exp](../../../../../log-sum-exp-function.md) of their path scores; selecting only the largest score would instead compute a best-path approximation.

## ↑ Ancestors (13)

1. [D](../d.md)
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
