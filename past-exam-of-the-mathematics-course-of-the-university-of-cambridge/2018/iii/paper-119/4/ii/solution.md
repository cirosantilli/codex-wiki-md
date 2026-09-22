<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $L\dashv R$ inducing $T$, the [Kleisli comparison functor](../../../../../../kleisli-comparison-functor.md) is always [full and faithful](../../../../../../full-and-faithful-functor.md), since the adjunction gives

$$
\mathcal D(LA,LB)\cong\mathcal C(A,RLB)=\mathcal C_T(A,B).
$$

Therefore it is part of an [equivalence of categories](../../../../../../equivalence-of-categories.md) if and only if every object of $\mathcal D$ is isomorphic to $LA$ for some $A$.

For an [idempotent monad](../../../../../../idempotent-monad.md), multiplication is invertible. The unit laws imply $T\eta=\eta T=\mu^{-1}$. If $(A,a)$ is an [algebra for a monad](../../../../../../algebra-for-a-monad.md), then $a\eta_A=1_A$, while naturality of $\eta$ gives

$$
\eta_Aa=T(a)\eta_{TA}=T(a)T(\eta_A)=T(a\eta_A)=1_{TA}.
$$

Thus $a:TA\to A$ is an isomorphism with inverse $\eta_A$. The algebra law $a\mu_A=aT(a)$ says that $a$ is a [morphism of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md) from the free algebra $(TA,\mu_A)$ to $(A,a)$, so every object of the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) is isomorphic to a free algebra. The criterion above yields

$$
\boxed{\mu\text{ invertible}\ \Longrightarrow\ \mathcal C_T\simeq\mathcal C^T.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
