<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the finite [Galois extension](../../../../../../finite-galois-extension.md), normalize the [discrete valuation](../../../../../../discrete-valuation.md) $v_L$ to have value group $\mathbb Z$. The [inertia group](../../../../../../inertia-group.md) is

$$
I=G_0=\ker\bigl(G\to\operatorname{Gal}(k_L/k_K)\bigr).
$$

The [lower ramification numbering](../../../../../../lower-ramification-numbering.md) is

$$
G_i=\{\sigma\in G:v_L(\sigma x-x)\ge i+1\text{ for every }x\in\mathcal O_L\},\qquad i\ge0.
$$

The [wild inertia group](../../../../../../wild-inertia-group.md) is $P=G_1$, and the [tame inertia quotient](../../../../../../tame-inertia-quotient.md) is $I/P$. We will prove that $P$ is a $p$-group, where $p=\operatorname{char}k_K$, and that $I/P$ is cyclic of order prime to $p$. Tame inertia here is a quotient, not a specified canonical subgroup complementary to $P$.

First reduce the inertia calculation to a [totally ramified extension](../../../../../../totally-ramified-extension.md). Choose $\bar b$ generating the finite residue extension $k_L/k_K$. Its minimal polynomial is separable. Lift that monic polynomial to $f\in\mathcal O_K[X]$, and use [Hensel lemma](../../../../../../hensel-s-lemma.md) in $\mathcal O_L$ to obtain a root $b$ with residue $\bar b$. Irreducibility of the reduction implies irreducibility of $f$ over $K$, by the monic form of the [Gauss lemma for polynomials](../../../../../../gauss-lemma-for-polynomials.md) over a [discrete valuation ring](../../../../../../discrete-valuation-ring.md). Thus $K_0=K(b)$ has degree $[k_L:k_K]$ and residue field $k_L$; the degree formula makes $K_0/K$ unramified. An automorphism fixes $b$ precisely when it fixes $\bar b$: the nontrivial direction is uniqueness in [Hensel lemma](../../../../../../hensel-s-lemma.md). Hence $I=\operatorname{Gal}(L/K_0)$, and $L/K_0$ is totally ramified.

Use the permitted integral-generation fact $\mathcal O_L=\mathcal O_{K_0}[\pi_L]$. Every element of $I$ fixes the coefficients in this expression. The identity $\sigma(\pi_L^j)-\pi_L^j=(\sigma\pi_L-\pi_L)\sum_{h=0}^{j-1}(\sigma\pi_L)^h\pi_L^{j-1-h}$ consequently proves the [uniformizer criterion for lower ramification groups](../../../../../../uniformizer-criterion-for-lower-ramification-groups.md):

$$
G_i=\{\sigma\in I:v_L(\sigma\pi_L-\pi_L)\ge i+1\},\qquad i\ge0.
$$

Necessity follows by testing $x=\pi_L$, and the displayed power identity proves sufficiency for every integral polynomial in $\pi_L$.

Define the [uniformizer character of inertia](../../../../../../uniformizer-character-of-inertia.md)

$$
\theta_0:I\to k_L^\times,\qquad\theta_0(\sigma)=\overline{\sigma\pi_L/\pi_L}.
$$

It is multiplicative: writing $u_\tau=\tau\pi_L/\pi_L$, one has $\sigma\tau\pi_L/\pi_L=\sigma(u_\tau)(\sigma\pi_L/\pi_L)$, and $\sigma$ acts trivially on residue units. Its kernel is exactly $v_L(\sigma\pi_L-\pi_L)\ge2$, namely $G_1$. Changing the uniformizer to $u\pi_L$ leaves the residue character unchanged, since $\overline{\sigma(u)/u}=1$. Therefore

$$
I/P\hookrightarrow k_L^\times.
$$

Every finite subgroup of a field's multiplicative group is cyclic: if its exponent is $m$, every element is a root of $X^m-1$, so its order is at most $m$; a finite abelian group has an element of order its exponent, constructed by multiplying elements of maximal prime-power orders, so its order is at least $m$. Equality makes it cyclic. Here $k_L^\times$ has order $|k_L|-1$, prime to $p$. We have proved

$$
\boxed{\text{The tame inertia group }G_0/G_1\text{ is cyclic of order prime to }p.}
$$

To verify the assertion about wild inertia as well, for $i\ge1$ define

$$
\theta_i:G_i\to(k_L,+),\qquad\theta_i(\sigma)=\overline{\frac{\sigma\pi_L-\pi_L}{\pi_L^{i+1}}}.
$$

Write $\sigma\pi_L=\pi_L+a\pi_L^{i+1}$ and $\tau\pi_L=\pi_L+b\pi_L^{i+1}$. Composition gives $\sigma\tau\pi_L\equiv\pi_L+(a+b)\pi_L^{i+1}\pmod{\pi_L^{i+2}}$, because inertia fixes residues and $i\ge1$. Thus $\theta_i$ is additive with kernel $G_{i+1}$. Thus [positive ramification quotients are elementary abelian](../../../../../../positive-ramification-quotients-are-elementary-abelian.md): each $G_i/G_{i+1}$ is a subgroup of the additive finite field, hence an elementary abelian $p$-group.

Finally the filtration terminates: a nonidentity element of $I$ cannot fix $\pi_L$, since it already fixes $K_0$ and $\mathcal O_L=\mathcal O_{K_0}[\pi_L]$. Its displacement has finite valuation, and there are only finitely many automorphisms. Iterating the finite $p$-group quotients gives that $P$ is a $p$-group. It is normal in $I$ and has prime-to-$p$ quotient, so it is its unique Sylow $p$-subgroup, justifying the wild inertia terminology.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
