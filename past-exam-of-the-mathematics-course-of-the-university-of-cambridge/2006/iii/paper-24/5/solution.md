<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $L\dashv U:\mathcal D\to\mathcal C$, let $T=UL$ be the induced [monad](../../../../../monad.md). The [Eilenberg-Moore comparison functor](../../../../../eilenberg-moore-comparison-functor.md) is

$$
K:\mathcal D\longrightarrow\mathcal C^T,\qquad K(D)=(UD,U\varepsilon_D).
$$

The adjunction is a [monadic adjunction](../../../../../monadic-adjunction.md) if this functor is an [equivalence of categories](../../../../../equivalence-of-categories.md). To define [monadic length](../../../../../monadic-length.md), start with $K_0=U$ and form the comparison $K_1$ into the Eilenberg-Moore category of its induced monad. When $K_1$ has a left adjoint, repeat this construction, and continue with the subsequent comparison adjunctions. The length is the least number of comparison steps after which the comparison is an equivalence; an equivalence has length zero and a monadic non-equivalence has length one. The successive left adjoints will all be explicit in this example.

The [precise monadicity theorem](../../../../../beck-s-monadicity-theorem.md) states: a [functor](../../../../../functor.md) $U$ with a left adjoint is monadic if and only if it reflects isomorphisms and every parallel pair in $\mathcal D$ whose image admits a [split coequalizer](../../../../../split-coequalizer.md) in $\mathcal C$ has a coequalizer in $\mathcal D$ preserved by $U$. Here a split coequalizer of $f,g:B\rightrightarrows C$ consists of $q:C\to Q$, $s:Q\to C$ and $t:C\to B$ satisfying

$$
qf=qg,\qquad qs=1_Q,\qquad ft=1_C,\qquad gt=sq.
$$

These identities imply the coequalizer property and survive every functor. We shall identify the relevant algebra categories directly, which proves monadicity without having to check quotient constructions separately.

Write $U_m^{m+1}:\mathcal C_{m+1}\to\mathcal C_m$ for one step in the [nested partial unary operation category](../../../../../nested-partial-unary-operation-category.md) tower. For $m=0$, its left adjoint is

$$
F_0^1(A)=A\times\mathbb N,\qquad\omega_1(a,k)=(a,k+1),\qquad\eta_A(a)=(a,0).
$$

A function $f:A\to UB$ extends uniquely by $(a,k)\mapsto\omega_1^k f(a)$, proving the adjunction.

For $m\geq1$, take $A\in\mathcal C_m$ and let

$$
S_m(A)=\{a\in A:\omega_m(a)\text{ is defined and }\omega_m(a)=a\}.
$$

The [free extension of nested partial unary operations](../../../../../free-extension-of-nested-partial-unary-operations.md) has underlying set

$$
F_m^{m+1}A=A\sqcup\{b_{a,k}:a\in S_m(A),\ k\in\mathbb N\}.
$$

Keep the old operations on $A$. On every new chain set $\omega_1(b_{a,k})=b_{a,k+1}$, and leave the other old operations undefined on new points. Define the new operation by $\omega_{m+1}(a)=b_{a,0}$ for $a\in S_m(A)$, and nowhere else. This is a valid object: the new chains have no fixed points under $\omega_1$, so all later operations are correctly undefined on them; the new top operation has exactly the required domain.

If $f:A\to U_m^{m+1}B$ preserves the old operations, it carries $S_m(A)$ into $S_m(B)$. Its unique extension is

$$
b_{a,k}\longmapsto\omega_1^k\bigl(\omega_{m+1}(f(a))\bigr).
$$

The formula preserves the first operation along each chain, the new operation at its old fixed-point source, and all the other defined operations. Conversely these requirements force the formula. This proves the one-step [adjunction](../../../../../adjoint-functors.md) in every case.

