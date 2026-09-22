<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [group](../../../../../group-split.md) $G$ is a [finitely presented group](../../../../../finitely-presented-group.md) if there is an epimorphism $F(X)\to G$ from a finite-rank [free group](../../../../../free-group.md) whose kernel is the [normal closure](../../../../../normal-closure.md) of finitely many words $R$. Equivalently, $G=\langle X\mid R\rangle$ with both $X$ and $R$ finite. [Normal closure](../../../../../normal-closure.md) means that every kernel element is a finite product of conjugates of the chosen relators or their inverses.

For [independence of finite presentation from finite generators](../../../../../independence-of-finite-presentation-from-finite-generators.md), suppose $G=\langle y_1,\ldots,y_m\mid r_1,\ldots,r_s\rangle$, and let $x_1,\ldots,x_k$ be any other finite generating set. Choose words $u_j(X)$ representing $y_j$ and words $v_i(Y)$ representing $x_i$. Consider the finite presentation

$$
P=\left\langle x_1,\ldots,x_k\ \middle|\
r_\ell(u_1(X),\ldots,u_m(X))=1,\quad
x_i=v_i(u_1(X),\ldots,u_m(X))
\right\rangle.
$$

Sending each $x_i$ to its actual element gives a surjection $P\to G$. Conversely, send $y_j$ to $u_j(X)$; the substituted relators make this a [homomorphism](../../../../../homomorphism.md) $G\to P$. Their composition on $G$ fixes every $y_j$, and their composition on $P$ fixes every $x_i$ by the extra relations. They are inverse [isomorphisms](../../../../../isomorphism.md). Hence **finite presentability is independent of the chosen finite generating set**.

For [subgroups](../../../../../subgroup.md) $A,B\leq G$ and an [isomorphism](../../../../../isomorphism.md) $\phi:A\to B$, adopt the convention

$$
G*_\phi=\langle G,t\mid t^{-1}at=\phi(a)\text{ for every }a\in A\rangle,
$$

a quotient of the [free product](../../../../../free-product.md) $G*\langle t\rangle$. The generator $t$ is the [stable letter](../../../../../stable-letter.md) of this [HNN extension](../../../../../hnn-extension.md). Fix [right coset transversals](../../../../../right-coset-transversal.md) $R_+$ for $B\backslash G$ and $R_-$ for $A\backslash G$, each with $1$ representing the [subgroup](../../../../../subgroup.md) itself. Thus each $g$ has a unique decomposition $g=br$ with $b\in B,r\in R_+$, and a unique decomposition $g=ar$ with $a\in A,r\in R_-$.

A normal form is a string

$$
g_0t^{\epsilon_1}r_1\cdots t^{\epsilon_n}r_n,\qquad
g_0\in G,\quad \epsilon_i\in\{1,-1\},\quad r_i\in R_{\epsilon_i},
$$

where $r_i\ne1$ whenever $\epsilon_{i+1}=-\epsilon_i$. The case $n=0$ is just $g_0$. The prohibition removes adjacent inverse [stable letters](../../../../../stable-letter.md) that would cancel. The following [permutation proof of HNN normal form uniqueness](../../../../../permutation-proof-of-hnn-normal-form-uniqueness.md) proves both existence and uniqueness.

Let $\mathcal N$ be the set of these formal strings. A base element $g$ acts by left multiplication on the initial coefficient $g_0$; call this permutation $L_g$. To define $L_t$, decompose the initial coefficient as $g_0=br$, with $b\in B,r\in R_+$. Unless $r=1$ and the old first [stable letter](../../../../../stable-letter.md) is $t^{-1}$, replace the initial segment by

$$
\phi^{-1}(b)\,t r.
$$

In the exceptional case, if the old string begins $b\,t^{-1}r_1\cdots$, cancel the new $t$ with that $t^{-1}$ and obtain the string beginning $\phi^{-1}(b)r_1\cdots$. These operations use the defining identity $tb=\phi^{-1}(b)t$.

Define $L_{t^{-1}}$ similarly: write $g_0=ar$ with $a\in A,r\in R_-$, prepend $\phi(a)t^{-1}r$, and cancel with an old first $t$ exactly when $r=1$. The resulting strings satisfy the normal-form conditions. These two maps are inverses. If the first operation inserts a letter, the reverse operation decomposes its new initial coefficient in the associated [subgroup](../../../../../subgroup.md) and cancels that letter. If the first operation cancels a letter, the reverse [coset](../../../../../coset.md) decomposition recovers the removed representative and reinserts it; an additional unwanted cancellation is excluded by the original normal-form condition.

