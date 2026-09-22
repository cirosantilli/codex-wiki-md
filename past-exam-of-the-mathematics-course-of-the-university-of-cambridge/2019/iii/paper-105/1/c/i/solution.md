<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Suppose the claimed [Poincare-Wirtinger inequality](../../../../../../../poincare-wirtinger-inequality.md) were false. There would be $u_k\in H^1(U)$ such that, after setting

$$
v_k=\frac{u_k-(u_k)_U}{\|u_k-(u_k)_U\|_{L^2(U)}},
$$

we have $(v_k)_U=0$, $\|v_k\|_2=1$, and $\|Dv_k\|_2\to0$. The sequence is bounded in $H^1(U)$, so part 1(b)(ii) supplies a subsequence converging strongly in $L^2(U)$ and weakly in $H^1(U)$ to some $v$.

The weak [gradient](../../../../../../../gradient.md) of $v$ is zero. Because $U$ is [connected](../../../../../../../connected-space.md), $v$ is a [constant function](../../../../../../../constant-function.md); its mean is zero, so $v=0$. Strong convergence would then give $\|v_k\|_2\to0$, contradicting $\|v_k\|_2=1$. Therefore

$$
\boxed{\|u-u_U\|_{L^2(U)}\leq C_1\|Du\|_{L^2(U)}.}
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
