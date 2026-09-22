<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Testing the [weak formulation](../../../../../../weak-formulation.md) with the [constant function](../../../../../../constant-function.md) $1$ proves the necessary compatibility condition

$$
\int_Uf=0.
$$

Assume first that $U$ is connected and this condition holds. On the [mean-zero Sobolev space](../../../../../../mean-zero-sobolev-space.md)

$$
H^1_\dagger(U)=\left\{v\in H^1(U):\int_Uv=0\right\},
$$

use the norm $\|v\|_\dagger=\|Dv\|_{L^2(U)}$. To prove the needed [Poincare-Wirtinger inequality](../../../../../../poincare-wirtinger-inequality.md), suppose it failed. There would be $v_k\in H^1_\dagger(U)$ with $\|v_k\|_2=1$ and $\|Dv_k\|_2\to0$. The [Rellich-Kondrachov compactness theorem](../../../../../../rellich-kondrachov-theorem.md) gives a subsequence converging strongly in $L^2$ and weakly in $H^1$ to a function $v$. Its [weak derivative](../../../../../../weak-derivative.md) vanishes, so connectedness makes $v$ constant; its zero mean makes it zero. This contradicts $\|v\|_2=1$. Hence $\|Dv\|_2$ is an equivalent [Hilbert space](../../../../../../hilbert-space-split.md) norm on $H^1_\dagger(U)$.

Define

$$
B(u,v)=\int_Ua^{ij}D_juD_iv,
\qquad
\ell(v)=\int_Ufv.
$$

Boundedness of $a^{ij}$ makes $B$ a [bounded bilinear form](../../../../../../bounded-bilinear-form.md), while [uniform ellipticity](../../../../../../uniformly-elliptic-operator.md) gives

$$
B(v,v)\geq\theta\|Dv\|_2^2,
$$

so it is a [coercive bilinear form](../../../../../../coercive-bilinear-form.md). The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the Poincare-Wirtinger inequality make $\ell$ a bounded [linear functional](../../../../../../linear-functional.md). The [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) supplies a unique $u\in H^1_\dagger(U)$ satisfying $B(u,v)=\ell(v)$ for every mean-zero $v$. For arbitrary $v\in H^1(U)$, subtract its mean; the omitted constant contributes zero on both sides because $D1=0$ and $\int_Uf=0$. Thus $u$ solves the original problem.

If two solutions exist, their difference $w$ satisfies $B(w,w)=0$, so uniform ellipticity gives $Dw=0$. It is therefore constant on $U$. The solution is unique up to an additive constant, and its mean-zero representative is unique. If $U$ is disconnected, the precise condition is $\int_{U_j}f=0$ on every connected component $U_j$, and one independent additive constant remains on each component.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
