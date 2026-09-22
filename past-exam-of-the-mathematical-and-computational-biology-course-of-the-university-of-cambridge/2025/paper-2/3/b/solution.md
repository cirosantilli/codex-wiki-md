<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The printed “otherwise” branch requires correction.** Its factor $3/4$ is the probability of ending at any of the three bases different from the initial base, not of ending at one specified different base. Assigning that probability to each of three alternatives would make a row of the [transition matrix](../../../../../stochastic-matrix.md) sum to $5/2-(3/2)e^{-\mu t}$, which exceeds one for $t>0$. This distinction is present in the source PDF, not introduced by the transcription.

For a consistent [Jukes-Cantor model](../../../../../jukes-cantor-model.md), let each ordered change from one [nucleotide](../../../../../nucleotide.md) to a specified different [nucleotide](../../../../../nucleotide.md) have instantaneous rate $q$. Its [continuous-time Markov chain](../../../../../continuous-time-markov-chain-split.md) has diagonal generator entries $-3q$ and off-diagonal entries $q$. If $p_s(t)$ is the probability of still having the same base as at time zero, its [Kolmogorov equations](../../../../../kolmogorov-equations.md) give

$$
p_s'(t)=-3q\,p_s(t)+q[1-p_s(t)]=q-4q\,p_s(t),\qquad p_s(0)=1.
$$

Solving the [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) gives

$$
p_s(t)=\frac14+\frac34e^{-4qt}.
$$

Set $\mu=4q$ to match the exponent used in the question. Symmetry then gives the properly normalized [transition probabilities](../../../../../transition-probability.md)

$$
\boxed{P_{ij}(t)=\begin{cases}\dfrac14(1+3e^{-\mu t}),&i=j,\\[2pt]\dfrac14(1-e^{-\mu t}),&i\ne j.\end{cases}}
$$

Summing the three different-base outcomes yields

$$
\boxed{P(\text{different base at }t)=\frac34(1-e^{-\mu t})}.
$$

The assumptions are a time-homogeneous [Markov process](../../../../../markov-process-split.md), the same change rate between every distinct ordered base pair, identical rates across independent sites, and no insertions or deletions. The [stationary distribution](../../../../../stationary-distribution.md) is uniform over the four bases; starting the process in that distribution is not required for this conditional calculation.

There is also a parameter-convention issue. The actual total [mutation rate](../../../../../mutation-rate.md) out of a base is $r=3q=3\mu/4$. Thus the exponent parameter $\mu$ in (b)–(d) is $4/3$ times the event rate used in the elementary counting interpretation of (a). Keeping this conversion explicit avoids changing the meaning of “mutation rate” halfway through the calculation.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
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
