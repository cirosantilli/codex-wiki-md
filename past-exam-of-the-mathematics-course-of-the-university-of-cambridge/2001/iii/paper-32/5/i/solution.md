<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let a [group](../../../../../../group-split.md) $G$ act on the sample space. A statistic $T$ is a [maximal invariant](../../../../../../maximal-invariant.md) when it is invariant and separates [group orbits](../../../../../../orbit-of-a-group-action.md):

$$
T(gx)=T(x),\qquad
T(x)=T(y)\ \Longrightarrow\ y=gx\text{ for some }g\in G.
$$

Together these conditions say that $T(x)=T(y)$ exactly when $x$ and $y$ belong to the same orbit.

The basic result is that [invariant tests factor through a maximal invariant](../../../../../../invariant-tests-factor-through-a-maximal-invariant.md). Specifically, a test function $\varphi(x)\in[0,1]$ is invariant exactly when it can be written $b(T(x))$. To prove the nontrivial direction, define $b(t)=\varphi(x)$ for any representative with $T(x)=t$. Two representatives are in the same orbit by maximality, and invariance gives them the same test value, so $b$ is well-defined. Conversely $b(T(gx))=b(T(x))$ proves invariance. Measurability is taken on the quotient statistic space; for the finite rank spaces used below it is automatic.

If a null family is transitive under the [group action](../../../../../../group-action.md), the null law of $T$ is parameter-free. Indeed, if $P_{\theta'}$ is the law of $gX$ when $X\sim P_\theta$, then for every measurable set $B$,

$$
P_{\theta'}\{T\in B\}=P_\theta\{T(gX)\in B\}
=P_\theta\{T(X)\in B\}.
$$

Thus invariant procedures use exactly the information in $T$, and its common null law calibrates tests without estimating the transformed nuisance distribution. This explains the role of maximal invariants in [nonparametric statistics](../../../../../../nonparametric-statistics-split.md).

For simultaneous strictly increasing bijections of the real line, the labeled [ranks of observations](../../../../../../rank-of-an-observation.md) are a [maximal invariant](../../../../../../maximal-invariant.md) on samples without ties. Increasing maps preserve every comparison. Conversely, two such samples with the same ranks can be matched by a piecewise linear increasing bijection through their corresponding ordered observations, extended with positive-slope tails. This proves [ranks as a maximal invariant under increasing transformations](../../../../../../ranks-as-a-maximal-invariant-under-increasing-transformations.md). Under independent sampling from any common continuous distribution, every labeled ordering is equally likely by [exchangeability](../../../../../../exchangeable-random-variables.md). Hence [rank tests](../../../../../../rank-test.md) have distribution-free null calibration even without a global transitivity assertion for the entire class of continuous distributions.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
