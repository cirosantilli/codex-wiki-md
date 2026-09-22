<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $b=\operatorname{Br}_D(e)$. By equivariance of the [Brauer homomorphism](../../../../../../../brauer-morphism.md), $b$ is a [central idempotent](../../../../../../../central-idempotent.md) of $kK$, since $C_G(D)\le K\le N_G(D)$. The [Nagao module theorem](../../../../../../../nagao-module-theorem.md) asserts that, if $eM=M$, then

$$
\boxed{M\downarrow_K=bM\oplus(1-b)M,}
$$

and every indecomposable summand of $(1-b)M$ is relatively projective for a $p$-subgroup of $K$ not containing $D$. Because $D$ is normal in $K$, its [module vertices](../../../../../../../vertex-of-an-indecomposable-module.md) cannot contain $D$ even after $K$-conjugation.

Here is a direct proof. As an element of $(kG)^K$, $e-b$ is a linear combination of $K$-conjugation orbit sums supported outside $C_G(D)$. An orbit represented by $x$ has sum

$$
\operatorname{Tr}_{C_K(x)}^K(x).
$$

Its stabilizer $C_K(x)$ does not contain $D$. On $T=(1-b)M$, the element $e-b$ acts as the identity. Map the orbit-sum expression into $\operatorname{End}_k(M)$ by left multiplication, and compose on both sides with the $K$-linear projection onto $T$. It follows that

$$
\operatorname{id}_T\in\sum_{x\notin C_G(D)}
\operatorname{Tr}_{C_K(x)}^K\operatorname{End}_{kC_K(x)}(T).
$$

Replace each [centralizer](../../../../../../../centralizer.md) by a Sylow $p$-subgroup of it using trace transitivity and its invertible prime-to-$p$ index. Project this identity further onto an indecomposable summand $U$ of $T$. Its [endomorphism ring](../../../../../../../endomorphism-ring.md) is local by [Krull–Schmidt theorem](../../../../../../../krull-schmidt-theorem.md). A sum of nonunits cannot be the identity in a [local ring](../../../../../../../local-ring.md), so one of the trace terms is a unit $u$ in $\operatorname{End}_{kK}(U)$. Multiplying the endomorphism inside that trace by $u^{-1}$ gives $\operatorname{id}_U$ as a single relative trace. The [D. Higman criterion](../../../../../../../d-higman-criterion.md) makes $U$ relatively projective for that [Sylow subgroup](../../../../../../../sylow-subgroup.md) $Q\le C_K(x)$, and $D\nleq Q$. This proves the assertion rather than just invoking the theorem's name.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
