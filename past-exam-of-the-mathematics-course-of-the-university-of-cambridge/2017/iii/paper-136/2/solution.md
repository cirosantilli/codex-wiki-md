<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

On [continuous functions on the p-adic integers](../../../../../continuous-functions-on-the-p-adic-integers.md), define the [forward difference operator](../../../../../forward-difference-operator.md) and the [Mahler coefficients](../../../../../mahler-coefficient.md) by

$$
(\Delta f)(x)=f(x+1)-f(x),\qquad
 a_n(f)=(\Delta^nf)(0)=\sum_{j=0}^n(-1)^{n-j}\binom nj f(j).
$$

Writing $S f(x)=f(x+1)$, the explicit iterate follows from $\Delta^n=(S-I)^n$. The [ultrametric inequality](../../../../../ultrametric-inequality.md) and integral [binomial coefficients](../../../../../binomial-coefficient.md) imply $\|\Delta f\|_\infty\leq\|f\|_\infty$ and $|a_n(f)|_p\leq\|f\|_\infty$, where the [supremum norm](../../../../../supremum-norm.md) is taken over $\mathbb Z_p$.

The [Mahler theorem](../../../../../mahler-s-theorem.md) states that every such $f$ has a unique expansion with [uniform convergence](../../../../../uniform-convergence.md)

$$
\boxed{f(x)=\sum_{n=0}^{\infty}a_n(f)\binom xn,\qquad a_n(f)\longrightarrow0.}
$$

Conversely, every sequence in $\mathbb Q_p$ tending to zero yields a [continuous function](../../../../../continuous-function.md) by this expansion. The [binomial polynomials](../../../../../binomial-polynomial.md) form an orthonormal expansion in the non-Archimedean sense: $\|f\|_\infty=\sup_n|a_n(f)|_p$.

Here is the requested proof under the permitted coefficient-decay assumption. For $n\geq1$, the [binomial polynomial](../../../../../binomial-polynomial.md) $B_n(x)=x(x-1)\cdots(x-n+1)/n!$ is a [continuous function](../../../../../continuous-function.md) on $\mathbb Z_p$. Its values on nonnegative integers are integral, and those integers are dense in the [p-adic integers](../../../../../p-adic-integer.md). Since $\mathbb Z_p$ is a [closed set](../../../../../closed-set.md) in $\mathbb Q_p$, $B_n(\mathbb Z_p)\subseteq\mathbb Z_p$. Also $B_n(n)=1$, so $\|B_n\|_\infty=1$, including $B_0=1$.

If $a_n\to0$, the [ultrametric inequality](../../../../../ultrametric-inequality.md) gives the uniform tail bound

$$
\left\|\sum_{n=N}^M a_nB_n\right\|_\infty\leq\max_{N\leq n\leq M}|a_n|_p\longrightarrow0.
$$

Completeness of $\mathbb Q_p$ gives a uniform limit $F$, and the [uniform limit theorem](../../../../../uniform-limit-theorem.md) makes $F$ continuous. At any nonnegative integer $m$, all $B_n(m)$ with $n>m$ vanish. Finite binomial inversion gives

$$
\sum_{n=0}^m\binom mn a_n
=\sum_{j=0}^m f(j)\binom mj\sum_{n=j}^m(-1)^{n-j}\binom{m-j}{n-j}
=f(m),
$$

since the inner sum is $(1-1)^{m-j}$. Hence $F=f$ on a [dense subset](../../../../../dense-set.md) and therefore on all of $\mathbb Z_p$. The values at $m=0,1,2,\ldots$ recover each coefficient recursively because $B_m(m)=1$; this proves uniqueness. The expansion bounds $\|f\|_\infty$ by $\sup|a_n|_p$, and the earlier coefficient inequality proves equality. This also proves the converse statement.

Although the problem allows us to assume decay, it can be established independently. By [compactness](../../../../../compact-space.md) and [uniform continuity](../../../../../uniform-continuity.md), approximate $f$ uniformly by $h$ constant on residue classes modulo $p^r$. On this finite-dimensional space, $S^{p^r}=I$ and

$$
(S-I)^{p^r}\equiv S^{p^r}-I=0\pmod p.
$$

The matrix of $\Delta^{p^r}$ has entries divisible by $p$, so its operator norm is at most $p^{-1}$; consequently $\|\Delta^{jp^r+s}h\|_\infty\leq p^{-j}\|h\|_\infty$ for $0\leq s<p^r$. Thus $a_n(h)\to0$. Since $|a_n(f)-a_n(h)|_p\leq\|f-h\|_\infty$, arbitrary uniform approximation proves [automatic decay of Mahler coefficients](../../../../../automatic-decay-of-mahler-coefficients.md).

For the last claim, construct the [discrete antidifferentiation on the p-adic integers](../../../../../discrete-antidifferentiation-on-the-p-adic-integers.md)

$$
G(x)=\sum_{n=0}^{\infty}a_n(f)\binom{x}{n+1}.
$$

Its coefficient sequence is $0,a_0,a_1,\ldots$, still tending to zero, so it is continuous. By [Pascal's identity](../../../../../pascal-s-rule.md), $\Delta B_{n+1}=B_n$. The boundedness of $\Delta$ permits applying it to the uniform limit, giving $\Delta G=f$. For the stated [linear map](../../../../../linear-map.md), invariance under translation by one now gives

$$
T(f)=T(\Delta G)=T(G(\cdot+1))-T(G)=0.
$$

Thus [translation-invariant linear forms on p-adic continuous functions vanish](../../../../../translation-invariant-linear-forms-on-p-adic-continuous-functions-vanish.md):

$$
\boxed{T=0.}
$$

No [continuity](../../../../../continuous-function.md) of $T$ has been assumed or used. In particular, one must not justify this by applying $T$ termwise to an infinite [Mahler expansion](../../../../../mahler-s-theorem.md); it is the existence of a continuous [discrete antiderivative](../../../../../discrete-antiderivative.md) that makes the conclusion valid.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 136](../../paper-136-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
