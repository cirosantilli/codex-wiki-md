<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [principal block](../../../../../principal-block.md) $B_0(G)$ is the unique [block of a group algebra](../../../../../block-of-a-group-algebra.md) containing the trivial $kG$-module. Its [central character of a block](../../../../../central-character-of-a-block.md) is augmentation $\varepsilon:Z(kG)\to k$, and its block idempotent $e_0$ is the unique primitive central idempotent with $\varepsilon(e_0)=1$. Its [defect groups of a block](../../../../../defect-group-of-a-block.md) are [Sylow subgroups](../../../../../sylow-subgroup.md): if $e_0=\operatorname{Tr}_D^G(a)$, augmentation gives $1=[G:D]\varepsilon(a)$, so $p\nmid[G:D]$.

The [Brauer third main theorem](../../../../../brauer-third-main-theorem.md) states that, if $b$ is a block of $kH$ with defect group $D$ and $DC_G(D)\le H\le G$, then

$$
\boxed{b^G=B_0(G)\iff b=B_0(H).}
$$

We give a proof, including the normal-subgroup ingredient needed for the difficult implication.

First, [block idempotents centralize a normal p-subgroup](../../../../../block-idempotents-centralize-a-normal-p-subgroup.md). If $P\triangleleft L$ is a [p-subgroup](../../../../../p-subgroup.md), the ideal $J(kP)kL$ is nilpotent: conjugation preserves $J(kP)$, so its powers are $J(kP)^m kL$, eventually zero. For a central idempotent $e$ of $kL$, the difference $e-\operatorname{Br}_P(e)$ is a sum of nonfixed $P$-conjugation orbit sums. Such an orbit maps to a single element of $L/P$ multiplied by its size, which is zero in $k$. Thus the difference belongs to $J(kP)kL$. Since $P$ is normal, its [centralizer](../../../../../centralizer.md) is normal too, and the Brauer image is $L$-invariant; consequently it is itself a central idempotent of $kL$. Commuting central idempotents congruent modulo a nilpotent ideal coincide: their off-diagonal products are nilpotent idempotents, hence zero. Therefore

$$
e=\operatorname{Br}_P(e)\in kC_L(P).
$$

It follows that central block idempotents of $kL$ are exactly the sums over $L$-orbits of primitive central idempotents of $kC_L(P)$. The principal block idempotent of $kC_L(P)$ is invariant under every automorphism preserving augmentation, so its singleton orbit is the principal block idempotent of $kL$.

In particular, if $PC_G(P)\le K\le L\le N_G(P)$, the groups $K,L$ have the same centralizer $C_G(P)$. Their principal block idempotents are both the principal block idempotent of $kC_G(P)$. By the definition using the [central character of a block](../../../../../central-character-of-a-block.md) of [block induction](../../../../../block-induction.md), a block of $K$ inducing to the principal block of $L$ must be principal: its idempotent, a sum of [centralizer](../../../../../centralizer.md) block [idempotents](../../../../../idempotent.md), has nonzero overlap with this single principal idempotent, and is therefore precisely that idempotent. The forward implication also holds, by the same observation.

For an arbitrary subgroup $H$ in the theorem, use the [Brauer first main theorem](../../../../../brauer-first-main-theorem.md) inside $H$ to replace $b$ by its correspondent $\beta$ in $K=N_H(D)$. This preserves principalness. Indeed a Brauer image preserves augmentation on central elements, since nonfixed $D$-orbits have sizes divisible by $p$; hence the principal block of $H$, when it has defect $D$, corresponds to the principal block of $K$. Conversely, if $\beta$ is principal, its induced [central character of a block](../../../../../central-character-of-a-block.md) is

$$
\varepsilon_K(\operatorname{Br}_D^H(z))=\varepsilon_H(z),
$$

so $\beta^H$ is principal. Transitivity gives $\beta^G=b^G$. Thus we may work with $DC_G(D)\le K\le N_G(D)$ and a block $\beta$ of defect $D$.

