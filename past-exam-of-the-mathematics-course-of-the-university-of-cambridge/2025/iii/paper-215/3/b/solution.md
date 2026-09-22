<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Writing $a=|A\setminus B|$ and $b=|B\setminus A|$ gives

$$
\rho(A,B)=\frac{a+b+|a-b|}{2}=\max(a,b).
$$

Make two states adjacent when one can pair every disagreement except at most one, equivalently when $\rho=1$, and give every such edge length one. Pairing a deletion with an insertion as a swap and then handling the excess disagreements constructs a path of length $\max(a,b)$; every edge changes $\rho$ by at most one, so this is the corresponding path metric.

For adjacent states, couple the lazy coin and coordinate choices so that a distinguished disagreement is removed whenever its coordinate is selected, matching a compensating coordinate in the swap case. A direct check of the nested and equal-cardinality cases gives

$$
\mathbb E_{A,B}\rho(X_1,Y_1)
\leq\left(1-\frac1{2n}\right)\rho(A,B).
$$

The [Path coupling theorem](../../../../../../path-coupling-theorem.md) extends this to all pairs. Since $\operatorname{diam}(V)=k$, part (a), with $\alpha\geq1/(2n)$ up to an absolute constant, gives

$$
\boxed{t_{\mathrm{mix}}(\varepsilon)\lesssim
n\bigl(\log k+\log(1/\varepsilon)\bigr)
\lesssim n\log(k/\varepsilon).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
