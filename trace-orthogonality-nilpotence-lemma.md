# Trace orthogonality nilpotence lemma

↑ **Parent:** [Matrix trace](matrix-trace.md)

Let $U\subseteq W\subseteq\operatorname{End}_{\mathbb C}(V)$ be [vector subspaces](vector-subspace.md) and $M=\{T:[T,W]\subseteq U\}$. If $\alpha\in M$ and $\operatorname{tr}(\alpha\beta)=0$ for all $\beta\in M$, then $\alpha$ is a [nilpotent endomorphism](nilpotent-linear-map.md).

To prove it, let $\beta$ act by $\overline\lambda$ on the [generalized eigenspace](generalized-eigenspace.md) of $\alpha$ of [eigenvalue](eigenvalue.md) $\lambda$. [Polynomial interpolation](polynomial-interpolation.md) on eigenvalue differences, together with [adjoint compatibility of additive Jordan decomposition](adjoint-compatibility-of-additive-jordan-decomposition.md), expresses $\operatorname{ad}\beta$ as a [polynomial](polynomial-split.md) in $\operatorname{ad}\alpha$ with zero constant term. Since $\operatorname{ad}\alpha$ maps $W$ into $U$ and preserves $U$, this gives $\beta\in M$. Taking the [matrix trace](matrix-trace.md) on each [generalized eigenspace](generalized-eigenspace.md) yields $0=\sum_\lambda\dim(V_\lambda)|\lambda|^2$, so every [eigenvalue](eigenvalue.md) is zero. This is the linear-algebra step behind the [Cartan solvability criterion](cartan-solvability-criterion.md); $U,W$ need not be Lie subalgebras.

## ↑ Ancestors (6)

1. [Matrix trace](matrix-trace.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-1/3/solution.md)
