<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Draw $X_1^n$ uniformly from $B$ and let $J$ be uniform on $\{1,\ldots,n\}$ independently. Then

$$
\mathbb P(X_J=a)
=\frac1{|B|}\sum_{x_1^n\in B}\widehat P_{x_1^n}(a)
=P_B(a).
$$

If $P_i$ denotes the marginal law of $X_i$, this also says $P_B=n^{-1}\sum_iP_i$. Since $X_1^n$ is uniform on $B$,

$$
\log_2|B|=H(X_1^n).
$$

[Subadditivity of information entropy](../../../../../../subadditivity-of-information-entropy.md) followed by [concavity of information entropy](../../../../../../concavity-of-information-entropy.md) gives

$$
H(X_1^n)
\leq\sum_{i=1}^nH(P_i)
\leq nH\!\left(\frac1n\sum_{i=1}^nP_i\right)
=nH(P_B).
$$

Exponentiating proves $|B|\leq2^{nH(P_B)}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
