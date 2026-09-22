<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For [positive linear operators on continuous functions](../../../../../../positive-linear-operator-on-continuous-functions.md), a general [Korovkin theorem](../../../../../../korovkin-theorem.md), in its [compact Korovkin test space](../../../../../../compact-korovkin-test-space.md) form, can be stated using a test space $H\subset C(K,\mathbb R)$, where $K$ is a [compact Hausdorff space](../../../../../../compact-hausdorff-space.md). Assume $H$ contains a strictly positive function $h_0$. Require that, for every $x\in K$, the only [positive linear functional](../../../../../../positive-linear-functional.md) $L$ on $C(K)$ with $L(h)=h(x)$ for all $h\in H$ is evaluation at $x$. Then **convergence on the test space implies convergence on every continuous function**:

$$
\boxed{\|U_nh-h\|_\infty\longrightarrow0\ (h\in H)
\quad\Longrightarrow\quad\|U_nf-f\|_\infty\longrightarrow0\ (f\in C(K)).}
$$

By the [Riesz-Markov-Kakutani representation theorem](../../../../../../riesz-markov-kakutani-representation-theorem.md), the functional condition equivalently says that a positive measure with these test moments must be $\delta_x$. This permits arbitrary test families, not just the interval tests $1,x,x^2$.

For completeness, let $c=\min_Kh_0>0$. Positivity gives $U_n1\leq c^{-1}U_nh_0$, so the [operator norms](../../../../../../operator-norm.md) are uniformly bounded. If the conclusion failed for some $f$, choose $x_n$ where its error is bounded away from zero. The evaluation functionals $L_n(g)=U_ng(x_n)$ have uniformly bounded norm. Compactness of $K$ and the [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) give a subnet on which $x_n\to x$ and $L_n$ converges in the [weak-star topology](../../../../../../weak-star-topology.md) to a positive $L$. For every $h\in H$, uniform test convergence gives $L(h)=h(x)$. The hypothesis forces $L(f)=f(x)$, contradicting the chosen errors. Complex-valued functions follow by applying the real result to their real and imaginary parts.

A useful concrete sufficient condition is that $1\in H$ and for each $x$ there is $g_x\in H$ with $g_x\geq0$ and zero set exactly $\{x\}$. Its zero moment forces the representing measure to be supported at $x$, while the constant moment fixes its mass.

For the circle, take $H=\operatorname{span}\{1,\sin t,\cos t\}$. The nonnegative function $g_x(t)=1-\cos(t-x)$ belongs to $H$ and vanishes only at $x$ on the circle. Thus **the periodic Korovkin test set is**

$$
\boxed{1,\ \sin x,\ \cos x.}
$$

[Uniform convergence](../../../../../../uniform-convergence.md) on these three functions is sufficient for [uniform convergence](../../../../../../uniform-convergence.md) on $C(\mathbb T)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
