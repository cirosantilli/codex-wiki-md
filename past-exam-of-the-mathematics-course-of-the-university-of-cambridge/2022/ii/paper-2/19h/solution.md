<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

[Irreducible degrees](../../../../../irreducible-character-degree.md) divide the [order](../../../../../order-of-a-finite-group.md) of a finite $2$-group and satisfy

$$
\sum_i d_i^2=|G|=16.
$$

The number of [linear characters](../../../../../linear-character.md) is $|G/G'|$. For a [nontrivial](../../../../../nontrivial-group.md) finite $2$-group this is at least $4$ unless the group is [abelian](../../../../../abelian-group.md), and every [nonlinear](../../../../../nonlinear-irreducible-character.md) degree is at least $2$. A degree $4$ constituent is therefore impossible in the nonabelian case. If there are $\ell$ linear and $m$ degree-two characters, then

$$
\ell+4m=16,\qquad \ell\in\{4,8,16\}.
$$

Thus the only degree collections are

$$
\boxed{1^{16}},\qquad
\boxed{1^8,2^2},\qquad
\boxed{1^4,2^3},
$$

with respectively $r=16,10,7$.

For $1^{16}$ take the [cyclic group](../../../../../cyclic-group.md) $G=C_{16}=\langle g\rangle$. Every [conjugacy class](../../../../../conjugacy-class.md) is a [singleton](../../../../../singleton-mathematics.md), and its [character table](../../../../../character-table.md) is

$$
\chi_j(g^k)=\zeta_{16}^{\,jk},
\qquad 0\leq j,k<16,
$$

where $\zeta_{16}=e^{2\pi i/16}$.

For $1^8,2^2$, take $G=D_8\times C_2$, where  
$D_8=\langle r,s:r^4=s^2=1,\ srs=r^{-1}\rangle$ and  
$C_2=\langle z\rangle$. On the five classes

$$
1,\quad r^2,\quad\{r,r^3\},\quad
\{s,r^2s\},\quad\{rs,r^3s\},
$$

the four linear characters of $D_8$, indexed by  
$\varepsilon,\delta\in\{\pm1\}$, and its degree-two character are

$$
\chi_{\varepsilon,\delta}=(1,1,\varepsilon,\delta,\varepsilon\delta),
\qquad
\psi=(2,-2,0,0,0).
$$

The ten classes of $G$ are $(C,1)$ and $(C,z)$. Its full table consists of

$$
(\chi\otimes\eta)(C,z^e)=\chi(C)\eta^e,
$$

where $\chi$ runs over the above five rows and  
$\eta\in\{1,-1\}$ runs over the two characters of $C_2$. This explicitly gives eight linear and two degree-two rows.

For $1^4,2^3$, take the [dihedral group](../../../../../dihedral-group.md)

$$
D_{16}=\langle r,s:r^8=s^2=1,\ srs=r^{-1}\rangle.
$$

Order its seven classes as

$$
1,\ r^4,\ \{r,r^7\},\ \{r^2,r^6\},\
\{r^3,r^5\},\
\{r^{2j}s\}_{j=0}^3,\ \{r^{2j+1}s\}_{j=0}^3.
$$

The four linear rows are

$$
\chi_{\varepsilon,\delta}
=(1,1,\varepsilon,1,\varepsilon,\delta,\varepsilon\delta),
\qquad \varepsilon,\delta=\pm1.
$$

The three degree-two rows, for $k=1,2,3$, are

$$
\psi_k=
\left(
2,\ 2(-1)^k,\
2\cos\frac{k\pi}{4},\
2\cos\frac{k\pi}{2},\
2\cos\frac{3k\pi}{4},\
0,\ 0
\right).
$$

The row norms and mutual inner products, weighted by the displayed class sizes, verify irreducibility and completeness.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
