<h1 id="18f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If $\delta\notin\mathbb Q(\alpha)$, then

$$
[K:\mathbb Q(\alpha)]=2,
\qquad
[K:\mathbb Q]=8.
$$

Let

$$
s(\alpha)=\alpha,\qquad s(\delta)=-\delta.
$$

This is the nonidentity automorphism of $K/\mathbb Q(\alpha)$. By extending an embedding that sends $\alpha$ to $\beta$, and composing with $s$ if necessary, choose

$$
r(\alpha)=\beta,\qquad r(\delta)=-\delta.
$$

Then

$$
r:\alpha\mapsto\beta\mapsto-\alpha
\mapsto-\beta\mapsto\alpha,
\qquad
r^4=s^2=1,
\qquad
srs=r^{-1}.
$$

The eight elements

$$
1,r,r^2,r^3,s,sr,sr^2,sr^3
$$

are distinct, and exhaust the Galois group. Thus the [dihedral Galois action on four radical roots](../../../../../../dihedral-galois-action-on-four-radical-roots.md) gives

$$
\boxed{\operatorname{Gal}(K/\mathbb Q)\cong D_8.}
$$

Now suppose $c$ is a square in $\mathbb Q$. Then $\delta\in\mathbb Q$, so every automorphism fixes $\delta$. We are in case (i) with $\tau(\delta)=\delta$, and therefore

$$
\operatorname{Gal}_{\mathbb Q}(g)\cong C_2\times C_2.
$$

Conversely, suppose the group is the [Klein four-group](../../../../../../klein-four-group.md). Label the roots

$$
\alpha,\ -\alpha,\ \beta,\ -\beta,
\qquad \alpha\beta=\delta.
$$

The three nonidentity elements in its transitive action are the three double transpositions. Each fixes $\delta$: they send the ordered pair $(\alpha,\beta)$ respectively to

$$
(-\alpha,-\beta),\qquad
(\beta,\alpha),\qquad
(-\beta,-\alpha),
$$

whose products all equal $\alpha\beta$. Hence every element of the Galois group fixes $\delta$. By the [Artin fixed-field theorem](../../../../../../artin-fixed-field-theorem.md),

$$
\delta\in K^{\operatorname{Gal}(K/\mathbb Q)}=\mathbb Q.
$$

Therefore $c=\delta^2$ is a square in $\mathbb Q$. This proves the [Klein-four criterion for an irreducible even quartic](../../../../../../klein-four-criterion-for-an-irreducible-even-quartic.md):

$$
\boxed{
\operatorname{Gal}_{\mathbb Q}(g)\cong C_2\times C_2
\quad\Longleftrightarrow\quad
c\in(\mathbb Q^\times)^2.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18F](../../18f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
