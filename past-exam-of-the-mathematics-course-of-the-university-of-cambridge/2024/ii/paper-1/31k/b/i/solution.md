<h1 id="31k/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $D=y^{(1)}-y^{(0)}$ and define the loss class

$$
\mathcal F=\{f_h(y^{(0)},y^{(1)},x)=D\,h(x):h\in H\}.
$$

Since $\widehat h$ minimizes $\widehat Q$,

$$
\begin{aligned}
Q(\widehat h)-Q(h^*)
&\leq (Q-\widehat Q)(\widehat h)
 +(\widehat Q-Q)(h^*).
\end{aligned}
$$

The expectation of the second term is zero. Symmetrization of the first gives

$$
\mathbb E\sup_{h\in H}(Q-\widehat Q)(h)
\leq2R_n(\mathcal F).
$$

Therefore the [expected excess-risk bound for empirical risk minimization](../../../../../../../expected-excess-risk-bound-for-empirical-risk-minimization.md) gives

$$
\boxed{\mathbb E Q(\widehat h)\leq Q(h^*)+2R_n(\mathcal F).}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [31K](../../../31k.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
