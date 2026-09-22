<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

On a compact [metric space](../../../../../metric-space.md) $X$, a conservative [Feller semigroup](../../../../../feller-semigroup.md) is a [strongly continuous semigroup](../../../../../c0-semigroup.md) of positive linear maps on $C(X)$ satisfying $P_t1=1$. [Positivity](../../../../../positivity-linear-maps.md) means $f\geq0\Longrightarrow P_tf\geq0$. These conditions imply sup-norm contraction. Conversely, for a [contraction semigroup](../../../../../contraction-semigroup.md) with $1\in D(L)$ and $L1=0$, differentiation on the [generator domain](../../../../../generator-domain.md) gives $\frac{d}{dt}P_t1=P_tL1=0$, so $P_t1=1$. On the real space $C(X)$, if $0\leq f\leq1$, then $\|1-P_tf\|_\infty\leq\|1-f\|_\infty\leq1$, implying $P_tf\geq0$. Scaling proves [positivity](../../../../../positivity-linear-maps.md) for every nonnegative $f$. This is the [unital contraction positivity criterion](../../../../../unital-contraction-positivity-criterion.md). For complex $C(X)$ the same conclusion follows because each functional $f\mapsto P_tf(x)$ has [norm](../../../../../norm.md) one and value one on $1$, hence is a [positive linear functional](../../../../../positive-linear-functional.md).

For each $t,x$, the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md) represents that functional by a unique [Borel probability measure](../../../../../borel-probability-measure.md) $p_t(x,dy)$:

$$
\boxed{P_tf(x)=\int_X f(y)\,p_t(x,dy).}
$$

Continuity of $P_tf$ gives weak continuity of $x\mapsto p_t(x,\cdot)$. Approximating indicators of open sets increasingly by [continuous functions](../../../../../continuous-function.md) proves Borel measurability in $x$; a monotone-class argument then gives a [Markov kernel](../../../../../markov-kernel.md). The [semigroup property](../../../../../semigroup-property.md) and uniqueness of representing measures yield $p_0(x,\cdot)=\delta_x$ and the [Chapman-Kolmogorov equation](../../../../../chapman-kolmogorov-equation.md)

$$
p_{s+t}(x,A)=\int_X p_t(y,A)\,p_s(x,dy).
$$

These are the required [transition probabilities](../../../../../transition-probability.md).

An [invariant probability measure for a semigroup](../../../../../invariant-probability-measure-for-a-semigroup.md) satisfies $\int_XP_tf\,d\mu=\int_Xf\,d\mu$ for every $t\geq0$ and $f\in C(X)$. Equivalently its distribution is preserved by the [Markov kernel](../../../../../markov-kernel.md). For $1\leq p<\infty$, [Jensen inequality](../../../../../jensen-s-inequality.md) gives $|P_tf|^p\leq P_t(|f|^p)$ pointwise. Integrating and using invariance proves

$$
\boxed{\|P_tf\|_{L^p(\mu)}\leq\|f\|_{L^p(\mu)}.}
$$

Also $\|P_tf-f\|_{L^p(\mu)}\leq\|P_tf-f\|_\infty\to0$. [Continuous functions](../../../../../continuous-function.md) are dense in these $L^p$ spaces for a finite [Borel measure](../../../../../borel-measure.md) on a compact metric space, so the contraction extends to a [strongly continuous semigroup](../../../../../c0-semigroup.md) on $L^p(\mu)$.

For real $f$ with $f,f^2\in D(L)$, the kernel form of [Jensen inequality](../../../../../jensen-s-inequality.md) gives $P_t(f^2)-(P_tf)^2\geq0$, with equality at $t=0$. Take its right [derivative](../../../../../derivative.md) to obtain the [generator square inequality](../../../../../generator-square-inequality.md)

$$
\boxed{L(f^2)\geq2fLf.}
$$

This is nonnegativity of the associated [carré du champ](../../../../../carre-du-champ-operator.md).

Each time-average functional $\phi_n$ is positive with $\phi_n(1)=1$, hence represents a [Borel probability measure](../../../../../borel-probability-measure.md) $\mu_n$. The [compactness of probability measures on a compact metric space](../../../../../compactness-of-probability-measures-on-a-compact-metric-space.md) gives a subsequence converging weakly to a probability measure $\mu$. Explicitly, $C(X)$ is a [separable Banach space](../../../../../separable-banach-space.md), so [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) and a countable dense family give a subsequence converging on every [continuous function](../../../../../continuous-function.md), rather than merely a net. For fixed $t\geq0$, the [semigroup property](../../../../../semigroup-property.md) gives the [Krylov-Bogolyubov time-average argument](../../../../../krylov-bogolyubov-theorem.md):

$$
\phi_n(P_tf)-\phi_n(f)=\frac1n\left[\int_n^{n+t}\!\int_XP_sf\,d\nu\,ds-\int_0^t\!\int_XP_sf\,d\nu\,ds\right].
$$

Its absolute value is at most $2t\|f\|_\infty/n$. Pass to the subsequential limit, observing that $P_tf\in C(X)$, to get $\int_XP_tf\,d\mu=\int_Xf\,d\mu$. Thus the limiting measure is invariant.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
