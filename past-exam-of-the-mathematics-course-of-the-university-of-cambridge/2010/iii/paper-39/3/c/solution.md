<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The key [convexity](../../../../../../convex-function.md) calculation is that the random-walk [transition operator](../../../../../../transition-operator.md) preserves [convex functions](../../../../../../convex-function.md). If $h$ is convex, then for $0<\theta<1$,

$$
Ph(\theta x+(1-\theta)y)
=\mathbb E[h(\theta(x+\xi)+(1-\theta)(y+\xi))]
\leq\theta Ph(x)+(1-\theta)Ph(y).
$$

The [pointwise maximum of convex functions](../../../../../../pointwise-maximum-of-convex-functions.md) is convex as well: the convexity inequality holds for each candidate and is bounded above by the convex combination of the two endpoint maxima. Thus the Bellman recursion proves [convexity of a random-walk Snell value function](../../../../../../convexity-of-a-random-walk-snell-value-function.md) by backward induction from $V(T,\cdot)=f$.

To ensure that the functions in this argument are genuinely finite, rather than silently imposing a growth bound on $f$, use [integrability of translated convex random-walk rewards](../../../../../../integrability-of-translated-convex-random-walk-rewards.md). Write $Z_j$ for a sum of $j$ independent increments with the same law. For $j\leq T-1$, the assumptions give integrability of $f(Z_j)$ and $f(Z_{j+1})$. The [negative part of a finite convex function is Lipschitz](../../../../../../negative-part-of-a-finite-convex-function-is-lipschitz.md), so translating $Z_j$ preserves integrability of the negative part. For the positive part and $x>0$, if the increment law is unbounded above, take an independent increment $\eta$ and $p=\mathbb P(\eta\geq x)>0$. On that event $Z_j+x$ lies between $Z_j$ and $Z_j+\eta$, so convexity gives

$$
p\,\mathbb E[f(Z_j+x)^+]
\leq p\,\mathbb E[f(Z_j)^+]+\mathbb E[f(Z_{j+1})^+]<\infty.
$$

If increments are bounded above by $M$, then $Z_j\leq jM$ and the same convexity argument between $Z_j$ and $jM+x$ bounds the positive part by $f(Z_j)^++f(jM+x)^+$. For $x<0$, use the corresponding lower-tail argument. Thus every translated reward $f(x+Z_j)$ is integrable for $j\leq T-1$.

For $t\geq1$, backward induction also gives the bound

$$
f(x)\leq V(t,x)\leq\sum_{j=0}^{T-t}\mathbb E[f(x+Z_j)^+]<\infty.
$$

It justifies every convolution in the Bellman recursion at these times, so the arbitrary assignments outside $A_t$ in the previous part are never needed when $f$ is convex. The displayed convexity calculation therefore proves that each $V(t,\cdot)$ for $t\geq1$ is a finite convex function. The chosen $V(0,\cdot)=U_0$ is constant and hence convex. This proves the requested conclusion for the deterministic representation under the finite-horizon assumptions.

There is a distinction between this representation and a value function for every possible starting point at time zero. Without translated integrability at the full horizon, the latter may take $+\infty$ at unused states. For example, with $T=1$, $f(x)=e^{x^2}$ and $\mathbb P(\xi_1=k)=c e^{-k^2-k}$ for $k=1,2,\ldots$, the observed reward is integrable, but $\mathbb E[f(x+\xi_1)]=c e^{x^2}\sum_{k\geq1}e^{(2x-1)k}$ is infinite for $x\geq1/2$. The constant time-zero extension avoids claiming a globally finite Bellman function under insufficient assumptions. If integrability is assumed for all times of an infinite random walk, the translated-reward argument with one extra time also makes the full time-zero Bellman function finite and convex.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
