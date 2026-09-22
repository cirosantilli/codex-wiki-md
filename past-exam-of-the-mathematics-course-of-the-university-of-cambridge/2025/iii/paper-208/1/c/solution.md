<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $q_i=\min(p_i,1-p_i)$. Applying part (b) after possibly replacing $X_i$ by $1-X_i$ gives $H(X_i)\leq2\sqrt{q_i}+q_i$. If $q_i<\delta_i$, then, because $0<\delta_i<1$, this is less than $3\sqrt{\delta_i}$, contradicting the assumption. Thus $p_i,1-p_i\geq\delta_i$.

The centered variables

$$
Y_i=\log P_i(X_i)+H(X_i)
$$

are independent and have mean zero. Their two possible values differ by

$$
\left|\log\frac{p_i}{1-p_i}\right|
\leq|\log\delta_i|.
$$

Applying [Hoeffding inequality](../../../../../../hoeffding-inequality.md) to $\sum_iY_i$ gives

$$
\boxed{\mathbb P\left(\log P(X_1,\ldots,X_n)+H(X_1,\ldots,X_n)\leq-t\right)
\leq\exp\left(-\frac{2t^2}{\sum_i(\log\delta_i)^2}\right).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
