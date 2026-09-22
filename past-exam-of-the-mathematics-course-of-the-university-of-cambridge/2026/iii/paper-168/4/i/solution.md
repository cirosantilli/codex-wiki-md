<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write the [multilinear polynomial](../../../../../../multilinear-polynomial.md) as $f=g+x_nh$, where $g$ is independent of $x_n$, $\deg g\leq k$, and $\deg h\leq k-1$. Put $m_3=\mathbb E X_n^3$. The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $|m_3|\leq\sqrt C$, and independence gives

$$
\mathbb E(g+X_nh)^4
\leq\lVert g\rVert_4^4+6\lVert g\rVert_4^2\lVert h\rVert_4^2
+4\sqrt C\,\lVert g\rVert_4\lVert h\rVert_4^3+C\lVert h\rVert_4^4.
$$

Choose $A=A(C)\geq1$ so large that

$$
\frac6A+\frac{2\sqrt C}{A^{3/2}}\leq2,
\qquad
\frac C{A^2}+\frac{2\sqrt C}{A^{3/2}}\leq1.
$$

Induction on $n$, using $2ab^3\leq a^2b^2+b^4$ and the orthogonal identity $\lVert f\rVert_2^2=\lVert g\rVert_2^2+\lVert h\rVert_2^2$, now yields

$$
\mathbb E f(X)^4\leq A^{2k}(\mathbb E f(X)^2)^2.
$$

If $\mathbb E X_i^3=0$ and $C\leq9$, the cubic term vanishes. Taking $A=3$ and applying the induction hypothesis gives exactly

$$
\begin{aligned}
\mathbb E f^4
&\leq9^k\lVert g\rVert_2^4
+6\cdot3^k3^{k-1}\lVert g\rVert_2^2\lVert h\rVert_2^2
+9\cdot9^{k-1}\lVert h\rVert_2^4\\
&=9^k(\lVert g\rVert_2^2+\lVert h\rVert_2^2)^2
=9^k(\mathbb E f^2)^2.
\end{aligned}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
