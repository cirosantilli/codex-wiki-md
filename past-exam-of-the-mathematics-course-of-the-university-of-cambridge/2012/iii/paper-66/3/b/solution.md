<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Combining the [EPR criterion of reality](../../../../../../epr-criterion-of-reality.md) with perfect predictive correlations and locality motivates pre-existing values for the locally selectable observables. The general [local hidden-variable theory](../../../../../../local-hidden-variable-theory.md) additionally assumes a complete shared variable $\lambda$ and conditional factorization

$$
p(A,B\mid a,b,\lambda)=p_A(A\mid a,\lambda)p_B(B\mid b,\lambda),
\qquad \rho(\lambda\mid a,b)=\rho(\lambda).
$$

The second condition is [measurement independence](../../../../../../measurement-independence.md). The reality criterion alone does not prove this factorization for arbitrary imperfect correlations: it motivates the local completion whose consequences are being tested.

A [deterministic local hidden-variable model](../../../../../../deterministic-local-hidden-variable-model.md) may be used without loss of generality by putting local random seeds into $\lambda$. For each $\lambda$, write its setting responses as $A,A',B,B'\in\{-1,1\}$. Integrating with the same setting-independent distribution and using the [triangle inequality](../../../../../../triangle-inequality.md) gives

$$
\begin{aligned}
|E(a,b)-E(a,b')|+|E(a',b)+E(a',b')|
&\leq\int d\lambda\,\rho(\lambda)
\left(|A(B-B')|+|A'(B+B')|\right)\\
&=\int d\lambda\,\rho(\lambda)
\left(|B-B'|+|B+B'|\right)=2.
\end{aligned}
$$

Exactly one of $B-B'$ and $B+B'$ vanishes and the other has magnitude two. Hence the requested **CHSH bound is two**. No assumption about the spacelike quantum state enters this local-model derivation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
