<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) for [bounded linear functionals](../../../../../continuous-linear-functional.md) says that a [bounded linear functional](../../../../../continuous-linear-functional.md) on any [linear subspace](../../../../../vector-subspace.md) of a [normed vector space](../../../../../normed-vector-space.md) extends to the whole space with its [norm](../../../../../norm.md) unchanged. No closedness or completeness of the subspace is required. Question 1 uses real-valued $\ell_\infty(\Gamma)$, so its operator assertions are read over the real scalar field. The analogous complex statements use complex-valued indexed functions.

For $x\ne0$, define $g(tx)=t\|x\|$ on its one-dimensional span. This is a norm-one functional, so [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) supplies an extension $f\in X^*$ with

$$
\boxed{\|f\|=1,\qquad f(x)=\|x\|.}
$$

The [canonical embedding into the bidual](../../../../../canonical-embedding-into-the-bidual.md) is $Jx(f)=f(x)$. It is linear and $\|Jx\|\le\|x\|$. The [bounded linear functional](../../../../../continuous-linear-functional.md) just constructed gives the reverse inequality for nonzero $x$, and the zero case is immediate. Thus $\boxed{\|Jx\|=\|x\|}$ and $J$ is injective.

For the [coordinate functional representation of an operator into bounded indexed functions](../../../../../coordinate-functional-representation-of-an-operator-into-bounded-indexed-functions.md), let $e_\gamma$ evaluate a coordinate and put $f_\gamma=e_\gamma T$. If $T$ is bounded and linear, then $f_\gamma\in X^*$ and $\|f_\gamma\|\le\|T\|$. Conversely, if $M=\sup_\gamma\|f_\gamma\|<\infty$, the formula $(Tx)(\gamma)=f_\gamma(x)$ defines a bounded scalar function for each $x$, is linear, and satisfies $\|Tx\|_\infty\le M\|x\|$. Combining the two estimates gives

$$
\boxed{T\in\mathcal B(X,\ell_\infty(\Gamma))\iff\sup_\gamma\|f_\gamma\|<\infty,
\qquad\|T\|=\sup_\gamma\|f_\gamma\|.}
$$

For an empty index set both spaces/families have [norm](../../../../../norm.md) bound zero; the [supremum](../../../../../supremum.md) of the empty nonnegative family is taken as zero.

Choose $\Gamma=B_{X^*}$ and $Tx=(f(x))_{f\in B_{X^*}}$. The [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) makes $\|Tx\|_\infty=\|x\|$, so this is a linear [isometric embedding](../../../../../isometric-embedding.md) into [bounded scalar functions on an index set](../../../../../bounded-scalar-functions-on-an-index-set.md).

If $X$ is nonzero and separable, choose a dense sequence $u_n$ in its unit sphere and supporting functionals $f_n$ with $\|f_n\|=f_n(u_n)=1$. For a unit vector $u$ and $\epsilon>0$, some $u_n$ satisfies $\|u-u_n\|<\epsilon$, whence $|f_n(u)|\ge1-\epsilon$. Thus $(f_n)$ is a [countable norming family](../../../../../countable-norming-family.md) and $x\mapsto(f_n(x))$ is an [isometry](../../../../../isometry.md) into the [l-infinity sequence space](../../../../../l-infinity-sequence-space.md). Completeness of $X$ is not needed.

If instead $X=E^*$ for a separable [normed vector space](../../../../../normed-vector-space.md) $E$, choose a dense sequence $v_n$ in $B_E$. The evaluations $f_n(x)=x(v_n)$ lie in $B_{X^*}$ and continuity of $x\in E^*$ gives $\sup_n|x(v_n)|=\|x\|$. This again gives $\Gamma=\mathbb N$, even when $E^*$ is not separable. If $X=\{0\}$, use zero coordinates throughout.

To prove 1-injectivity, take $T:Y\to\ell_\infty(\Gamma)$ on a subspace of $Z$. Extend every coordinate $f_\gamma\in Y^*$ to $\widetilde f_\gamma\in Z^*$ by [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md), keeping its [norm](../../../../../norm.md). Their uniform bound defines $\widetilde Tz=(\widetilde f_\gamma(z))$, and the coordinate [norm](../../../../../norm.md) identity yields

$$
\boxed{\widetilde T|_Y=T,\qquad\|\widetilde T\|=\|T\|.}
$$

Selection of these extensions uses the usual choice convention for arbitrary index sets. This verifies the [lambda-injective normed space](../../../../../lambda-injective-normed-space.md) definition with $\lambda=1$.

For the final [retraction characterization of lambda-injectivity](../../../../../retraction-characterization-of-lambda-injectivity.md), suppose first that $X$ is lambda-injective and $i:X\to Z$ is a linear [isometry](../../../../../isometry.md). The inverse $i(X)\to X$ has [norm](../../../../../norm.md) one when $X\ne0$; extend it to $P:Z\to X$ with $\|P\|\le\lambda$. Then $Pi=I_X$, and $iP$ is a bounded projection onto $i(X)$. For the zero space take $P=0$.

Conversely, suppose every linear [isometry](../../../../../isometry.md) out of $X$ has such a left inverse. Fix an [isometry](../../../../../isometry.md) $j:X\to\ell_\infty(\Gamma)$ as above and a left inverse $P$ with $\|P\|\le\lambda$. For any $T:Y\to X$, extend $jT$ to $S:Z\to\ell_\infty(\Gamma)$ by 1-injectivity. Then $\widetilde T=PS$ extends $T$, and $\|\widetilde T\|\le\lambda\|S\|=\lambda\|T\|$. Therefore $X$ is lambda-injective exactly when every isometric embedding $i:X\to Z$ admits a bounded map $P:Z\to X$ satisfying

$$
\boxed{Pi=I_X,\qquad\|P\|\le\lambda.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
