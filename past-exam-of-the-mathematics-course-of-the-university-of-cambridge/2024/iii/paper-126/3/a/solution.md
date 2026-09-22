<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [group scheme](../../../../../../group-scheme.md) over $k$ is a $k$-scheme $G$ with multiplication $m_G:G\times_kG\to G$, identity $e_G:\operatorname{Spec}k\to G$, and inversion $i_G:G\to G$ satisfying the group axioms as identities of morphisms. A [homomorphism of group schemes](../../../../../../homomorphism-of-group-schemes.md) $f:H\to G$ is a $k$-morphism satisfying

$$
f\circ m_H=m_G\circ(f\times f),
$$

and it then preserves the identity and inversion.

Assume $G$ and $H$ are commutative. The group $G(H)=\operatorname{Mor}_k(H,G)$ has pointwise addition

$$
f+g=m_G\circ(f,g).
$$

For every $k$-algebra $R$ and $x,y\in H(R)$,

$$
(f+g)_R(x+y)=f_R(x)+f_R(y)+g_R(x)+g_R(y)=(f+g)_R(x)+(f+g)_R(y),
$$

where commutativity permits the middle terms to be reordered. Hence $f+g$ is a homomorphism. The zero morphism and pointwise inverse are also homomorphisms, so $\operatorname{Hom}_k(H,G)$ is a subgroup of $G(H)$. The definition immediately gives

$$
\boxed{(f+g)_R(x)=f_R(x)+g_R(x).}
$$

Repeated pointwise addition gives $(nf)_R(x)=n f_R(x)$. Since $f_R$ is a group homomorphism,

$$
n f_R(x)=f_R(nx)=([n]_G)_R(f_R(x)).
$$

The [Yoneda lemma](../../../../../../yoneda-lemma.md) turns equality on all $R$-valued points into equality of morphisms, proving

$$
\boxed{nf=f\circ[n]_H=[n]_G\circ f.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 126](../../../paper-126-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
