<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Here the usual [homological algebra](../../../../../homological-algebra.md) convention is that the right-exact [functor](../../../../../functor.md) $F$ is additive. Module categories have enough [projective modules](../../../../../projective-module.md), because any [module](../../../../../module-mathematics.md) is a quotient of a [free module](../../../../../free-module.md). Choose a [projective resolution](../../../../../projective-resolution.md)

$$
\cdots\xrightarrow{d_3}P_2\xrightarrow{d_2}P_1\xrightarrow{d_1}P_0\longrightarrow M\longrightarrow0.
$$

Apply $F$ to the unaugmented [chain complex](../../../../../chain-complex.md) and define the [left derived functors](../../../../../left-derived-functor.md) by

$$
\boxed{L_iF(M)=H_i(F(P_\bullet))=\frac{\ker F(d_i)}{\operatorname{im}F(d_{i+1})}\quad(i>0),\qquad L_0F(M)=\operatorname{coker}F(d_1).}
$$

Additivity ensures that $F$ preserves zero maps, sums of maps and homotopy identities, so the transformed differentials still compose to zero.

For a [module homomorphism](../../../../../module-homomorphism.md) $u:M\to N$, lift it to a [chain map](../../../../../chain-map.md) between chosen [projective resolutions](../../../../../projective-resolution.md). In degree zero, lift through $Q_0\twoheadrightarrow N$ using projectivity of $P_0$. In each higher degree, the already constructed map lands in the next kernel; exactness of $Q_\bullet$ and projectivity of $P_i$ supply the next lift. Any two lifts are [chain homotopic](../../../../../chain-homotopy.md): their degree-zero difference lands in $\ker(Q_0\to N)=\operatorname{im}d_1^Q$, so it lifts to $h_0:P_0\to Q_1$. Inductively lift the remaining difference after subtracting the preceding homotopy term. This gives

$$
u_i-v_i=d_{i+1}^Qh_i+h_{i-1}d_i^P,\qquad h_{-1}=0.
$$

Applying $F$ preserves this identity, so the lifts induce the same [homology](../../../../../homology-split.md) map. Identity lifts and composable lifts show that $L_iF$ is a [functor](../../../../../functor.md). Comparison lifts between two resolutions over the identity of $M$ are inverse up to [chain homotopy](../../../../../chain-homotopy.md); hence the construction is independent of the chosen resolution up to its canonical natural [isomorphism](../../../../../isomorphism.md).

Right exactness identifies $L_0F(M)=\operatorname{coker}(F(P_1)\to F(P_0))$ naturally with $F(M)$. For a [projective module](../../../../../projective-module.md) $P$, the length-zero resolution gives $L_iF(P)=0$ for $i>0$. For a [short exact sequence](../../../../../short-exact-sequence.md) $0\to M'\to M\to M''\to0$, the [horseshoe lemma](../../../../../horseshoe-lemma.md) builds a degreewise split short exact sequence of [projective resolutions](../../../../../projective-resolution.md). Concretely, lift the projective generators covering $M''$ into $M$ and combine them with generators covering $M'$; repeat on the kernels. The middle projective term in each degree is the direct sum of the two outer ones. An [additive functor](../../../../../additive-functor.md) preserves these split sequences, and lifting cycles, taking their differentials and returning to the subcomplex produces the connecting maps in

$$
\cdots\to L_2F(M'')\to L_1F(M')\to L_1F(M)\to L_1F(M'')\to F(M')\to F(M)\to F(M'')\to0.
$$

This is the natural long exact derived-functor sequence. In particular, if $0\to K\to P\to M\to0$ has $P$ projective, then $L_iF(M)\cong L_{i-1}F(K)$ for $i\ge2$, and $L_1F(M)=\ker(F(K)\to F(P))$. These are dimension-shifting formulas. Positive degrees can be killed by the surjection $P\to M$. If $F$ is exact, it preserves every resolution's exactness and all its positive [left derived functors](../../../../../left-derived-functor.md) vanish. Conversely, if $L_1F$ vanishes on all modules, the displayed long exact sequence makes $F$ exact. A natural transformation between additive right-exact [functors](../../../../../functor.md) induces transformations on the [left derived functors](../../../../../left-derived-functor.md) by applying it termwise.

For [extension of scalars](../../../../../extension-of-scalars.md) $F(M)=B\otimes_AM$, these derived functors are the [Tor functors](../../../../../tor-functor.md) $\operatorname{Tor}_i^A(B,M)$. When $B=A/(a)$ and $a$ is a [non-zero-divisor](../../../../../non-zero-divisor.md), there is the length-one [free resolution](../../../../../free-resolution.md)

$$
0\longrightarrow A\xrightarrow{\ a\ }A\longrightarrow B\longrightarrow0.
$$

Although the construction above resolves $M$, one may instead use this resolution of $B$. To justify that calculation, tensor a free resolution of $M$ with the two-term resolution of $B$ to form a double complex. Taking homology first along the resolution of $B$ leaves $B\otimes_AP_\bullet$; taking it first along the resolution of $M$ leaves $M\xrightarrow{a}M$. The free terms preserve exactness under tensoring. The double complex is first-quadrant with finitely many terms on each total diagonal, so both filtrations compute the same total homology. This proves the required balancing directly.

The kernel and cokernel of multiplication by $a$ now give [Tor for a principal non-zero-divisor quotient](../../../../../tor-for-a-principal-non-zero-divisor-quotient.md):

$$
\boxed{L_0F(M)=M/aM,\qquad L_1F(M)=\{m\in M:am=0\},\qquad L_iF(M)=0\quad(i\ge2).}
$$

These are naturally $B$-modules. For $M=A$, the degree-one group is zero; for $M=B$, multiplication by $a$ is zero and both degrees zero and one are $B$. Thus, when $B\ne0$, degree one explicitly detects the failure of this base-change [functor](../../../../../functor.md) to be exact.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
