<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A set $S$ of [prime numbers](../../../../../prime-number.md) has [Dirichlet density](../../../../../dirichlet-density.md) $\delta$ if the following limit exists:

$$
\delta(S)=\lim_{s\downarrow1}\frac{\sum_{p\in S}p^{-s}}{\log(1/(s-1))}=\delta.
$$

Equivalently, the denominator can be $\sum_p p^{-s}$, since that sum is $\log(1/(s-1))+O(1)$. Adding or removing finitely many [prime numbers](../../../../../prime-number.md) leaves the [Dirichlet density](../../../../../dirichlet-density.md) unchanged.

Put $\alpha=\sqrt[4]{2}>0$ and $L=\mathbb Q(\alpha,i)$. This is the [splitting field](../../../../../splitting-field.md) of $X^4-2$, whose four [roots of a polynomial](../../../../../root-of-a-polynomial.md) are $\alpha,i\alpha,-\alpha,-i\alpha$. The polynomial is an [Eisenstein polynomial](../../../../../eisenstein-polynomial.md) at $2$, so $[\mathbb Q(\alpha):\mathbb Q]=4$. Since $\mathbb Q(\alpha)$ is contained in the [real numbers](../../../../../real-number.md), it does not contain $i$, giving $[L:\mathbb Q]=8$. Thus $L/\mathbb Q$ is a [Galois extension](../../../../../finite-galois-extension.md) of degree $8$. Its [Galois group](../../../../../galois-group.md) is the [dihedral group](../../../../../dihedral-group.md) of order $8$: the [field automorphisms](../../../../../field-automorphism.md) $r(\alpha)=i\alpha$, $r(i)=i$ and $s(\alpha)=\alpha$, $s(i)=-i$ satisfy $r^4=s^2=1$ and $srs=r^{-1}$.

For an odd [prime number](../../../../../prime-number.md) $p$, the condition $p\equiv1\pmod4$ means that the [finite field](../../../../../finite-field.md) $\mathbb F_p$ contains all fourth [roots of unity](../../../../../root-of-unity.md). Under this condition, $2$ is a [quartic residue](../../../../../quartic-residue.md) exactly when $X^4-2$ has a root in $\mathbb F_p$; multiplying that root by $1,i,-1,-i$ gives all four distinct roots. Conversely, complete splitting of $X^4-2$ over $\mathbb F_p$ gives both a fourth root of $2$ and a primitive fourth [root of unity](../../../../../root-of-unity.md), so it also forces $p\equiv1\pmod4$.

The [polynomial discriminant](../../../../../polynomial-discriminant.md) of $X^4-2$ is $-2^{11}$. Hence every odd [prime number](../../../../../prime-number.md) is unramified in $L$, and the root-splitting criterion is equivalent to its [Frobenius automorphism](../../../../../frobenius-automorphism.md) acting trivially on all the roots. Since the roots generate $L$, this is equivalent to the [Frobenius automorphism](../../../../../frobenius-automorphism.md) being the identity, or to $p$ being a [completely split prime](../../../../../completely-split-prime.md) of $L/\mathbb Q$. The [Chebotarev density theorem](../../../../../chebotarev-density-theorem.md) says that the unramified [prime numbers](../../../../../prime-number.md) with [Frobenius conjugacy class](../../../../../frobenius-conjugacy-class.md) $C$ have [Dirichlet density](../../../../../dirichlet-density.md) $|C|/|\operatorname{Gal}(L/\mathbb Q)|$. Here $C=\{1\}$, so

$$
\boxed{\delta(S)=\frac18.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
