<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

We first derive the recurrence needed for the [partition of unity](../../../../../../partition-of-unity.md). Denote an order-$r$ partition-normalized [spline](../../../../../../spline-mathematics.md) by $N_{i,r}$. For $r\geq2$, set $h_t(u)=(u-t)_+^{r-2}$, so $(u-t)h_t(u)=(u-t)_+^{r-1}$. The elementary product identities for [divided differences](../../../../../../divided-difference.md) are

$$
\begin{aligned}
[u_0,\ldots,u_s](u h(u))&=u_0[u_0,\ldots,u_s]h+[u_1,\ldots,u_s]h\\
&=u_s[u_0,\ldots,u_s]h+[u_0,\ldots,u_{s-1}]h.
\end{aligned}
$$

They follow from the [Leibniz rule for divided differences](../../../../../../leibniz-rule-for-divided-differences.md) because the divided differences of the linear factor vanish above first order. Use the first identity on $t_i,\ldots,t_{i+r-1}$ and the second on $t_{i+1},\ldots,t_{i+r}$. Subtracting cancels the common middle-block term. The defining divided-difference recurrence for $N_{i,r}$ then gives

$$
\boxed{N_{i,r}(t)=\frac{t-t_i}{t_{i+r-1}-t_i}N_{i,r-1}(t)
+\frac{t_{i+r}-t}{t_{i+r}-t_{i+1}}N_{i+1,r-1}(t).}
$$

This is the [Cox-de Boor recurrence](../../../../../../cox-de-boor-recursion-formula.md), derived here from the specified normalization rather than assumed as a partition theorem.

Extend the distinct knot sequence in both directions to a strictly increasing sequence $(t_i)_{i\in\mathbb Z}$ tending to $\pm\infty$. For order one, $N_{i,1}=\mathbf1_{[t_i,t_{i+1})}$, so the full sum equals one. All higher-order [splines](../../../../../../spline-mathematics.md) are supported on $[t_i,t_{i+r}]$, making the following sums locally finite. Reindexing the second term of the recurrence yields

$$
\begin{aligned}
\sum_{i\in\mathbb Z}N_{i,r}(t)
&=\sum_{j\in\mathbb Z}\left[\frac{t-t_j}{t_{j+r-1}-t_j}
+\frac{t_{j+r-1}-t}{t_{j+r-1}-t_j}\right]N_{j,r-1}(t)\\
&=\sum_{j\in\mathbb Z}N_{j,r-1}(t).
\end{aligned}
$$

Induction proves that the full sum is one for every order. The same recurrence gives nonnegativity: each [coefficient](../../../../../../coefficient.md) is nonnegative wherever its associated lower-order [spline](../../../../../../spline-mathematics.md) is nonzero. Removing [splines](../../../../../../spline-mathematics.md) therefore gives the [subpartition of unity for B-splines](../../../../../../subpartition-of-unity-for-b-splines.md) on the whole line.

For $t_k<t<t_{n+1}$, a [spline](../../../../../../spline-mathematics.md) with index $i\leq0$ ends no later than $t_k$, and one with $i\geq n+1$ starts no earlier than $t_{n+1}$. They all vanish, leaving exactly the indices $1,\ldots,n$. For $k\geq2$ the [splines](../../../../../../spline-mathematics.md) are continuous and vanish at their [support](../../../../../../support.md) endpoints, so the equality extends to the closed basic knot interval:

$$
\boxed{\sum_{i=1}^nN_i(t)=1,\qquad t_k\leq t\leq t_{n+1}.}
$$

If order one is allowed, the standard half-open indicator convention gives equality on $[t_1,t_{n+1})$; to include its final endpoint literally, assign the left-limit value there. This harmless endpoint convention does not change integrals or $L^\infty$ [norms](../../../../../../norm.md). For the continuous [splines](../../../../../../spline-mathematics.md) of order at least two no such convention is necessary.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
