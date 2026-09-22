<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $A=kG$, $N=N_G(D)$ and $C=C_G(D)$. The [Brauer morphism](../../../../../../brauer-morphism.md) is the coefficient projection

$$
\operatorname{Br}_D^G:A^D\longrightarrow kC,\qquad\sum_{g\in G}a_gg\longmapsto\sum_{g\in C}a_gg,
$$

where the superscript $D$ denotes invariance under conjugation. This is an algebra homomorphism: for $c\in C$, the pairs $(x,y)$ with $xy=c$ are permuted by $D$; their coefficient products are constant on each orbit. Every nonfixed orbit has size divisible by $p$ and contributes zero. The fixed pairs are exactly $x,y\in C$, giving the coefficient of $c$ in the product of the projections. It is surjective since $kC\subset A^D$.

We need two trace facts. The kernel is

$$
\ker\operatorname{Br}_D^G=\sum_{Q<D}\operatorname{Tr}_Q^D(A^Q).
$$

Indeed, a basis of $A^D$ consists of conjugation-orbit sums. Nonfixed orbit sums are traces from their proper stabilizers, while fixed basis elements are exactly the elements of $C$. Traces from proper subgroups have zero coefficient at every fixed element, proving the reverse inclusion. Second, [Brauer morphism and relative trace](../../../../../../brauer-morphism-and-relative-trace.md) gives

$$
\operatorname{Br}_D^G\bigl(\operatorname{Tr}_D^G(a)\bigr)=\operatorname{Tr}_D^N\bigl(\operatorname{Br}_D^G(a)\bigr).
$$

One can see this by letting $D$ act on the cosets $G/D$: fixed cosets are exactly $N/D$, and all other orbit contributions vanish after projection. More generally, $\operatorname{Br}_E^G(\operatorname{Tr}_D^G(A^D))=0$ unless $E$ is conjugate into $D$.

Set $I_D=\operatorname{Tr}_D^G(A^D)$ and $J_D=\operatorname{Tr}_D^N(kC)=(kC)_D^N$. The first is an ideal of the [center of an associative algebra](../../../../../../center-of-an-associative-algebra.md) $Z(A)$; the second is an ideal of $(kC)^N$, which is commutative because $C\subset N$. The displayed trace identity and surjectivity of the Brauer projection give a surjective algebra homomorphism

$$
\operatorname{Br}_D^G:I_D\twoheadrightarrow J_D.
$$

The ideals can lack identities, so we justify the required idempotent argument. A finite-dimensional commutative algebra is a product of [Artinian local rings](../../../../../../artinian-local-ring.md). Its ideal intersects each local factor either in the whole factor, containing its identity, or in a proper [nilpotent ideal](../../../../../../nilpotent-ideal.md). Under a surjection of such ideals, the proper parts have nilpotent image. Each nonzero image of a local-factor identity has a local corner algebra, a quotient of that factor, and is therefore primitive. If $u$ is the sum of these nonzero images, then $j-uj$ lies in the nilpotent image of the proper-factor ideals for every $j$ in the target; an idempotent has $j-uj=0$. Its components in the local corners are consequently zero or the corner identities. These orthogonal images account for every primitive idempotent in the target, because what remains is nilpotent. Thus [primitive idempotents under a surjection of commutative Artinian ideals](../../../../../../primitive-idempotents-under-a-surjection-of-commutative-artinian-ideals.md) apply: the primitive idempotents of $J_D$ correspond exactly to primitive central idempotents $b\in I_D$ with $\operatorname{Br}_D^G(b)\ne0$.

To identify these with the required blocks, we prove the [trace criterion for defect groups](../../../../../../trace-criterion-for-defect-groups.md). Choose a subgroup $D_0$ of smallest order with $b\in I_{D_0}$. Such a subgroup exists: for a Sylow $p$-subgroup $P$, $b=\operatorname{Tr}_P^G(b/[G:P])$. If $\operatorname{Br}_{D_0}^G(b)=0$, write $b=\operatorname{Tr}_{D_0}^G(a)$ and replace $a$ by $ba$. The kernel formula and transitivity of trace would give

$$
b\in\sum_{Q<D_0}I_Q.
$$

Multiplying by $b$ gives the identity of the local algebra $bZ(A)$ in a sum of the ideals $bI_Q$. If all were proper, they would lie in its unique maximal ideal; hence some $bI_Q$ contains $b$, contradicting minimality. Therefore $\operatorname{Br}_{D_0}^G(b)\ne0$.

The general trace-vanishing assertion shows that any $E$ with nonzero Brauer image is conjugate into $D_0$. Conversely, every conjugate of $D_0$ has nonzero image. Hence the maximal such subgroups, each called a [defect group of a block](../../../../../../defect-group-of-a-block.md), are precisely the conjugates of $D_0$. It also follows, using trace transitivity, that $b\in I_D$ if and only if a defect group is conjugate into $D$. Combining this with $\operatorname{Br}_D^G(b)\ne0$ forces equality of the subgroup orders, so the idempotents singled out above are exactly those with defect group $D$.

We have proved the desired bijection

$$
\boxed{b\longmapsto\operatorname{Br}_D^G(b):\{\text{blocks of }kG\text{ with defect }D\}\overset{\sim}{\longrightarrow}\operatorname{Prim}(J_D)}.
$$

Finally, [Brauer first main theorem](../../../../../../brauer-first-main-theorem.md) states that these blocks correspond bijectively to the blocks of $kN_G(D)$ with defect group $D$. Apply the same argument to $N$: its normalizer of $D$ is itself and its centralizer of $D$ is still $C$. The target ideal is therefore the same $J_D$. Matching the two bijections proves the theorem and gives the [Brauer correspondence](../../../../../../brauer-correspondence.md), characterized by equal nonzero Brauer images. Notice that we never assume the entire kernel on $I_D$ is nilpotent; it may kill whole blocks of smaller defect.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
