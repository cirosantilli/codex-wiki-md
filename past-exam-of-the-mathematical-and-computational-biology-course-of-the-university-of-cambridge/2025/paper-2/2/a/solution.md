<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

With no deletion states allowed, each [match state](../../../../../match-state.md) must emit once in every aligned sequence. Thus the four gap-free alignment columns, $1,2,5,7$, become $M_1,M_2,M_3,M_4$. Columns $3$ and $4$ form one optional run, represented by a single looping [insertion state](../../../../../insertion-state.md) $I_2$; column $6$ requires a separate [insertion state](../../../../../insertion-state.md) $I_3$ after $M_3$. **Two insertion states are sufficient and minimal** in an ordered [profile hidden Markov model](../../../../../profile-hidden-markov-model.md): the two optional regions are separated by a compulsory emission and occupy different positions in the profile.

Estimate each [transition probability](../../../../../transition-probability.md) by the number of observed uses of that transition divided by all transitions leaving its source state. The complete arrow diagram is given below; repeated labels denote the same state, so the second and third lines supply the branches of the first line. Start and End are silent:

$$
\begin{gathered}
\mathrm{Start}\xrightarrow{1}M_1\xrightarrow{1}M_2\xrightarrow{1/4}M_3\xrightarrow{1/2}M_4\xrightarrow{1}\mathrm{End},\\
M_2\xrightarrow{3/4}I_2\xrightarrow{3/4}M_3,\qquad I_2\xrightarrow{1/4}I_2,\\
M_3\xrightarrow{1/2}I_3\xrightarrow{1}M_4.
\end{gathered}
$$

Three aligned sequences visit $I_2$, giving three exits to $M_3$, while one sequence emits twice there, giving one self-transition. Thus its exit and loop probabilities are $3/4$ and $1/4$, respectively. Two sequences visit $I_3$ and two bypass it. All absent transitions have probability zero.

The [probability mass functions](../../../../../probability-mass-function.md) of the emitting states, estimated from all characters assigned to each state with no added counts, are

$$
\begin{array}{c|rrrr}
\text{state}&\mathrm A&\mathrm T&\mathrm G&\mathrm C\\\hline
M_1&1/2&0&1/4&1/4\\
M_2&0&0&3/4&1/4\\
I_2&1/4&1/2&1/4&0\\
M_3&0&1&0&0\\
I_3&0&0&0&1\\
M_4&1/4&0&3/4&0
\end{array}.
$$

In particular, pooling the two optional columns into $I_2$ pools four emissions: two T, one A and one G. This is a generative [Hidden Markov model](../../../../../hidden-markov-model.md), so it can generate other run lengths and combinations as well as the training sequences; reproducing each training column deterministically is not its purpose.

## ↑ Ancestors (13)

1. [A](../a.md)
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
