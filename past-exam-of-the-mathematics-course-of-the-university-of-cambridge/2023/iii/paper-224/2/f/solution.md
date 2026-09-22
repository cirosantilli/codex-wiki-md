<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

On $B$, part b gives $\log_2P_n=\log_2Q^n-\log_2Q^n(B)$. Hence the [information entropy](../../../../../../information-entropy.md) of the conditional law satisfies

$$
H(X_1^n)
=-\sum_{x_1^n\in B}P_n(x_1^n)\log_2Q^n(x_1^n)
+\log_2Q^n(B).
$$

Parts d and e imply

$$
\begin{aligned}
\log_2Q^n(B)
&=H(X_1^n)+\sum_{x_1^n\in B}P_n(x_1^n)\log_2Q^n(x_1^n)\\
&\leq nH(\overline P)+n\sum_{a\in A}\overline P(a)\log_2Q(a)\\
&=-nD(\overline P\Vert Q).
\end{aligned}
$$

Exponentiation proves $Q^n(B)\leq2^{-nD(\overline P\Vert Q)}$.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [2](../../2.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
