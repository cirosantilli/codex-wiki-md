<h1 id="5/ii/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [transition matrix](../../../../../../../stochastic-matrix.md) over five years is $P(5)=e^{5Q}$. Its first row conditions on starting in state 1. The displayed approximate probabilities mean that, five years later, about **65% remain disease-free, 6% have local recurrence only, 10% have distant metastasis only, 2% have both, and 16% have died**. They are probabilities of the states occupied at five years; they are not the probabilities of the next jump destinations or annual [transition intensities](../../../../../../../transition-intensity.md). In particular the positive [probability](../../../../../../../probability.md) of state 4 does not require a direct $1\to4$ arrow: the paths $1\to2\to4$ and $1\to3\to4$ contribute to it. The [probability](../../../../../../../probability.md) of death includes deaths after any allowed sequence of intermediate states.

The printed row sums to $0.99$ rather than one because the entries are approximate; an exact stochastic transition row sums to one. Exponentiating the displayed three-decimal generator gives approximately $(0.65377,0.06490,0.09775,0.02532,0.15826)$, illustrating that the edited, low-precision table should not be treated as an exact matrix exponential of its separately rounded rates.

State 5 is an [absorbing state](../../../../../../../absorbing-state.md), so once entered it can never be left. Its generator row is zero, and the last row of every positive-time [transition matrix](../../../../../../../stochastic-matrix.md) is therefore

$$
\boxed{(0,0,0,0,1).}
$$

This explains all four leading zeroes in the printed last row.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [Ii](../../ii.md)
3. [5](../../../5.md)
4. [Paper 37](../../../../paper-37-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
