<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $k=\mathbb F_p$. The [Nottingham group](../../../../../nottingham-group.md) $\mathcal N$ is the set of formal series $f(t)=t+\sum_{i\ge2}a_it^i$ over $k$, with ordinary composition $f\circ g$ as multiplication and the $t$-adic [topology](../../../../../topology-split.md). The identity is $t$. A compositional inverse exists uniquely by solving its coefficients successively, since the linear coefficient is $1$.

Equivalently $\mathcal N$ is the [group](../../../../../group-split.md) of continuous $k$-automorphisms of $k((t))$ whose action on $(t)/(t^2)$ is the identity. Such an automorphism is determined by the image of $t$, which is $t+O(t^2)$. To identify this with ordinary series composition without reversing multiplication, send $f$ to the automorphism $h(t)\mapsto h(f^{-1}(t))$. Its composite with the automorphism for $g$ is the one for $f\circ g$.

The depth filtration is

$$
\mathcal N_m=\{f:f(t)\equiv t\pmod{t^{m+1}}\},\qquad m\ge1.
$$

Each $\mathcal N_m$ is open and normal, and the coefficient of $t^{m+1}$ identifies $\mathcal N_m/\mathcal N_{m+1}$ with $(k,+)$. Thus $[\mathcal N:\mathcal N_m]=p^{m-1}$, and $\mathcal N$ is the [inverse limit](../../../../../inverse-limit.md) of its [finite p-group](../../../../../finite-p-group.md) truncations.

Here is a local-field proof that **every [finite p-group](../../../../../finite-p-group.md) embeds in $\mathcal N$**. We first establish the realization step rather than assume the Nottingham embedding itself. Put $F=k((t))$ and $\Gamma=\operatorname{Gal}(F^{\mathrm{sep}}/F)$, and let $I\trianglelefteq\Gamma$ be the inertia [subgroup](../../../../../subgroup.md), the [group homomorphism kernel](../../../../../kernel-of-a-group-homomorphism.md) of the action on the [algebraic closure](../../../../../algebraic-closure.md) of the [residue field](../../../../../residue-field.md). We use the standard additive [normal basis theorem](../../../../../normal-basis-theorem.md) consequence $H^j(\Gamma,F^{\mathrm{sep}})=0$ for $j>0$. It follows by taking direct limits of the finite-Galois normal-basis [modules](../../../../../module-mathematics.md), whose additive [cohomology](../../../../../cohomology-split.md) vanishes. The Artin-Schreier sequence

$$
0\longrightarrow\mathbb F_p\longrightarrow F^{\mathrm{sep}}\xrightarrow{z\mapsto z^p-z}F^{\mathrm{sep}}\longrightarrow0
$$

then gives

$$
H^1(\Gamma,\mathbb F_p)=F/\{z^p-z:z\in F\},\qquad H^2(\Gamma,\mathbb F_p)=0.
$$

The classes $t^{-m}$ for positive $m$ prime to $p$ are [linearly independent](../../../../../linear-independence.md): a nonzero finite linear combination has a most negative [valuation](../../../../../valuation.md) prime to $p$, whereas a negative [valuation](../../../../../valuation.md) of $z^p-z$ is divisible by $p$. Thus there are infinitely many independent continuous characters $\Gamma\to C_p$.

Induct on the order of a [finite p-group](../../../../../finite-p-group.md) $E$. Choose a central [subgroup](../../../../../subgroup.md) $C\cong C_p$ and put $Q=E/C$. By induction there is an onto map $\phi:\Gamma\to Q$ with $\phi(I)=Q$, corresponding to a [totally ramified](../../../../../totally-ramified-extension.md) $Q$-extension. The central extension $1\to C\to E\to Q\to1$ is specified by a [two-cocycle](../../../../../two-cocycle.md). Its pullback along $\phi$ is a [coboundary](../../../../../coboundary.md) because $H^2(\Gamma,\mathbb F_p)=0$. Correcting a set-theoretic section by that [coboundary](../../../../../coboundary.md) gives a continuous [homomorphism](../../../../../homomorphism.md) $\rho_0:\Gamma\to E$ lifting $\phi$.

We must make the lift onto on inertia, not merely onto on the whole [Galois group](../../../../../galois-group.md). Let $A=I\cap\ker\phi$. On $A$, the lift $\rho_0$ takes values in $C$. Characters vanishing on $A$ form a finite-dimensional space: $\Gamma/A$ has a finite [subgroup](../../../../../subgroup.md) $I/A\cong Q$ and procyclic quotient $\Gamma/I\cong\widehat{\mathbb Z}$, so a character is determined by finitely many values on generators of these two pieces. The infinite-dimensional character space therefore has infinitely many distinct restrictions to $A$. Choose a character $\chi:\Gamma\to C$ whose restriction to $A$ does not cancel $\rho_0|_A$, and set $\rho(\gamma)=\chi(\gamma)\rho_0(\gamma)$. Centrality of $C$ makes this another [homomorphism](../../../../../homomorphism.md) lifting $\phi$. Its image on $A$ is nontrivial and hence all of $C$, while its image on $I$ maps onto $Q$. Therefore $\rho(I)=E$. The fixed [field](../../../../../field.md) of $\ker\rho$ is the required [totally ramified](../../../../../totally-ramified-extension.md) finite [Galois extension](../../../../../finite-galois-extension.md) $K/F$ with [group](../../../../../group-split.md) $E$. This proves the realization step for every [finite p-group](../../../../../finite-p-group.md).

