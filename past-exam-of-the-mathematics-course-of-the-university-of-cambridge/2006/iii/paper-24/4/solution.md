<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For an [adjunction](../../../../../adjoint-functors.md) $L:\mathcal C\rightleftarrows\mathcal D:R$, with unit $\eta$ and counit $\varepsilon$, call the adjunction idempotent when the multiplication

$$
\mu=R\varepsilon L:(RL)^2\longrightarrow RL
$$

of its induced [monad](../../../../../monad.md) is invertible. We show that this [idempotent adjunction](../../../../../idempotent-adjunction.md) condition is equivalent to invertibility of $\delta=L\eta R:LR\to(LR)^2$, the comultiplication of the induced [comonad](../../../../../comonad.md).

For an [idempotent monad](../../../../../idempotent-monad.md) $T$, the unit laws imply

$$
T\eta_A=\eta_{TA}=\mu_A^{-1}.
$$

If $a:TA\to A$ is a [monad algebra](../../../../../algebra-for-a-monad.md), naturality of the unit and its algebra unit law give

$$
\eta_Aa=Ta\,\eta_{TA}=Ta\,T\eta_A=T(a\eta_A)=1_{TA},\qquad a\eta_A=1_A.
$$

Thus $\eta_A$ is an isomorphism. Apply this to the canonical algebra $R\varepsilon_B:T(RB)\to RB$: its unit law is a [triangle identity for an adjunction](../../../../../triangle-identities-for-an-adjunction.md). It follows that $\eta_{RB}$, and therefore $L\eta_{RB}$, is invertible for every $B$. Hence $\delta$ is invertible.

Apply the same argument to the dual adjunction $R^{\mathrm{op}}\dashv L^{\mathrm{op}}$. It gives the converse. **Idempotence is self-dual: the induced monad is idempotent exactly when the induced comonad is idempotent.** In particular, idempotence requires the unit to be invertible on every object in the image of the right adjoint.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
