<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**For a convex subset of a Banach space, weak closure equals norm closure.** The [Mazur theorem](../../../../../mazur-theorem.md) states that for every [convex set](../../../../../convex-set.md) $C\subseteq X$,

$$
\overline C^{\,w}=\overline C^{\,\|\cdot\|}.
$$

Since every [bounded linear functional](../../../../../continuous-linear-functional.md) is norm-continuous, the [weak topology](../../../../../weak-topology-split.md) is weaker than the [norm topology](../../../../../norm-topology.md), giving $\overline C^{\,\|\cdot\|}\subseteq\overline C^{\,w}$.

For the reverse inclusion, use this form of the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md): if $D$ is a nonempty norm-closed [convex set](../../../../../convex-set.md) in a real [normed vector space](../../../../../normed-vector-space.md) and $x\notin D$, there is a continuous real-linear functional $F$ such that

$$
F(x)>\sup_{d\in D}F(d).
$$

Apply it to $D=\overline C^{\,\|\cdot\|}$. In a complex [Banach space](../../../../../banach-space-split.md), use the underlying real space; every continuous real-linear $F$ is the real part of the complex [bounded linear functional](../../../../../continuous-linear-functional.md) $f(v)=F(v)-iF(iv)$. The separating strict inequality gives a neighbourhood open for the [weak topology](../../../../../weak-topology-split.md) of $x$ disjoint from $D$, so $x\notin\overline C^{\,w}$. The empty set case is immediate. This proves the [Mazur theorem](../../../../../mazur-theorem.md).

**A weakly null sequence has disjoint convex blocks converging to zero in norm.** If $x_n\xrightarrow{w}0$, then for every starting index $m$,

$$
0\in\overline{\{x_i:i\ge m\}}^{\,w}\subseteq\overline{\operatorname{conv}\{x_i:i\ge m\}}^{\,w}.
$$

The [Mazur theorem](../../../../../mazur-theorem.md) places $0$ in the norm closure of that tail [convex hull](../../../../../convex-hull.md). Thus a finite [convex combination](../../../../../convex-combination.md) of vectors from any tail can have norm less than any prescribed $\varepsilon>0$.

Choose the [convex blocks](../../../../../convex-block.md) recursively. After selecting the previous terminal index $q_{n-1}$, let $p_n>q_{n-1}$, and choose a finite [convex combination](../../../../../convex-combination.md) from $\{x_i:i\ge p_n\}$ with norm less than $2^{-n}$. Choose $q_n$ beyond its largest used index, padding the intervening coefficients and the final coefficient with zero. This ensures the printed strict condition $p_n<q_n$ as well as $q_n<p_{n+1}$. Setting unused coefficients to zero yields

$$
u_n=\sum_{i=p_n}^{q_n}a_i x_i,\qquad a_i\ge0,\qquad\sum_{i=p_n}^{q_n}a_i=1,\qquad\|u_n\|<2^{-n}.
$$

Therefore $u_n\to0$ in norm. The recursive tail selection is what makes these [convex blocks](../../../../../convex-block.md), rather than merely unrelated [convex combinations](../../../../../convex-combination.md).

Next suppose $X^*$ is separable and $(x_n)$ is bounded. Use the [canonical embedding into the bidual](../../../../../canonical-embedding-into-the-bidual.md) $J_X:X\to X^{**}$, where $J_Xx(f)=f(x)$. If $\|x_n\|\le M$, then $J_Xx_n\in M B_{X^{**}}$. The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) makes this ball compact in $\sigma(X^{**},X^*)$, and [weak-star metrizability of the dual ball](../../../../../weak-star-metrizability-of-the-dual-ball.md) makes it metrizable because its predual $X^*$ is separable. A [compact space](../../../../../compact-space.md) that is a [metric space](../../../../../metric-space.md) is sequentially compact, so some subsequence $(y_n)$ satisfies

$$
J_Xy_n\xrightarrow{w^*}\phi\in X^{**}.
$$

The limit need not belong to $J_XX$; it is precisely the use of the [bidual space](../../../../../bidual-of-a-normed-space.md) that supplies compactness without assuming reflexivity.

For a [convex block](../../../../../convex-block.md) $u_n=\sum_{i=p_n}^{q_n}a_i y_i$, every $f\in X^*$ satisfies

$$
|f(u_n)-\phi(f)|\le\sum_{i=p_n}^{q_n}a_i|f(y_i)-\phi(f)|
\le\sup_{i\ge p_n}|f(y_i)-\phi(f)|\longrightarrow0.
$$

Both $f(y_n)$ and $f(u_n)$ tend to $\phi(f)$, so

$$
\boxed{y_n-u_n\xrightarrow{w}0.}
$$

This is the useful [convex-block cancellation of a weak-star limit](../../../../../convex-block-cancellation-of-a-weak-star-limit.md); it does not require the limit to be a vector in $X$.

**The quotient sequence has approximate lifts in $3B_X$ that are weakly null after passing to a subsequence.** Let $q:X\to Z=X/Y$ be the [quotient map](../../../../../quotient-map.md), with the [quotient norm](../../../../../quotient-norm.md). Since $\|z_n\|\le1$, choose $v_n\in X$ such that

$$
q(v_n)=z_n,\qquad\|v_n\|<\frac32.
$$

This uses the infimum defining the [quotient norm](../../../../../quotient-norm.md) and does not assume that it is attained. By the preceding compactness argument, pass to a subsequence $y_n=v_{k_n}$ with a common [weak-star](../../../../../weak-star-topology.md) limit in $X^{**}$. Its quotient images $q(y_n)=z_{k_n}$ form a [weakly null sequence](../../../../../weakly-null-sequence.md).

Apply the [convex block](../../../../../convex-block.md) construction to $(q(y_n))$ in the [quotient Banach space](../../../../../quotient-banach-space.md). Using the same coefficients on $(y_n)$ gives [convex blocks](../../../../../convex-block.md)

$$
u_n=\sum_{i=p_n}^{q_n}a_i y_i,\qquad\|u_n\|<\frac32,\qquad\|q(u_n)\|\to0.
$$

Set $x_n=y_n-u_n$. The [convex-block cancellation of a weak-star limit](../../../../../convex-block-cancellation-of-a-weak-star-limit.md) proves $x_n\xrightarrow{w}0$, while

$$
\|x_n\|\le\|y_n\|+\|u_n\|<3,\qquad
\|q(x_n)-z_{k_n}\|=\|q(u_n)\|\longrightarrow0.
$$

Thus the [approximate weakly null lifting through a quotient](../../../../../approximate-weakly-null-lifting-through-a-quotient.md) is achieved with the required bound:

$$
\boxed{x_n\in3B_X,\quad x_n\xrightarrow{w}0,\quad\|q(x_n)-z_{k_n}\|\to0.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
