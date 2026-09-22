<h1 id="2/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Write $f$ as the [ring homomorphism](../../../../../../ring-homomorphism.md) $A\to B$. By the permitted assumption, $B$ is a finitely generated $A$-algebra. We will prove that every element of $B$ is integral over $A$, including any nilpotent contribution. If $B=0$, there is nothing to prove.

We use the [integral closure as an intersection of valuation rings](../../../../../../integral-closure-as-an-intersection-of-valuation-rings.md) in its general form: if an [integral domain](../../../../../../integral-domain.md) $R$ lies in a [field](../../../../../../field.md) $K$, then its [integral closure](../../../../../../integral-closure.md) inside $K$ is the intersection of all [valuation rings](../../../../../../valuation-ring.md) of $K$ containing $R$. Here $K$ need not be the [fraction field](../../../../../../field-of-fractions.md) of $R$. One direction follows from [valuation rings are integrally closed](../../../../../../valuation-rings-are-integrally-closed.md). For the other, if $0\ne x\in K$ is not integral, the [ideal](../../../../../../ideal.md) $x^{-1}R[x^{-1}]$ is proper: an expression for $1$ in that [ideal](../../../../../../ideal.md), multiplied by a sufficiently large power of $x$, would be a monic equation for $x$. Choose a [maximal ideal](../../../../../../maximal-ideal.md) containing this [ideal](../../../../../../ideal.md), and apply the [valuation domination lemma](../../../../../../valuation-domination-lemma.md) to the corresponding [local ring](../../../../../../local-ring.md) inside $K$. The resulting [valuation ring](../../../../../../valuation-ring.md) $V$ contains $R$ and has $x^{-1}$ in its [maximal ideal](../../../../../../maximal-ideal.md), so $x\notin V$. This proves the claimed intersection criterion. The [valuation domination lemma](../../../../../../valuation-domination-lemma.md) is obtained by choosing, using [Zorn's lemma](../../../../../../zorn-s-lemma.md), a maximal local overring dominating the given [local ring](../../../../../../local-ring.md); the usual alternative between adjoining $z$ and adjoining $z^{-1}$ forces this maximal overring to be a [valuation ring](../../../../../../valuation-ring.md).

The [Noetherian ring](../../../../../../noetherian-ring.md) $B$ has finitely many minimal [prime ideals](../../../../../../prime-ideal.md) $\mathfrak q_1,\ldots,\mathfrak q_r$. Set

$$
D_i=B/\mathfrak q_i,\qquad K_i=\operatorname{Frac}(D_i),\qquad R_i=\operatorname{im}(A\to D_i).
$$

Take any [valuation ring](../../../../../../valuation-ring.md) $V$ of $K_i$ containing $R_i$. The maps $B\to D_i\to K_i$ and $A\to R_i\to V$ form a square for the [valuative criterion for properness](../../../../../../valuative-criterion-for-properness.md). Its lift gives $B\to V$, whose composite with $V\hookrightarrow K_i$ is the original map. Consequently the image $D_i$ is contained in $V$. The intersection criterion proves that every element of $D_i$ is integral over $R_i$.

Fix $b\in B$. For each $i$, choose a monic polynomial $P_i(T)\in A[T]$ whose value at the image of $b$ in $D_i$ is zero; coefficients over $R_i$ can be lifted to $A$. The product $P(T)=\prod_iP_i(T)$ is monic and satisfies

$$
P(b)\in\bigcap_i\mathfrak q_i=\sqrt{(0)}.
$$

The [nilradical](../../../../../../nilradical.md) of a [Noetherian ring](../../../../../../noetherian-ring.md) is nilpotent. Explicitly, choose finitely many generators $n_j$ with $n_j^{e_j}=0$; every product of $1+\sum_j(e_j-1)$ generators then contains a vanishing power. Thus $(\sqrt{(0)})^N=0$ for some $N$, and $P(T)^N$ is a monic polynomial annihilating $b$. Hence $B$ is integral over $A$.

Finally choose algebra generators $b_1,\ldots,b_s$, with monic equations of degrees $d_1,\ldots,d_s$. Reducing powers in these equations shows that the finitely many monomials

$$
b_1^{a_1}\cdots b_s^{a_s},\qquad 0\leq a_j<d_j,
$$

span $B$ as an $A$-[module](../../../../../../module-mathematics.md). Therefore $B$ is a finite $A$-[module](../../../../../../module-mathematics.md), proving

$$
\boxed{\text{a proper morphism between affine Noetherian schemes is finite}.}
$$

## ↑ Ancestors (11)

1. [V](../v.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
