<h1 id="9/solution">Solution</h1>

↑ **Parent:** [9](../9.md)

**Conjugacy classes.** For $a\in G$, its [conjugacy class](../../../../conjugacy-class.md) is

$$
\boxed{\operatorname{Cl}(a)=\{gag^{-1}:g\in G\}.}
$$

Every element belongs to its own [conjugacy class](../../../../conjugacy-class.md), by taking $g=e$. To prove uniqueness, suppose $x=gag^{-1}=hbh^{-1}$ belongs to both $\operatorname{Cl}(a)$ and $\operatorname{Cl}(b)$. Then

$$
b=(h^{-1}g)a(h^{-1}g)^{-1}.
$$

For every $t\in G$, this makes $tbt^{-1}$ a conjugate of $a$ as well. Hence $\operatorname{Cl}(b)\subseteq\operatorname{Cl}(a)$, and reversing the argument gives the other inclusion. Two [conjugacy classes](../../../../conjugacy-class.md) that meet are therefore equal, proving that the classes partition $G$.

**Abelian case.** If $G$ is an [abelian group](../../../../abelian-group.md), then $gag^{-1}=agg^{-1}=a$ for every $g$, so $\boxed{\operatorname{Cl}(a)=\{a\}}$ for each $a$.

**Centre.** An element has a singleton [conjugacy class](../../../../conjugacy-class.md) precisely when $gzg^{-1}=z$ for every $g$, equivalently $gz=zg$ for every $g$. Thus the definition in the paper agrees with the usual [centre of a group](../../../../center-of-a-group.md):

$$
Z(G)=\{z\in G:gz=zg\text{ for every }g\in G\}.
$$

The identity lies in $Z(G)$. If $z,w\in Z(G)$, then for any $g$, $gzw=zgw=zwg$, so $zw\in Z(G)$. Also $gz=zg$ implies $z^{-1}g=gz^{-1}$, so $z^{-1}\in Z(G)$. This proves it is a [subgroup](../../../../subgroup.md). Any two of its elements commute because either one commutes with every element of $G$. Consequently $\boxed{Z(G)\text{ is an abelian subgroup of }G}$.

**Square symmetry.** Use the paper's notation $D_4$ for the eight-element [dihedral group](../../../../dihedral-group.md) of a square. Let $r$ be a quarter-turn and $s$ a reflection, so $r^4=s^2=e$ and $srs=r^{-1}$. A rotation $r^j$ commutes with $s$ exactly when $r^j=r^{-j}$, or $2j=0$ modulo four. This selects $e$ and $r^2$. No reflection $r^js$ commutes with $r$, because

$$
(r^js)r=r^{j-1}s,\qquad r(r^js)=r^{j+1}s,
$$

and $r^{j-1}\ne r^{j+1}$. Therefore

$$
\boxed{Z(D_4)=\{e,r^2\}=\{\text{identity},\text{half-turn}\}.}
$$

## ↑ Ancestors (12)

1. [9](../9.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
