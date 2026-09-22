<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $K$ be a field, $K_s$ a separable closure and $G_K$ its [absolute Galois group](../../../../../../absolute-galois-group.md). A discrete [Galois module](../../../../../../galois-module.md) $A$ is an abelian group with a continuous $G_K$-action, so each element has an open stabilizer. [Galois cohomology](../../../../../../galois-cohomology.md) uses continuous cochains. Its zeroth group is $H^0(K,A)=A^{G_K}$, and its first group is

$$
H^1(K,A)=Z^1(K,A)/B^1(K,A),
$$

where

$$
c_{\sigma\tau}=c_\sigma+\sigma c_\tau,
\qquad
B^1(K,A)=\{c_\sigma=\sigma a-a:a\in A\}.
$$

Thus cocycles measure a failure of descent, and coboundaries account for changing a chosen lift. A short exact sequence of [Galois modules](../../../../../../galois-module.md) gives a [long exact sequence in group cohomology](../../../../../../long-exact-sequence-in-group-cohomology.md). Its connecting map sends an invariant element of a quotient to the cocycle $\sigma b-b$ of a chosen lift $b$; changing the lift changes this by a coboundary. These constructions provide the bridge between arithmetic divisibility and cohomology.

For [Kummer theory](../../../../../../kummer-theory.md), assume the characteristic does not divide $n$. The multiplicative exact sequence is

$$
1\longrightarrow\mu_n\longrightarrow K_s^\times
\xrightarrow{,n,}K_s^\times\longrightarrow1.
$$

The final arrow is surjective because a root of $T^n-a$ is separable for $a\ne0$. [Hilbert's theorem 90](../../../../../../hilbert-s-theorem-90.md) says $H^1(K,K_s^\times)=0$. Here is its usual finite-extension proof. For a multiplicative cocycle $c_\sigma$ on a finite [Galois extension](../../../../../../finite-galois-extension.md) $L/K$, choose $a\in L$ so that

$$
A=\sum_{\sigma\in\operatorname{Gal}(L/K)}c_\sigma\sigma(a)\ne0.
$$

Such an $a$ exists by the [Artin independence theorem](../../../../../../linear-independence-of-distinct-field-embeddings.md). The cocycle identity gives $\tau A=c_\tau^{-1}A$. With $b=A^{-1}$ this becomes $c_\tau=\tau b/b$, a coboundary. Every continuous cocycle with values in $K_s^\times$ is defined over a sufficiently large finite Galois extension, so the same result holds for the absolute group.

The [long exact sequence in group cohomology](../../../../../../long-exact-sequence-in-group-cohomology.md) now gives

$$
\boxed{H^1(K,\mu_n)\cong K^\times/(K^\times)^n.}
$$

The class of $a$ maps to $c_\sigma=\sigma(\alpha)/\alpha$, where $\alpha^n=a$. This cohomological statement does not require $\mu_n\subset K$; it retains the actual Galois action on $\mu_n$. If all $n$th roots of unity do lie in $K$, the action is trivial, and after choosing a primitive root of unity the cocycles are characters into $\mathbb Z/n\mathbb Z$. Thus adjoining an $n$th root of $a$ describes a cyclic extension of degree dividing $n$, and Kummer classes classify the corresponding characters. For $n=2$, this gives the familiar quadratic extensions and the [square-class group of a field](../../../../../../square-class-group-of-a-field.md).

Now let $K$ be a [number field](../../../../../../number-field.md) and $E/K$ an [elliptic curve](../../../../../../elliptic-curve.md). The [multiplication-by-n morphism](../../../../../../multiplication-by-n-morphism.md) is a surjective isogeny on $E(\overline K)$, with kernel $E[n]\cong(\mathbb Z/n\mathbb Z)^2$. The [Kummer exact sequence of an elliptic curve](../../../../../../kummer-exact-sequence-of-an-elliptic-curve.md)

$$
0\longrightarrow E[n]\longrightarrow E(\overline K)
\xrightarrow{[n]}E(\overline K)\longrightarrow0
$$

yields

$$
0\longrightarrow E(K)/nE(K)\xrightarrow{\delta}
H^1(K,E[n])\longrightarrow H^1(K,E)[n]\longrightarrow0.
$$

Explicitly, choose $Q$ with $nQ=P$ and set $\delta(P)_\sigma=\sigma Q-Q$. This lies in $E[n]$, satisfies the cocycle identity and is unchanged as a class if $Q$ is replaced by another division point. If it is a coboundary $\sigma T-T$ for $T\in E[n]$, then $Q-T$ is rational over $K$ and $P=n(Q-T)$. Conversely such a rational division point makes the cocycle zero. This proves the injectivity of the [Kummer map of an elliptic curve](../../../../../../kummer-map-of-an-elliptic-curve.md) on $E(K)/nE(K)$.

To prove the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md), it remains to prove that this particular cohomological image is finite. The full group $H^1(K,E[n])$ need not be finite, so the injection alone is not enough. Choose a finite set $S$ of finite places containing the bad-reduction places and those dividing $n$. At any other place, the construction in Question 3 works over the local field: reduce $P$, find an $n$-division point over a finite residue extension, lift it by the [Hensel lemma](../../../../../../hensel-s-lemma.md), and correct its error by the inverse formal multiplication. Thus $P$ has an $n$-division point over the [maximal unramified extension](../../../../../../maximal-unramified-extension.md). Choosing that lift locally makes the cocycle zero on inertia. For an arbitrary lift its restriction is a coboundary, so the cohomology class is unramified. Therefore the image lies in [first Galois cohomology unramified outside a finite set](../../../../../../first-galois-cohomology-unramified-outside-a-finite-set.md):