Let $T_m=U_m^{m+1}F_m^{m+1}$. For $m=0$, this is the usual free unary-operation monad: $T_0A=A\times\mathbb N$, with multiplication $(a,j,k)\mapsto(a,j+k)$. An algebra action $h:A\times\mathbb N\to A$ obeys $h(a,0)=a$ and $h(h(a,j),k)=h(a,j+k)$. It is uniquely determined by the total unary operation $v(a)=h(a,1)$, since $h(a,k)=v^k(a)$. Algebra morphisms are exactly functions commuting with $v$. Thus $\mathcal C_0^{T_0}\cong\mathcal C_1$.

For $m\geq1$, no new chain point belongs to $S_m(T_mA)$, so $S_m(T_mA)=S_m(A)$. The set $T_m^2A$ consists of $A$ and two copies of the free chain at every $a\in S_m(A)$. Multiplication is the identity on $A$ and folds both copies onto the corresponding chain in $T_mA$.

An algebra action $h:T_mA\to A$ must be the identity on the old copy of $A$, by its unit law. Preservation of $\omega_1$ forces

$$
h(b_{a,k})=\omega_1^k v(a),\qquad v(a)=h(b_{a,0}).
$$

The choices $v(a)\in A$, for $a\in S_m(A)$, are otherwise arbitrary. There are no higher old operations to preserve on new points. Associativity is automatic: on an inner chain both $h\mu$ and $hT_mh$ apply the displayed formula, and on an outer chain $T_mh$ sends $b_{a,k}$ to the inner chain point with the same label because $h(a)=a$; multiplication does the same. Therefore $h\mu=hT_mh$ on every point.

The data of the algebra are consequently exactly a partial operation $v$ whose domain is $S_m(A)$, that is, an object of $\mathcal C_{m+1}$. For a map $f:A\to B$ in $\mathcal C_m$, the algebra-morphism equation $fh=h'T_mf$ at $b_{a,0}$ says precisely $f(v(a))=v'(f(a))$; equality on the rest of the chain then follows from preservation of $\omega_1$. Thus we have identified objects and morphisms, not just their underlying sets:

$$
\boxed{\mathcal C_m^{T_m}\cong\mathcal C_{m+1}.}
$$

Under this isomorphism the comparison functor for $F_m^{m+1}\dashv U_m^{m+1}$ is the identity identification. Hence **every one-step forgetful adjunction is monadic**.

Now take $n>m$. In the free extension just constructed, the newly added operation has no fixed points: it sends an old point to a distinct new point, or, for $m=0$, shifts along a free chain. Therefore all further operations can only be undefined. Adding them freely adds no more points. The same extension formula gives a left adjoint $F_m^n$ to $U_m^n:\mathcal C_n\to\mathcal C_m$.

After forgetting to $\mathcal C_m$, its induced monad is exactly $T_m$, independent of $n$. This includes the unit and multiplication: the unit is the old-point inclusion, and the counit formula gives the same addition of chain indices for $m=0$ or the same folding of the two chain copies for $m\geq1$. Its comparison functor, after the identification $\mathcal C_m^{T_m}\cong\mathcal C_{m+1}$, is exactly

$$
U_{m+1}^n:\mathcal C_n\longrightarrow\mathcal C_{m+1}.
$$

Indeed, the comparison action on the first point of each free chain recovers $\omega_{m+1}$, while the higher operations are forgotten. Thus each comparison step recovers exactly one additional operation. After $n$ steps from sets, the comparison is the identity of $\mathcal C_n$.

No earlier step is an equivalence. For $0\leq m<n$, put all of the first $m$ operations equal to the identity on a three-element set. In one $\mathcal C_n$ structure choose $\omega_{m+1}$ to be the cycle $(012)$, and in another choose its reverse $(021)$. Both have no fixed points at this stage, so every higher operation is undefined. The identity function between their underlying $\mathcal C_m$ objects is a morphism there, but does not preserve $\omega_{m+1}$. Hence $U_m^n$ is not full, and cannot be an equivalence. This also applies for $m=0$, when there are no old operations. We conclude

$$
\boxed{\text{the adjunction between }\mathcal C_n\text{ and }\mathbf{Set}\text{ has monadic length }n.}
$$

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 24](../../paper-24-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
