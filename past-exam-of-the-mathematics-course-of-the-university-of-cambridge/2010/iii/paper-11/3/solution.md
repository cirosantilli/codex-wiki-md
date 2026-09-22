<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The printed statement needs **$A\ne\varnothing$**: for the empty set every linear subspace has cardinality at least one, so the requested bound is impossible. We prove the intended nonempty version of the [Freiman-Ruzsa theorem over a finite field](../../../../../freiman-ruzsa-theorem-over-a-finite-field.md). Necessarily $C\ge1$, because any one translate of $A$ inside $A+A$ has size $|A|$.

We first prove all [sumset](../../../../../sumset.md) estimates needed below. For finite nonempty $X$ and finite $U,V$ in an [abelian group](../../../../../abelian-group.md), choose one representation $z=u_z-v_z$ for each $z\in U-V$. The map

$$
(U-V)\times X\longrightarrow(U+X)\times(V+X),\qquad
(z,x)\longmapsto(u_z+x,v_z+x)
$$

is injective: subtracting the outputs recovers $z$, hence its chosen representation and then $x$. This proves the [Ruzsa triangle inequality](../../../../../ruzsa-triangle-inequality.md)

$$
|U-V|\le\frac{|U+X||V+X|}{|X|}.
$$

Choose nonempty $X\subseteq B$ minimizing $c'=|X+B|/|X|\le C$, where $B$ is any set with $|B+B|\le C|B|$. We prove the [Petridis minimal-growth lemma](../../../../../petridis-minimal-growth-lemma.md) $|X+B+D|\le c'|X+D|$ for every finite $D$. List $D=\{d_1,\ldots,d_s\}$, and let $X_i$ consist of those $x\in X$ for which $x+d_i$ was not already in $X+\{d_1,\ldots,d_{i-1}\}$. The disjoint pieces $X_i+d_i$ partition $X+D$.

Every $(X\setminus X_i)+B+d_i$ was already covered in $X+B+\{d_1,\ldots,d_{i-1}\}$. The new part at step $i$ therefore has size at most

$$
|X+B|-|(X\setminus X_i)+B|
\le c'|X|-c'|X\setminus X_i|=c'|X_i|.
$$

Here minimality of $X$ applies to every nonempty subset $X\setminus X_i$, and the empty case has size zero. Summing proves the lemma. Iteration gives $|X+kB|\le C^k|X|$. Apply the [Ruzsa triangle inequality](../../../../../ruzsa-triangle-inequality.md) with $U=kB$, $V=\ell B$ to obtain

$$
|kB-\ell B|\le C^{k+\ell}|X|\le C^{k+\ell}|B|.
$$

This derives the required [Plünnecke-Ruzsa inequality](../../../../../plunnecke-ruzsa-inequality.md). In [characteristic two](../../../../../characteristic-two.md), subtraction is addition, so $|rB|\le C^r|B|$ for every positive integer $r$.

Fix $a\in A$ and translate to $B=A+a$, which contains zero, has size $|A|$, and has the same [doubling constant](../../../../../doubling-constant.md). Choose $m=\lceil\log_2(2|12B|)\rceil$. A uniformly random [linear map](../../../../../linear-map.md) $L:\mathbb F_2^N\to G'=\mathbb F_2^m$ kills each specified nonzero vector with probability $2^{-m}$. The [union bound](../../../../../boole-s-inequality.md) shows that some $L$ satisfies

$$
\ker L\cap12B=\{0\},\qquad |G'|=2^m<4|12B|\le4C^{12}|B|.
$$

Because $0\in B$, all lower [iterated sumsets](../../../../../iterated-sumset.md) lie in $12B$. In particular $L$ is injective on $B$, since the difference of two elements belongs to $2B$. For $B'=L(B)$, the density $\alpha=|B'|/|G'|$ is at least $1/(4C^{12})$. This proves [injective linear modelling of a small sumset](../../../../../injective-linear-modelling-of-a-small-sumset.md).

We next prove the [Finite-field Bogolyubov lemma](../../../../../finite-field-bogolyubov-lemma.md) in this model. Write $f=1_{B'}$ and use normalized real [Fourier coefficients on a finite abelian group](../../../../../fourier-coefficient-on-a-finite-abelian-group.md) $\widehat f(\xi)=\mathbb E_xf(x)(-1)^{\xi\cdot x}$. Let

$$
S=\{\xi:|\widehat f(\xi)|\ge\alpha^{3/2}/\sqrt2\},\qquad
W=\{w:\xi\cdot w=0\text{ for every }\xi\in S\}.
$$

By [Parseval identity](../../../../../parseval-identity.md), $|S|\le2\alpha^{-2}$. Thus $W$ is a [vector subspace](../../../../../vector-subspace.md) of codimension at most $D=\lceil32C^{24}\rceil$.

For $w\in W$, [Fourier inversion](../../../../../fourier-inversion-theorem.md) of the fourfold normalized [convolution](../../../../../convolution.md) gives

$$
f*f*f*f(w)=\sum_{\xi}\widehat f(\xi)^4(-1)^{\xi\cdot w}.
$$

All terms with $\xi\in S$ are nonnegative, and the zero-frequency term is $\alpha^4$. The absolute contribution from the remaining frequencies is at most

$$
\sum_{\xi\notin S}|\widehat f(\xi)|^4
\le\frac{\alpha^3}{2}\sum_\xi|\widehat f(\xi)|^2
=\frac{\alpha^4}{2}.
$$

Hence the convolution is positive and $W\subseteq4B'$. Also $|W|\ge2^{-D}|G'|\ge2^{-D}|B|$.

For each $w\in W$, choose its lift $\sigma(w)\in4B$. It is unique because two lifts differ by an element of $8B\cap\ker L$, which is zero. For $w_1,w_2\in W$, the discrepancy

$$
\sigma(w_1)+\sigma(w_2)+\sigma(w_1+w_2)
$$

belongs to $12B\cap\ker L$, so it vanishes. Also $\sigma(0)=0$. Therefore $\sigma$ is a [linear map](../../../../../linear-map.md) and its image $\widetilde W\subseteq4B$ is a [vector subspace](../../../../../vector-subspace.md) with $|\widetilde W|=|W|\ge2^{-D}|B|$. This establishes [lifting a subspace through a Freiman model](../../../../../lifting-a-subspace-through-a-freiman-model.md) without assuming that arbitrary choices of preimages preserve addition.

Finally, $B+\widetilde W\subseteq5B$ is a union of $\widetilde W$-[cosets](../../../../../coset.md). The number of these cosets is at most

$$
t=\frac{|B+\widetilde W|}{|\widetilde W|}\le C^5 2^D.
$$

Choose representatives $b_1,\ldots,b_t$ from $B$. Then $B\subseteq\widetilde W+\{b_1,\ldots,b_t\}$, so adjoining these representatives and $a$ to $\widetilde W$ gives a [vector subspace](../../../../../vector-subspace.md) $V$ containing $A$. Over $\mathbb F_2$, adjoining each vector multiplies the size by at most two. Since $|\widetilde W|\le|4B|\le C^4|B|$, the [Freiman-Ruzsa bound from Bogolyubov and linear modelling](../../../../../freiman-ruzsa-bound-from-bogolyubov-and-linear-modelling.md) yields

$$
\boxed{|V|\le K(C)|A|,\qquad
K(C)=C^4\,2^{\,1+\lceil C^5\,2^{\lceil32C^{24}\rceil}\rceil}.}
$$

This bound depends only on $C$, as required, and every [sumset](../../../../../sumset.md) estimate used in its derivation has been proved.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
