<h1 id="3/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $G=E\mathbin\square F$. To prove [convexity](../../../../../../../convex-function.md), take $u_1,u_2$ with finite $G$ values, $0<t<1$, and $\varepsilon>0$. By the definition of [infimum](../../../../../../../infimum.md), choose $v_i$ with

$$
E(v_i)+F(u_i-v_i)\leq G(u_i)+\varepsilon.
$$

Put $u_t=tu_1+(1-t)u_2$ and $v_t=tv_1+(1-t)v_2$. [Convexity](../../../../../../../convex-function.md) of $E$ and $F$ gives

$$
\begin{aligned}
G(u_t)&\leq E(v_t)+F(u_t-v_t)\\
&\leq t[E(v_1)+F(u_1-v_1)]
+(1-t)[E(v_2)+F(u_2-v_2)]\\
&\leq tG(u_1)+(1-t)G(u_2)+\varepsilon.
\end{aligned}
$$

Let $\varepsilon\downarrow0$. If either endpoint value is infinite, the convexity inequality is automatic, and $t=0,1$ gives equality. Thus **the [infimal convolution](../../../../../../../infimal-convolution.md) of two [convex functions](../../../../../../../convex-function.md) is [convex](../../../../../../../convex-function.md)** under the stated properness assumption. The proof uses approximate minimizing splits, so no attainment of the inner [infimum](../../../../../../../infimum.md) is assumed.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [3](../../../3.md)
4. [Paper 326](../../../../paper-326-split.md)
5. [Iii](../../../../split.md)
6. [2018](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
