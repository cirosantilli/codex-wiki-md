<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Write $R^iF$ for the cohomological indexing of the [right derived functor](../../../../../right-derived-functor.md). For the contravariant construction, assume $F$ is additive and left exact, so an exact sequence $M'\to M\to M''\to0$ gives $0\to F(M'')\to F(M)\to F(M')$. Module categories have enough [projective modules](../../../../../projective-module.md): a free module on a generating set surjects onto any module, and repeating the construction on its kernel produces a [projective resolution](../../../../../projective-resolution.md)

$$
\cdots\xrightarrow{d_2}P_1\xrightarrow{d_1}P_0\xrightarrow{\epsilon}M\longrightarrow0.
$$

Contravariance turns it into the [cochain complex](../../../../../cochain-complex.md)

$$
F(P_0)\xrightarrow{F(d_1)}F(P_1)\xrightarrow{F(d_2)}F(P_2)\longrightarrow\cdots,
\qquad
\boxed{R^iF(M)=H^i(F(P_\bullet)).}
$$

The composite of consecutive differentials is zero because $F$ is additive and reverses composition. Applying left exactness to $P_1\to P_0\to M\to0$ gives $F(M)=\ker(F(d_1))$, so $R^0F\simeq F$.

Here are the comparison and exactness arguments behind this construction. A map $M\to N$ lifts to a chain map between projective resolutions. In degree zero, lift through the surjection $Q_0\twoheadrightarrow N$ by projectivity of $P_0$. Inductively, the required composite from $P_i$ lands in the cycle module of the target resolution, which is the image of $Q_i$ by exactness, so projectivity supplies the next lift. Two such lifts are chain homotopic. Their difference in degree zero lands in $\ker(Q_0\to N)=\operatorname{im}d_1$, so it lifts to a homotopy map $P_0\to Q_1$. Subtracting the corresponding homotopy term in degree one gives another map into the next cycle module; continue inductively. Applying additive contravariant $F$ turns this chain homotopy into a cochain homotopy, so the maps on cohomology agree. Applying this to lifts of identity maps between two resolutions gives mutually inverse maps on cohomology. Thus the [contravariant right derived functor](../../../../../contravariant-right-derived-functor.md) is well-defined, contravariant and natural in $M$.

For $0\to M'\to M\to M''\to0$, construct compatible projective resolutions by the [horseshoe lemma](../../../../../horseshoe-lemma.md). Its construction is elementary: lift the projective cover of $M''$ into $M$ and add the projective cover of $M'$; their sum surjects onto $M$. The kernels fit into a new short exact sequence of the corresponding kernels, so repeat at each degree. This gives a degreewise split sequence

$$
0\longrightarrow P'_\bullet\longrightarrow P_\bullet\longrightarrow P''_\bullet\longrightarrow0.
$$

An additive contravariant functor takes split sequences to split sequences with their arrows reversed. The resulting short exact sequence of cochain complexes gives

