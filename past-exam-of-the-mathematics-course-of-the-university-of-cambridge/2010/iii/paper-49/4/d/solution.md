<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write the normalized [qubit](../../../../../../qubit.md) as $|\phi\rangle=c_0|0\rangle+c_1|1\rangle$, with $|c_0|^2+|c_1|^2=1$. Only the $|1\rangle$ amplitude changes between the two [phase gates](../../../../../../phase-gate.md), so

$$
\bigl(R(\theta+\delta)-R(\theta)\bigr)|\phi\rangle
=c_1e^{i\theta}(e^{i\delta}-1)|1\rangle.
$$

Since $|e^{i\delta}-1|=2|\sin(\delta/2)|\leq|\delta|$,

$$
\boxed{\|R_m|\phi\rangle-R(\theta)|\phi\rangle\|
=2|c_1||\sin(\delta/2)|\leq|\delta|.}
$$

The [phase-gate discretization error](../../../../../../phase-gate-discretization-error.md) is uniform over all input states; its exact [operator norm](../../../../../../operator-norm.md) is $2|\sin(\delta/2)|$. To choose an approximating gate, round $N\theta/(2\pi)$ to the nearest integer and reduce it modulo $N$. Taking the shortest circular angle difference gives $|\delta|\leq\pi/N$, and hence a uniform state-vector error at most $\pi/2^n$. The circular choice handles the identified endpoints $0$ and $2\pi$ correctly.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 49](../../../paper-49-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
