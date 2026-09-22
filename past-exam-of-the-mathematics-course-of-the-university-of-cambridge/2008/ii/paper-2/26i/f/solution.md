<h1 id="26i/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Here $\vartheta<1$ is equivalent to $\mu\alpha<\lambda\beta$, which gives $b<1$ from its explicit formula. Any nonnegative solution is of the form

$$
h^{(i)}=a\begin{pmatrix}1\\1\end{pmatrix}+(1-a)\vartheta^i\begin{pmatrix}b\\1\end{pmatrix},
$$

since its second component at level zero must be one. Letting $i\to\infty$ forces $a\ge0$ for nonnegativity. The choice $a=0$ is nonnegative, and subtracting it from any other such solution gives $a[(1,1)^T-\vartheta^i(b,1)^T]\ge0$. Therefore minimality selects

$$
\boxed{h_{C_i}=b\vartheta^i,\qquad h_{W_i}=\vartheta^i.}
$$

In particular the return probability after leaving $W_0$ is $b<1$, so **the irreducible chain is transient**. These formulas are the [hitting probabilities for a velocity-switching Markov ladder](../../../../../../hitting-probabilities-for-a-velocity-switching-markov-ladder.md).

## ↑ Ancestors (11)

1. [F](../f.md)
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
