<h1 id="26j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Because $X=\mathbb N$ is a [countable set](../../../../../../countable-set.md) and $\mu(X)=1$, some $x\in X$ satisfies $\mu(\{x\})>0$. Invariance and the inclusion $\{T^nx\}\subseteq T^{-1}\{T^{n+1}x\}$ give

$$
\mu(\{T^{n+1}x\})
=\mu(T^{-1}\{T^{n+1}x\})
\geq\mu(\{T^nx\}).
$$

If the forward [orbit](../../../../../../orbit-dynamical-system.md) contained infinitely many distinct points, their disjoint singletons would each have measure at least $\mu(\{x\})>0$, contradicting that $\mu$ is a [probability measure](../../../../../../probability-measure.md). The orbit therefore eventually enters a finite [periodic orbit](../../../../../../periodic-orbit.md) $Y$.

Now $T(Y)=Y$, so $Y\subseteq T^{-1}Y$. Since $\mu$ is invariant,

$$
\mu(T^{-1}Y\setminus Y)=\mu(T^{-1}Y)-\mu(Y)=0.
$$

Thus $Y$ belongs to the [invariant sigma-algebra](../../../../../../invariant-sigma-algebra.md) modulo null sets. It has positive measure, so the fact that $T$ is an [ergodic transformation](../../../../../../ergodicity.md) forces

$$
\boxed{\mu(Y)=1}.
$$

This is the [ergodic invariant probability on a countable state space has finite cyclic support](../../../../../../ergodic-invariant-probability-on-a-countable-state-space-has-finite-cyclic-support.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [26J](../../26j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
