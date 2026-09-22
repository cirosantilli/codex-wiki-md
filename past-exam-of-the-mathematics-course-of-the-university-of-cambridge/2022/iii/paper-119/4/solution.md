<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [monad](../../../../../monad.md) on a category $\mathcal C$ consists of an endofunctor $T$, a unit $\eta:1_{\mathcal C}\Rightarrow T$, and a multiplication $\mu:T^2\Rightarrow T$ satisfying

$$
\mu\,T\eta=1_T=\mu\,\eta T,
\qquad
\mu\,T\mu=\mu\,\mu T.
$$

If $F:\mathcal C\rightleftarrows\mathcal D:G$ is an [adjunction](../../../../../adjoint-functors.md) with unit $\eta$ and counit $\varepsilon$, then

$$
T=GF,qquad \mu=G\varepsilon F
$$

defines the [monad induced by an adjunction](../../../../../monad-induced-by-an-adjunction.md). The two triangle identities give the unit laws, while naturality of $\varepsilon$ gives associativity.

Let $\mathcal D$ now be a full subcategory of $[\mathcal C,\mathcal C]$ that contains the identity endofunctor and is closed under composition, and suppose $T$ is terminal in $\mathcal D$. There is exactly one natural transformation

$$
\eta:1_{\mathcal C}\Rightarrow T
$$

and exactly one

$$
\mu:T^2\Rightarrow T.
$$

Both sides of either unit law are endomorphisms of the terminal object $T$, so they equal $1_T$; both sides of associativity are maps $T^3\to T$, so they are equal as well. This gives a monad, and terminality also makes both structure maps unique. This is the [monad structure on a terminal endofunctor](../../../../../monad-structure-on-a-terminal-endofunctor.md).

For a set $A$, let $\mathcal U(A)$ be the set of [ultrafilters](../../../../../ultrafilter.md) on $A$. A function $f:A\to A'$ induces the pushforward

$$
\mathcal U(f)(U)=\{B\subseteq A':f^{-1}(B)\in U\},
$$

which makes $\mathcal U$ the [ultrafilter functor](../../../../../ultrafilter-functor.md). There is no ultrafilter on the empty set. Moreover, every ultrafilter on $A\sqcup B$ contains exactly one of the complementary summands $A$ and $B$, and restriction gives a unique ultrafilter on that summand. Therefore

$$
\mathcal U(\varnothing)=\varnothing,
\qquad
\mathcal U(A\sqcup B)\cong\mathcal U(A)\sqcup\mathcal U(B),
$$

so $\mathcal U$ preserves finite coproducts.

Let $F:\mathbf{Set}\to\mathbf{Set}$ preserve finite coproducts. For $x\in F(A)$ define

$$
\Phi_A(x)=\{B\subseteq A:x\in\operatorname{im}(F(B)\to F(A))\}.
$$

The decomposition $A=B\sqcup(A\setminus B)$ and preservation of coproducts say that $x$ lies in exactly one of the two corresponding images. Thus exactly one of $B$ and its complement belongs to $\Phi_A(x)$. Upward closure follows by factoring subset inclusions. If $B,C\in\Phi_A(x)$, decompose $A$ into the four disjoint Boolean cells determined by $B$ and $C$. The unique cell containing $x$ must lie inside both sets, so $B\cap C\in\Phi_A(x)$. Hence $\Phi_A(x)$ is an ultrafilter.

For $f:A\to A'$, the decompositions

$$
A=f^{-1}(B)\sqcup f^{-1}(A'\setminus B),
\qquad
A'=B\sqcup(A'\setminus B)
$$

show that

$$
B\in\Phi_{A'}(Ff(x))
\quad\Longleftrightarrow\quad
f^{-1}(B)\in\Phi_A(x).
$$

Thus $\Phi:F\Rightarrow\mathcal U$ is natural.

It is the only such natural transformation. For $B\subseteq A$, let $\chi_B:A\to\{0,1\}$ be its characteristic function. Since

$$
F(\{0,1\})\cong F(1)\sqcup F(1)
$$

and the two ultrafilters on $\{0,1\}$ are the principal ones, naturality with the two singleton inclusions forces any transformation $F\Rightarrow\mathcal U$ to send each summand to the corresponding principal ultrafilter. Naturality with $\chi_B$ then says that $B$ belongs to the image ultrafilter exactly when $x$ lies in the image of $F(B)\to F(A)$. Hence the transformation must be $\Phi$.

The ultrafilter functor is therefore the [terminal finite-coproduct-preserving set endofunctor](../../../../../terminal-finite-coproduct-preserving-set-endofunctor.md). The preceding terminal-object argument supplies its unique [ultrafilter monad](../../../../../ultrafilter-monad.md) structure.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 119](../../paper-119-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
