<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A map $\Phi:S_D\to\mathbb R$ is [Hadamard differentiable](../../../../../hadamard-differentiability.md) at $s_0$ if there is a [continuous linear functional](../../../../../continuous-linear-functional.md) $\dot\Phi_{s_0}:S\to\mathbb R$ such that, whenever $t_j\to0$ with $t_j\ne0$, $a_j\to a$ in $S$, and $s_0+t_ja_j\in S_D$,

$$
\frac{\Phi(s_0+t_ja_j)-\Phi(s_0)}{t_j}\longrightarrow\dot\Phi_{s_0}(a).
$$

For tangential [Hadamard differentiability](../../../../../hadamard-differentiability.md), the limit directions $a$ are restricted to a specified tangent subspace and the [derivative](../../../../../derivative.md) is continuous linear on that subspace. The domain condition is indispensable.

Assume $X_n\in S_D$ almost surely and use the usual measurable, separably supported setting for norm-valued [convergence in distribution](../../../../../convergence-in-distribution.md), with the limit in the tangent space. The [functional delta method](../../../../../functional-delta-method.md) gives

$$
\boxed{r_n\bigl(\Phi(X_n)-\Phi(s_0)\bigr)\xrightarrow d\dot\Phi_{s_0}(X).}
$$

To justify this by [Skorokhod representation theorem](../../../../../skorokhod-representation-theorem.md), a sufficient precise version is: for weakly convergent random elements in a separable complete [metric](../../../../../metric.md) space, one can construct copies of the whole sequence and its limit on one probability space which converge almost surely in the [metric](../../../../../metric.md). More generally the separable-limit-support version of the representation theorem can be used. Apply it to $Z_n=r_n(X_n-s_0)$, obtaining $\widetilde Z_n\to\widetilde X$ almost surely. The variables $s_0+r_n^{-1}\widetilde Z_n$ have the same laws as $X_n$ and lie in $S_D$ on a common probability-one event. The definition of [Hadamard differentiability](../../../../../hadamard-differentiability.md), with $t_n=1/r_n$, gives convergence almost surely of the transformed quotients to $\dot\Phi_{s_0}(\widetilde X)$, and hence the claimed [convergence in distribution](../../../../../convergence-in-distribution.md). If $X$ is a [Gaussian measure](../../../../../gaussian-measure.md), the limit is Gaussian because the [derivative](../../../../../derivative.md) is linear. Without membership of $X_n$ in $S_D$, the expression $\Phi(X_n)$ in the question is not defined.

The final function space is $C_b(\mathbb R)$ with [supremum norm](../../../../../supremum-norm.md); it is not separable as a whole. This does not affect the deterministic differentiability proof below. Any statistical application of the preceding representation argument must use its separability or tightness hypotheses, rather than assuming that every normed space automatically satisfies them.

Fix admissible $F,G$ and set $T(F,G)=\int_0^uG(x)F'(x)\,dx$. The candidate [derivative](../../../../../derivative.md), defined even for continuous directions $a,b$ without [derivatives](../../../../../derivative.md), is

$$
\boxed{\dot T_{F,G}(a,b)=\int_0^ub(x)F'(x)\,dx+G(u)a(u)-G(0)a(0)-\int_0^uG'(x)a(x)\,dx.}
$$

This follows formally from the product rule and [integration by parts](../../../../../integration-by-parts.md). We now establish the uniform-direction limit required by [Hadamard differentiability](../../../../../hadamard-differentiability.md).

Let $F_j=F+t_ja_j$ and $G_j=G+t_jb_j$ belong to the stated domain, with $a_j\to a$, $b_j\to b$ in [supremum norm](../../../../../supremum-norm.md). The domain gives $\int|F_j'|\le1$ and $\int|F'|\le1$, while $F_j\to F$ uniformly. We first claim that, for every continuous $b$ on $[0,u]$,

$$
\int_0^ub(x)F_j'(x)\,dx\longrightarrow\int_0^ub(x)F'(x)\,dx.
$$

For a continuously differentiable test function $v$, [integration by parts](../../../../../integration-by-parts.md) gives convergence directly from uniform convergence of $F_j$: both boundary terms and $\int v'F_j$ converge. By the [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md), approximate $b$ uniformly on $[0,u]$ by a [polynomial](../../../../../polynomial-split.md) $v$. The difference between the two integrals introduced by this approximation is at most $2\|b-v\|_\infty$, by the uniform [bounded variation](../../../../../total-variation-of-a-function.md) bounds. Letting the approximation error decrease proves the claim. This is [weak convergence of bounded-variation integrators](../../../../../weak-convergence-of-bounded-variation-integrators.md).

Now decompose the quotient in the order that retains the bounded-variation bound:

$$
\frac{T(F_j,G_j)-T(F,G)}{t_j}
=\int_0^ub_jF_j'\,dx+\int_0^uG a_j'\,dx.
$$

The first term differs from $\int bF_j'$ by at most $\|b_j-b\|_\infty$, so it tends to $\int bF'$. For the second term, [integration by parts](../../../../../integration-by-parts.md) yields

$$
\int_0^uG a_j'=G(u)a_j(u)-G(0)a_j(0)-\int_0^uG'a_j,
$$

which tends to the corresponding expression with $a$. Hence the quotient tends to $\dot T_{F,G}(a,b)$ for every admissible perturbation sequence. Finally,

$$
|\dot T_{F,G}(a,b)|\le\|b\|_\infty+
\left(|G(u)|+|G(0)|+\int_0^u|G'|\right)\|a\|_\infty.
$$

This proves that the [derivative](../../../../../derivative.md) is a [continuous linear functional](../../../../../continuous-linear-functional.md) on the product space. Therefore **$T$ is [Hadamard differentiable](../../../../../hadamard-differentiability.md) at every point of the stated domain**. The bounded-variation restriction is what controls the apparently dangerous interaction between uniformly small perturbations and possibly large perturbation [derivatives](../../../../../derivative.md); no convergence of $a_j'$ or $b_j'$ has been assumed.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
