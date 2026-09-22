<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For [Banach spaces](../../../../../banach-space-split.md) $E,F$ and $1\le p<\infty$, define the weak $p$-norm of a finite family by

$$
w_p(x_1,\ldots,x_m)=\sup_{\phi\in B_{E^*}}\left(\sum_{i=1}^m|\phi(x_i)|^p\right)^{1/p}.
$$

A [bounded linear operator](../../../../../continuous-linear-operator.md) $T:E\to F$ is an [absolutely p-summing operator](../../../../../absolutely-p-summing-operator.md) if $(\sum_i\|Tx_i\|^p)^{1/p}\le Cw_p(x_1,\ldots,x_m)$ for every finite family. The least constant is $\pi_p(T)$.

The [Pietsch factorization theorem](../../../../../pietsch-factorization-theorem.md) states that such an operator admits a [probability measure](../../../../../probability-measure.md) $\mu$ on $K=B_{E^*}$ with its [weak-star topology](../../../../../weak-star-topology.md) such that

$$
\|Tx\|\le\pi_p(T)\left(\int_K|\phi(x)|^p\,d\mu(\phi)\right)^{1/p}\qquad(x\in E).
$$

Equivalently, let $i:E\to C(K)$ be the evaluation embedding $i(x)(\phi)=\phi(x)$ and $j_p:C(K)\to L^p(\mu)$ the natural map. There is a [bounded linear operator](../../../../../continuous-linear-operator.md) $V:H\to F$, where $H=\overline{j_pi(E)}\subset L^p(\mu)$, such that $T=Vj_pi$ and $\|V\|\le\pi_p(T)$. Conversely, any such factorization makes $T$ an [absolutely p-summing operator](../../../../../absolutely-p-summing-operator.md), with $\pi_p(T)\le\|V\|$. The final operator is required on this closed subspace $H$; no extension to all of $L^p(\mu)$ is assumed.

Here is the existence proof. If $T=0$ the conclusion is immediate. Otherwise write $C=\pi_p(T)>0$. The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) makes $K$ compact, and $\phi\mapsto|\phi(x)|^p$ is continuous for each $x\in E$. For finitely many vectors $x_1,\ldots,x_m$, put

$$
v(\phi)=(|\phi(x_i)|^p)_{i=1}^m,\qquad a=(C^{-p}\|Tx_i\|^p)_{i=1}^m.
$$

We claim the compact [convex hull](../../../../../convex-hull.md) of $v(K)$ meets $a+[0,\infty)^m$. If it did not, finite-dimensional [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) would give weights $\lambda_i\ge0$ with

$$
\sup_{\phi\in K}\sum_i\lambda_i|\phi(x_i)|^p< C^{-p}\sum_i\lambda_i\|Tx_i\|^p.
$$

The weights are nonnegative because the second convex set is unbounded in every positive coordinate direction. This strict inequality contradicts the defining summing inequality applied to $\lambda_i^{1/p}x_i$. Thus a finite convex combination of the vectors $v(\phi)$ lies coordinatewise above $a$. Equivalently, a finitely supported [probability measure](../../../../../probability-measure.md) satisfies all these finitely many domination constraints.

By the [Riesz-Markov-Kakutani representation theorem](../../../../../riesz-markov-kakutani-representation-theorem.md), probability measures on compact $K$ are the positive norm-one functionals on $C(K)$ taking the constant function to one. They form a compact set in the [weak-star topology](../../../../../weak-star-topology.md), by the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md). Each domination constraint $\int|\phi(x)|^p\,d\mu\ge C^{-p}\|Tx\|^p$ is closed. The finite feasibility just proved gives the [finite intersection property](../../../../../finite-intersection-property.md), hence one measure $\mu$ satisfies every constraint.

Define $V(j_pi(x))=Tx$. The domination inequality makes this well-defined and bounded by $C$, and completeness of $F$ extends it to $H$. Conversely, any factorization satisfies

$$
\sum_i\|Tx_i\|^p\le\|V\|^p\int_K\sum_i|\phi(x_i)|^p\,d\mu(\phi)
\le\|V\|^p w_p(x_1,\ldots,x_m)^p.
$$

This proves both directions of the [Pietsch factorization theorem](../../../../../pietsch-factorization-theorem.md), including the optimal factorization norm.

For the multiplication operator, let $f\in L^p(0,1)$ and take $g_1,\ldots,g_m\in C([0,1])$. Point evaluations are norm-one [linear functionals](../../../../../linear-functional.md) on $C([0,1])$, so

$$
\sum_i\|fg_i\|_p^p
=\int_0^1|f(t)|^p\sum_i|g_i(t)|^p\,dt
\le\|f\|_p^p\sup_{t\in[0,1]}\sum_i|g_i(t)|^p
\le\|f\|_p^p w_p(g_1,\ldots,g_m)^p.
$$

Thus $M_f$ is an [absolutely p-summing operator](../../../../../absolutely-p-summing-operator.md) and $\pi_p(M_f)\le\|f\|_p$. Taking the single function $g=1$ gives the reverse inequality, so

$$
\boxed{\pi_p(M_f)=\|M_f\|=\|f\|_p.}
$$

For $f\ne0$, the explicit domination measure on $[0,1]$ is $|f(t)|^p\,dt/\|f\|_p^p$, pushed into $K$ by $t\mapsto\delta_t$. For $f=0$ everything is zero; no essential boundedness of $f$ is needed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 10](../../paper-10-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
