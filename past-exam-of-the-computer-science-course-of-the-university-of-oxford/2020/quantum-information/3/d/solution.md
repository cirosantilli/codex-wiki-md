<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Apply parts (b)(ii) and (b)(iii), keeping the oracle's minus sign:

$$
\begin{aligned}
WV_f|e_0\rangle
&=\frac1{\sqrt N}\left[\frac{2(S_0-S_1)}N|J\rangle-|A_0\rangle+|A_1\rangle\right]\\
&=\frac1{\sqrt N}\bigl[|J\rangle-|A_0\rangle+|A_1\rangle\bigr]\\
&=\boxed{\frac2{\sqrt N}|A_1\rangle=\frac2{\sqrt N}\sum_{f(x)=1}|x\rangle.}
\end{aligned}
$$

The middle equality uses part (a), and the last uses $|J\rangle=|A_0\rangle+|A_1\rangle$. The final squared [norm](../../../../../norm.md) is $4S_1/N=1$, providing a [normalization](../../../../../normalization.md) check.

The sign convention matters: here $W=2|e_0\rangle\langle e_0|-I$ fixes $|e_0\rangle$ and negates its [orthogonal](../../../../../orthogonal-vectors.md) complement. Its action on amplitudes is [inversion about the mean](../../../../../inversion-about-the-mean.md). The negative of this reflection would change the final [vector](../../../../../vector.md) by an overall [global phase](../../../../../global-phase.md), but mixing those conventions midway would give incorrect intermediate signs.[Section 4, diffusion transform and equation (4.0), inversion-about-average interpretation](../../../../../a-fast-quantum-mechanical-algorithm-for-database-search-by-lov-grover.md)

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Quantum information](../../../quantum-information-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
