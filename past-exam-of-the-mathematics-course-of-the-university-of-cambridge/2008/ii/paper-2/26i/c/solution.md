<h1 id="26i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the $C$ equation at level $i-1$ to express $h_{C_i}$ in terms of the preceding level, then substitute it into the $W$ equation at level $i$. This yields

$$
\boxed{h^{(i)}=Ah^{(i-1)},\qquad A=\begin{pmatrix}
1+\alpha/\lambda&-\alpha/\lambda\\
\dfrac{\beta(1+\alpha/\lambda)}{\mu+\beta}&\dfrac{\mu-\beta\alpha/\lambda}{\mu+\beta}
\end{pmatrix}.}
$$

The standard eigenpair is $\boxed{1,\ (1,1)^T}$. Each row sums to one because constant functions are harmonic for every Markov generator. This recurrence matrix need not have nonnegative entries; it encodes a harmonic equation, rather than a transition matrix. The superscript $(i)$ labels the level vector and is not an additional printed subpart.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26I](../../26i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