$$
\delta(E(K)/nE(K))\subseteq H^1_S(K,E[n]).
$$

We prove the required finiteness of this group. Take a finite Galois extension $L/K$ containing all of $E[n]$ and $\mu_n$, and enlarge $S$ to include any remaining ramification of $L/K$. Let $S_L$ be the places above it. The [inflation-restriction exact sequence](../../../../../../inflation-restriction-exact-sequence.md) bounds the kernel of restriction to $L$ by

$$
H^1(\operatorname{Gal}(L/K),E[n]),
$$

a finite group, since both its group of arguments and its group of values are finite. Over $L$ the torsion module is constant and can be identified with $\mu_n^2$, so [Kummer theory](../../../../../../kummer-theory.md) gives

$$
H^1(L,E[n])\cong\bigl(L^\times/(L^\times)^n\bigr)^2.
$$

Restrictions of our unramified classes remain unramified outside $S_L$. If a Kummer class $[a]$ is unramified at such a place $v$, its $n$th root can be taken in an unramified local extension. The extended valuation still has integer values, and $n\,v(\sqrt[n]a)=v(a)$. Hence $v(a)$ is divisible by $n$. Each coordinate therefore lies in the [S-unramified power class group](../../../../../../s-unramified-power-class-group.md)

$$
L(S_L,n)=\{[a]\in L^\times/(L^\times)^n:
 v(a)\equiv0\pmod n\text{ for }v\notin S_L\}.
$$

This group is finite. Indeed, the ideal of $a$ away from $S_L$ is $\mathfrak a^n$. Sending $[a]$ to $[\mathfrak a]$ yields the exact sequence

$$
0\longrightarrow\mathcal O_{L,S_L}^{\times}/(\mathcal O_{L,S_L}^{\times})^n
\longrightarrow L(S_L,n)
\longrightarrow\operatorname{Cl}(\mathcal O_{L,S_L})[n]\longrightarrow0.
$$

For its kernel, a principal $\mathfrak a$ lets us divide $a$ by an $n$th power to obtain an $S_L$-unit. For surjectivity, an ideal class killed by $n$ has an $n$th power which is principal away from $S_L$, giving such an $a$. The [S-unit group](../../../../../../s-unit-group.md) is finitely generated and the [ideal class group](../../../../../../ideal-class-group.md) is finite; hence both end groups are finite, proving [finiteness of S-unramified Kummer classes](../../../../../../finiteness-of-s-unramified-kummer-classes.md). Restriction has finite image in $L(S_L,n)^2$ and finite kernel, so $H^1_S(K,E[n])$ is finite. We conclude

$$
\boxed{\#\bigl(E(K)/nE(K)\bigr)<\infty\qquad(n\ge2),}
$$

which is the [Weak Mordell-Weil theorem](../../../../../../weak-mordell-weil-theorem.md) and its [Kummer-theoretic proof of the weak Mordell-Weil theorem](../../../../../../kummer-theoretic-proof-of-the-weak-mordell-weil-theorem.md).

This framework also defines the [Selmer group of an elliptic curve](../../../../../../n-selmer-group.md) by imposing that a class in $H^1(K,E[n])$ lie in the local Kummer image at every completion. Its classes are unramified outside a fixed finite set, so the same finiteness proof applies. Its relation to rational points is

$$
0\longrightarrow E(K)/nE(K)\longrightarrow
\operatorname{Sel}^{(n)}(E/K)\longrightarrow
\operatorname{Sha}(E/K)[n]\longrightarrow0.
$$

The [Tate–Shafarevich group](../../../../../../tate-shafarevich-group.md) here measures the difference between locally soluble torsors and globally soluble ones. Finally, the weak theorem gives finite divisibility quotients; adding the [height descent lemma](../../../../../../height-descent-lemma.md) and bounded-height finiteness proves the stronger [Mordell-Weil theorem](../../../../../../mordell-weil-group.md). Those height inputs are additional to the cohomological finiteness just established.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