The permutations satisfy $L_gL_h=L_{gh}$ and

$$
L_aL_t=L_tL_{\phi(a)}\qquad(a\in A).
$$

Indeed, in the decomposition $g_0=br$, multiplying $g_0$ on the left by $\phi(a)$ leaves its representative $r$ unchanged and changes $b$ to $\phi(a)b$. Its image under $\phi^{-1}$ is $a\phi^{-1}(b)$, exactly the coefficient produced by multiplying the normalized result on the left by $a$. The cancellation case has the same representative and the same conclusion. Therefore

$$
L_{t^{-1}}L_aL_t=L_{\phi(a)}.
$$

All defining relations of the [HNN extension](../../../../../hnn-extension.md) hold in this action, so it induces a [homomorphism](../../../../../homomorphism.md) from $G*_\phi$ into the permutations of $\mathcal N$.

Starting with the empty string, successive left multiplications normalize any word, and every normalization step uses a defining relation. This proves existence. If two normal words represented the same [group](../../../../../group-split.md) element, their induced permutations would agree. Applied to the empty string, each normal word gives exactly its own formal string, since its representatives are already chosen and all forbidden cancellations have been excluded. Thus the strings are equal. This proves the [normal form theorem for an HNN extension](../../../../../normal-form-theorem-for-an-hnn-extension.md), including the injectivity of the base [group](../../../../../group-split.md) $G\to G*_\phi$.

A [reduced sequence in an HNN extension](../../../../../reduced-sequence-in-an-hnn-extension.md) is a word

$$
g_0t^{\epsilon_1}g_1\cdots t^{\epsilon_n}g_n
$$

with no pinch $t^{-1}at$ for $a\in A$ and no pinch $tbt^{-1}$ for $b\in B$. Equivalently, if adjacent exponents are $-1,+1$, their intervening coefficient is outside $A$; if they are $+1,-1$, it is outside $B$.

Normalize such a word from right to left using the procedure above. Inductively its stable-letter length does not change. To see why, suppose the next letter has exponent $\delta$. Moving an associated-subgroup factor through it contributes to its left an element of $\phi^{-1}(B)=A$ when $\delta=1$, or of $\phi(A)=B$ when $\delta=-1$. If the preceding exponent is $-\delta$, this factor belongs to that preceding letter's pinch [subgroup](../../../../../subgroup.md). Multiplying an intervening coefficient outside that [subgroup](../../../../../subgroup.md) by an element inside it cannot put the product inside the [subgroup](../../../../../subgroup.md). Hence no cancellation occurs; when the two exponents agree, cancellation is impossible anyway. Thus a reduced word with $n\geq1$ has a normal form still containing $n$ [stable letters](../../../../../stable-letter.md), which cannot be the identity normal form. This is [Britton's lemma](../../../../../britton-s-lemma.md):

$$
\boxed{\text{a reduced sequence containing a stable letter is nonidentity}.}
$$

For the final example, write the centralizing extension as

$$
E=\langle a,b,t\mid t^{-1}w_jt w_j^{-1}=1\ (j\geq1)\rangle.
$$

It is generated by $a,b,t$. Suppose it were finitely presented. By the finite-generator independence already proved, the kernel of $F(a,b,t)\to E$ would be normally generated by finitely many words. Each of these kernel [group generators](../../../../../generator-of-a-group.md) is a finite product of conjugates of the displayed defining relators, so only finitely many indices occur in all their expressions. Choose $N$ at least as large as all of them. The full kernel would then equal the [normal closure](../../../../../normal-closure.md) of the first $N$ relators: one inclusion follows from those expressions, and the reverse inclusion follows because all these relators already belong to the kernel.

But the [group](../../../../../group-split.md) with only those first $N$ relators is the identity [HNN extension](../../../../../hnn-extension.md) over $H_N=\langle w_1,\ldots,w_N\rangle$. Since the $w_j$ are a free basis of $H$, $w_{N+1}\notin H_N$. The word $t^{-1}w_{N+1}t w_{N+1}^{-1}$ is reduced in this partial extension, so [Britton's lemma](../../../../../britton-s-lemma.md) makes it nonidentity there. It is identity in $E$, contradicting equality of the kernels. Therefore

$$
\boxed{E\text{ is finitely generated but not finitely presented}.}
$$

This is the free-basis instance of the general fact that [finite presentation of a centralizing HNN extension detects finite generation of its associated subgroup](../../../../../finite-presentation-of-a-centralizing-hnn-extension-detects-finite-generation-of-its-associated-subgroup.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
