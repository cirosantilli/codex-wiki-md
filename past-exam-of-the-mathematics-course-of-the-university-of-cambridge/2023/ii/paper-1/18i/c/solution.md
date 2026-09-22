<h1 id="18i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\alpha=\sqrt[4]7$. The roots of $T^4-7$ are $\alpha,i\alpha,-\alpha,-i\alpha$, so its [splitting field](../../../../../../splitting-field.md) is

$$
L=\mathbb Q(\alpha,i).
$$

The polynomial is [irreducible](../../../../../../irreducible-polynomial.md) over $\mathbb Q$ by the Eisenstein criterion at $7$, and $\mathbb Q(\alpha)\subset\mathbb R$ does not contain $i$. The [tower law for field extensions](../../../../../../tower-law-for-field-extensions.md) therefore gives $[L:\mathbb Q]=8$.

Define automorphisms

$$
r(\alpha)=i\alpha,quad r(i)=i,qquad
s(\alpha)=\alpha,quad s(i)=-i.
$$

They satisfy $r^4=s^2=1$ and $srs=r^{-1}$. The eight maps $r^j$ and $r^js$ are distinct, so they exhaust the Galois group. Hence

$$
\operatorname{Gal}(L/\mathbb Q)\cong D_8,
$$

the [dihedral group](../../../../../../dihedral-group.md) of order eight.

The [Galois correspondence](../../../../../../galois-correspondence.md) gives all intermediate fields. The full list, with a single generator for each field, is

$$
\begin{array}{c|c|c}
\text{subgroup}&\text{fixed field}&\text{normal over }\mathbb Q\\ \hline
D_8&\mathbb Q=\mathbb Q(0)&\text{yes}\\
\langle r\rangle&\mathbb Q(i)&\text{yes}\\
\langle r^2,s\rangle&\mathbb Q(\sqrt7)&\text{yes}\\
\langle r^2,rs\rangle&\mathbb Q(\sqrt{-7})&\text{yes}\\
\langle r^2\rangle&\mathbb Q(\sqrt7+i)&\text{yes}\\
\langle s\rangle&\mathbb Q(\alpha)&\text{no}\\
\langle r^2s\rangle&\mathbb Q(i\alpha)&\text{no}\\
\langle rs\rangle&\mathbb Q((1+i)\alpha)&\text{no}\\
\langle r^3s\rangle&\mathbb Q((1-i)\alpha)&\text{no}\\
\{1\}&L=\mathbb Q(\alpha+i)&\text{yes}.
\end{array}
$$

For example, $\sqrt7+i$ has stabilizer $\langle r^2\rangle$, and $(1+i)\alpha$ has stabilizer $\langle rs\rangle$; the other entries follow similarly. Also $\alpha+i$ has trivial stabilizer, so its orbit has eight elements and the [primitive element theorem](../../../../../../primitive-element-theorem.md) conclusion $L=\mathbb Q(\alpha+i)$ holds explicitly.

Finally, the [normal subextension criterion](../../../../../../normal-subextension-criterion.md) says that normal intermediate fields correspond exactly to normal subgroups. In $D_8$ these are $D_8$, $\langle r\rangle$, the two index-two Klein four-groups, $\langle r^2\rangle$, and $\{1\}$, which gives exactly the “yes” rows above. This is the [subfields of the splitting field of x to the fourth minus seven](../../../../../../subfields-of-the-splitting-field-of-x-to-the-fourth-minus-seven.md) lattice.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18I](../../18i.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
