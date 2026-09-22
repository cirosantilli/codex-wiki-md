<h1 id="s03/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

When $p_0,p_1>0$, the observed relative frequencies converge, for large sample size, to the conditional [probabilities](../../../../../probability.md)

$$
\frac{n_0}{n}\longrightarrow\frac{|\alpha|^2}{|\alpha|^2+|\beta|^2},\qquad
\frac{m_0}{m}\longrightarrow\frac{|\gamma|^2}{|\gamma|^2+|\delta|^2}.
$$

Equality says that the second binary outcome has the same distribution whichever first outcome occurred; this is [independence](../../../../../independent-random-variables.md) of these two particular measurement results. Cross-multiplication gives

$$
|\alpha|^2(|\gamma|^2+|\delta|^2)=|\gamma|^2(|\alpha|^2+|\beta|^2),
\qquad\boxed{|\alpha\delta|=|\beta\gamma|.}
$$

For finite samples the two empirical fractions fluctuate; they are estimates, not exact deterministic equalities. If $p_0=0$ or $p_1=0$, the missing conditional fraction is undefined, but one outcome is constant, so the joint measurement results are independent and the displayed modulus identity still holds.

This criterion only addresses the computational-basis statistics. For example

$$
|\chi\rangle=\tfrac12(|00\rangle+|01\rangle+|10\rangle-|11\rangle)
$$

has all four joint [probabilities](../../../../../probability.md) equal to $1/4$, yet is maximally [entangled](../../../../../entangled-state.md): its first-[qubit](../../../../../qubit.md) [density matrix](../../../../../density-matrix-split.md) is $I/2$ and $\alpha\delta=-1/4\ne1/4=\beta\gamma$. Moreover classical correlations of mixed separable states also exist, for example $\tfrac12|00\rangle\langle00|+\tfrac12|11\rangle\langle11|$. Correlations in a single basis alone neither certify nor exclude [quantum entanglement](../../../../../entangled-state.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [S03](../../../s03.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
