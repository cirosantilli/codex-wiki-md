<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $K=\Sigma^{-1}$ be the [precision matrix](../../../../../../precision-matrix.md), let $R=\{1,\ldots,p\}\setminus\{j,k\}$, and condition on $V_R=v_R$. In the Gaussian exponent, all terms depending jointly on $v_j$ and $v_k$ are contained in

$$
-\frac12\left(K_{jj}v_j^2+2K_{jk}v_jv_k+K_{kk}v_k^2
+2b_j(v_R)v_j+2b_k(v_R)v_k\right).
$$

If $K_{jk}=0$, this conditional density is a product of one function of $v_j$ and one function of $v_k$, so the [conditional independence](../../../../../../conditional-independence.md) of $V_j$ and $V_k$ given $V_R$ holds.

Conversely, conditional independence makes this everywhere-positive conditional density factorize. Its mixed second derivative must therefore vanish:

$$
\frac{\partial^2}{\partial v_j\partial v_k}
\log f(v_j,v_k\mid v_R)=-K_{jk}=0.
$$

**Hence the conditional independence holds exactly when $(\Sigma^{-1})_{jk}=0$.**

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