$$
\begin{aligned}
0&\longrightarrow F(M'')\longrightarrow F(M)\longrightarrow F(M')
\longrightarrow R^1F(M'')\longrightarrow R^1F(M)\longrightarrow R^1F(M')\\
&\longrightarrow R^2F(M'')\longrightarrow\cdots.
\end{aligned}
$$

The connecting map is obtained by lifting a cocycle from the quotient complex, taking its differential, and viewing the result in the subcomplex; changing a lift changes the result by a coboundary. This construction proves both exactness and naturality of the [long exact sequence](../../../../../long-exact-sequence.md).

Positive derived functors vanish on projective modules, since such a module has a resolution concentrated in degree zero. For $0\to K\to P\to M\to0$ with $P$ projective, the preceding sequence gives $R^{i+1}F(M)\simeq R^iF(K)$ for $i\geq1$. This is dimension shifting. If $F$ is exact, all positive derived functors vanish because applying $F$ preserves exactness of the resolution. A natural transformation of additive left-exact contravariant functors induces natural transformations of their derived functors by applying it degreewise. These derived functors form the universal contravariant cohomological delta functor: successive projective surjections, on which the positive functors vanish, and the connecting maps determine any extension of a degree-zero natural transformation uniquely.

The displayed example in the PDF has a genuine variance mismatch. The functor $G(M)=\operatorname{Hom}_A(A/(a),M)$ is covariant in $M$, not contravariant. For a map $u:M\to N$, its induced map sends $h$ to $u\circ h$, in the same direction. We compute that displayed example with its correct variance, and then explain the contravariant variant.

For an additive covariant left-exact functor, use an [injective resolution](../../../../../injective-resolution.md) $0\to M\to I^0\to I^1\to\cdots$ instead of a projective resolution, and set $R^iG(M)=H^i(G(I^\bullet))$. Such resolutions exist for arbitrary modules. In fact $J=\operatorname{Hom}_{\mathbb Z}(A,D)$, with $(a\phi)(b)=\phi(ab)$, is injective: the adjunction

$$
\operatorname{Hom}_A(N,J)\simeq\operatorname{Hom}_{\mathbb Z}(N,D)
$$

sends a map to its value at $1$, and has inverse $\lambda\mapsto[n\mapsto(b\mapsto\lambda(bn))]$. Extension on the right was proved in Question 5, so it gives extension on the left. Products of injective modules are injective by extending every component separately. The map

$$
M\longrightarrow\prod_{\phi\in M^*}J,\qquad
m\longmapsto\bigl[b\longmapsto\phi(bm)\bigr]_\phi
$$

is $A$-linear and injective, because a nonzero $m$ is detected by some character at $b=1$. Applying the same embedding to successive cokernels produces the stated injective resolution. Its comparison and homotopy arguments are dual to the projective ones, and covariant derived functors have the long exact sequence in the original order of $M',M,M''$.

Let $B=A/(a)$. Evaluation at $1+(a)$ identifies

$$
G(M)=\operatorname{Hom}_A(B,M)=\{m\in M:am=0\},
$$

a naturally defined $B$-module. It is left exact: a compatible element in the kernel of $G(M)\to G(M'')$ is exactly an element of $M'$ killed by $a$.

Because $a$ is a non-zero-divisor on $A$, multiplication by $a$ is surjective on every injective module $I$. Indeed, for $m\in I$, the map $aA\to I$ given by $ax\mapsto xm$ is well-defined and $A$-linear. It extends to $A\to I$, and if the extension takes $1$ to $v$, then $av=m$. Thus for an injective resolution we have a short exact sequence of cochain complexes

$$
0\longrightarrow G(I^\bullet)\longrightarrow I^\bullet
\xrightarrow{\ a\ }I^\bullet\longrightarrow0.
$$

The cohomology of $I^\bullet$ is $M$ in degree zero and zero in higher degrees. Its long exact sequence therefore gives

$$
0\longrightarrow R^0G(M)\longrightarrow M\xrightarrow{\ a\ }M
\longrightarrow R^1G(M)\longrightarrow0,
\qquad R^iG(M)=0\ (i\geq2).
$$

Consequently the [Ext from a principal non-zero-divisor quotient](../../../../../ext-from-a-principal-non-zero-divisor-quotient.md) computation is

$$
\boxed{R^0G(M)=\ker(a:M\to M),\qquad
R^1G(M)=M/aM,\qquad R^iG(M)=0\quad(i\geq2).}
$$

All these groups are naturally $B$-modules. Equivalently they are $\operatorname{Ext}_A^i(B,M)$; the two-term free resolution $0\to A\xrightarrow{a}A\to B\to0$ gives the same kernel and cokernel after applying $\operatorname{Hom}_A(-,M)$.

If one instead wants a genuinely contravariant example, take $H(N)=\operatorname{Hom}_A(N,B)$. Then $R^iH(N)=\operatorname{Ext}_A^i(N,B)$, obtained by resolving the variable $N$. There is no claim of vanishing above degree one for arbitrary $N$. At $N=B$, the same two-term resolution has zero differential after applying $\operatorname{Hom}_A(-,B)$, and gives $\operatorname{Ext}_A^0(B,B)=B$, $\operatorname{Ext}_A^1(B,B)=B$, and zero higher groups. This keeps the printed covariant calculation distinct from the general contravariant construction.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
