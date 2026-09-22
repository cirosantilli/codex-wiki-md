<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [symmetric group](../../../../symmetric-group.md) $S_3$ has three [conjugacy classes](../../../../conjugacy-class.md), determined by cycle type: the identity, three [transpositions](../../../../transposition-permutation.md), and two three-cycles. Hence it has three complex [irreducible representations](../../../../irreducible-representation.md). Two are the [trivial representation](../../../../trivial-representation.md) $\mathbf1$ and the [sign representation](../../../../sign-representation.md) $\varepsilon$. Their [dimensions](../../../../dimension-vector-space.md) are one, so the [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) gives $1+1+d^2=6$, whence $d=2$ for the remaining [representation](../../../../group-representation.md) $D$.

Write $\chi_D=(2,a,b)$ on these classes. Orthogonality to $\mathbf1$ and $\varepsilon$ gives $2+3a+2b=0$ and $2-3a+2b=0$. Thus $a=0,b=-1$, and the [character table](../../../../character-table.md) is

$$
\boxed{\begin{array}{c|rrr}
&e&(12)&(123)\\\hline
\text{class size}&1&3&2\\\hline
\mathbf1&1&1&1\\
\varepsilon&1&-1&1\\
D&2&0&-1
\end{array}}
$$

The [character](../../../../character-of-a-representation.md) of a [tensor product representation](../../../../tensor-product-of-group-representations.md) is the product of the factor [characters](../../../../character-of-a-representation.md). Thus $\varepsilon^2=\mathbf1$, $\varepsilon\otimes D=D$, and $\chi_{D\otimes D}=(4,0,1)=\chi_{\mathbf1}+\chi_\varepsilon+\chi_D$. These determine all the [Clebsch-Gordan decomposition of group representations](../../../../clebsch-gordan-decomposition-of-group-representations.md):

$$
\boxed{\begin{array}{c|ccc}
\otimes&\mathbf1&\varepsilon&D\\\hline
\mathbf1&\mathbf1&\varepsilon&D\\
\varepsilon&\varepsilon&\mathbf1&D\\
D&D&D&\mathbf1\oplus\varepsilon\oplus D
\end{array}}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../c/solution.md)
