<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The determinant in the hint is independent of $Y$ and equals the [Wronskian](../../../../../../wronskian.md)

$$
W(X)=
\begin{vmatrix}
F&F_Y\\
F_X&F_{XY}
\end{vmatrix}
=P(X)Q'(X)-P'(X)Q(X).
$$

It is nonzero because $P,Q$ are linearly independent. Also $\deg W<2n$, and coefficient convolution gives

$$
H(W)\leq2n(n+1)C^{2n}\leq C_0^n
$$

for a constant $C_0$ depending only on $C$.

Fix $y$, and suppose $F(X,y)$ has multiplicity $r$ at $a=p/q$. In

$$
W=F(X,y)Q'-F_X(X,y)Q,
$$

the two terms vanish to orders at least $r$ and $r-1$, so $W$ has multiplicity at least $r-1$ at $a$. The primitive polynomial $(qX-p)^{r-1}$ therefore divides $W$ in $\mathbb Z[X]$ by [Gauss lemma for polynomials](../../../../../../gauss-lemma-for-polynomials.md). Comparing leading coefficients gives

$$
q^{r-1}\leq H(W)\leq C_0^n.
$$

If $r>\delta n+1$, this implies $q^{\delta n}<C_0^n$ and hence $q<C_0^{1/\delta}$. Choosing $q$ larger than this bound proves that $r\leq\delta n+1$, uniformly in $y$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