The forward implication is already proved by this augmentation calculation, now with $H$ replaced by $G$. For the converse, fix $G$ and suppose there is a counterexample with $\beta$ nonprincipal but $\beta^G$ principal. Choose one whose defect group $D$ has maximal order. Put $N=N_G(D)$ and $c=\beta^N$. To verify the transitivity needed here, write $B=\beta^G$. Its defining character gives $e_\beta\operatorname{Br}_D(e_B)=e_\beta$. The image $\operatorname{Br}_D(e_B)$ is $N$-invariant and central in $kN$, so the definition of $c$ gives $e_c\operatorname{Br}_D(e_B)=e_c$. If $E\ge D$ is a defect group of $c$, applying $\operatorname{Br}_E$ gives $\operatorname{Br}_E(e_c)\operatorname{Br}_E(e_B)=\operatorname{Br}_E(e_c)$, since $C_G(E)\subseteq C_G(D)$. The character defining $c^G$ therefore selects $e_B$. Thus $c^G=\beta^G$. The normal-subgroup observation shows that $c$ is nonprincipal, since otherwise $\beta$ would be principal. Every defect group of $c$ contains the normal $p$-subgroup $D$ up to conjugacy: $\operatorname{Br}_D(e_c)=e_c\ne0$. Choose a defect group $E\ge D$ of $c$. Then $C_G(E)\le C_G(D)\le N$, so $(G,N,c)$ is another admissible counterexample, now with defect group $E$. Maximality forces $E=D$.

The first main theorem applied to $N=N_G(D)$ therefore implies that the principal block $c^G$ has defect $D$. Thus $D$ is a Sylow subgroup of $G$, and also of $N$. The principal block of $N$ then has defect $D$ and, by the forward implication, induces to the principal block of $G$. Injectivity in the first main theorem gives $c=B_0(N)$, contradicting the established nonprincipalness of $c$. This proves the third main theorem.

A useful equivalent consequence, with its justification, is

$$
\operatorname{Br}_Q(e_0(G))=e_0(C_G(Q))\qquad\text{for every }p\text{-subgroup }Q.
$$

Let $a$ be a block idempotent of $kC_G(Q)$ occurring in the left side, and let $E$ be a defect group of $a$ containing the central $p$-subgroup $Q$. Then $C_G(E)\le C_G(Q)$, so $a^G$ is defined. Applying $\operatorname{Br}_E$ to $a\operatorname{Br}_Q(e_0)=a$ shows that the [central character of a block](../../../../../central-character-of-a-block.md) defining $a^G$ selects $e_0$: deleting coefficients outside $C_G(E)$ can be done after deleting those outside $C_G(Q)$. Hence $a^G=B_0(G)$, and the theorem makes $a$ principal. The image is nonzero because its augmentation is $1$, so it is exactly the principal centralizer idempotent.

Now put $C=C_G(x)$ and $P=O_p(C)$, the [p-core of a finite group](../../../../../p-core-of-a-finite-group.md). The hypothesis $O_{p'}(C)=1$, using the [p-prime core of a finite group](../../../../../p-prime-core-of-a-finite-group.md), and the definition of a [p-constrained group](../../../../../p-constrained-group.md) say $C_C(P)\le P$. The normal-subgroup observation puts every block idempotent of $kC$ inside $kC_C(P)\subseteq kP$. A [group algebra of a p-group in characteristic p is local](../../../../../group-algebra-of-a-p-group-in-characteristic-p-is-local.md), so its only idempotents are $0,1$. **Thus $kC$ has a single block, its principal block.**

Write $Q=\langle x\rangle$. By the trace and Brauer characterization of defect in Question 1,

$$
x\text{ is conjugate into }D\iff\operatorname{Br}_Q(e_B)\ne0.
$$

For the forward direction one can conjugate $Q$ into $D$; the nonzero image at $D$ then ensures the image at $Q$ is nonzero. The reverse direction follows because every subgroup with nonzero image is conjugate into a defect group. Since $kC$ has only one block, a nonzero image must equal $1=e_0(C)$. The preceding local-block argument then gives $B=B_0(G)$ by the third main theorem. Conversely, if $B$ is principal, its defect group is a Sylow subgroup and every $p$-element is conjugate into it. Therefore

$$
\boxed{x\text{ is }G\text{-conjugate to an element of }D\iff B=B_0(G).}
$$

This includes $x=1$: in that case the hypotheses force $kG$ itself to have only its principal block.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