Since the [residue field](../../../../../residue-field.md) of $K$ is still $k$, choosing a [uniformizer](../../../../../uniformizer.md) $u$ identifies $K$ with $k((u))$. Indeed successive subtraction of its residue coefficient and division by $u$ gives each element of its [valuation ring](../../../../../valuation-ring.md) a unique convergent expansion $\sum_{i\ge0}b_iu^i$ with $b_i\in k$, and fractions give the Laurent expansions. Each element of $E$ preserves the [valuation](../../../../../valuation.md) and fixes $k$, so sends $u$ to $a_1u+a_2u^2+\cdots$. The linear coefficient is a [homomorphism](../../../../../homomorphism.md) $E\to k^\times$. Since $E$ is a $p$-group and $|k^\times|=p-1$, that [homomorphism](../../../../../homomorphism.md) is trivial. Thus the faithful Galois action lies in $\mathcal N(k)$, completing the embedding proof.

An infinite [profinite group](../../../../../profinite-group.md) is [hereditarily just infinite](../../../../../hereditarily-just-infinite-profinite-group.md) when every [open subgroup](../../../../../open-subgroup.md) is infinite and every nontrivial closed [normal subgroup](../../../../../normal-subgroup.md) of each such [open subgroup](../../../../../open-subgroup.md) is open. We sketch the normal-subgroup argument, giving the depth calculation in odd characteristic explicitly. For series of depths $r,s$,

$$
f=t+at^{r+1}+\cdots,\quad g=t+bt^{s+1}+\cdots\quad\Longrightarrow\quad[f,g]=t+ab(r-s)t^{r+s+1}+O(t^{r+s+2}),
$$

where $[f,g]=f^{-1}\circ g^{-1}\circ f\circ g$. The coefficient follows by comparing $f\circ g$ and $g\circ f$ in degree $r+s+1$: their cross terms are $ab(r+1)$ and $ab(s+1)$.

Let $H$ be open and $1\ne K\trianglelefteq H$ closed. Choose $m$ with $\mathcal N_m\le H$ and choose $f\in K$ of depth $r$. For every $j\ge m$ with $j\not\equiv r\pmod p$, commutation with $t+bt^{j+1}$ supplies an element of $K$ of depth $r+j$, with any prescribed nonzero [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) by varying $b$. Thus every sufficiently high layer except possibly depths congruent to $2r$ modulo $p$ occurs in $K$.

When $p$ is odd, choose one available depth $u\ge r+m$ with $u\not\equiv2r,r\pmod p$. Such a residue exists even for $p=3$. An element $h\in K$ of that depth can be commuted with $t+bt^{k-u+1}$ for every sufficiently large missing depth $k\equiv2r\pmod p$. The new [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) contains $2u-k\equiv2(u-r)\ne0$, so those missing layers occur too. Hence $K$ contains an element with any chosen coefficient in every depth $k\ge M$, for some $M$.

Successive coefficient correction now proves $\mathcal N_M\le K$: match the coefficient of an arbitrary target in depth $M$ by an element of $K$, correct the error in depth $M+1$, and continue. The partial products converge $t$-adically to the target and remain in $K$, which is closed. Thus $K$ is open. This proves hereditary just infiniteness for odd $p$.

For characteristic two, the [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) alone misses even depths. The standard characteristic-two normal-closure collection lemma supplies the needed extra input: for every $m\ge1$ and every nonidentity $f\in\mathcal N(\mathbb F_2)$, the [closed subgroup](../../../../../closed-subgroup.md) generated by the conjugates $f^g$ with $g\in\mathcal N_m$ contains $\mathcal N_M$ for some $M$. Its proof retains the next coefficients in pairs of [group commutators](../../../../../group-commutator.md) to fill the parity gaps, then uses the same successive coefficient correction. Apply this lemma to $f\in K$ and $\mathcal N_m\le H$: every such conjugate lies in $K$, so $K$ contains the tail and is open. This states the additional collection result used in the characteristic-two sketch; the odd-prime leading-term argument is not being applied there. Since every [open subgroup](../../../../../open-subgroup.md) contains a tail and is infinite, **the [Nottingham group](../../../../../nottingham-group.md) is [hereditarily just infinite](../../../../../hereditarily-just-infinite-profinite-group.md) for every prime $p$**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 5](../../paper-5-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
