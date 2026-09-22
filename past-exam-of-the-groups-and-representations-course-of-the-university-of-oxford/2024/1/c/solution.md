<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

There is one complex [irreducible representation](../../../../irreducible-representation.md) for each [conjugacy class](../../../../conjugacy-class.md), hence three. The [trivial representation](../../../../trivial-representation.md) $\mathbf1$ and [sign representation](../../../../sign-representation.md) $\varepsilon$ are distinct and one-dimensional. The [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) leaves

$$
1^2+1^2+d^2=6,\qquad\boxed{d=2.}
$$

Call the remaining [irreducible representation](../../../../irreducible-representation.md) $\mathbf2$. The [permutation representation](../../../../permutation-representation.md) on $\mathbb C^3$ has [character](../../../../character-of-a-representation.md) equal to the number of fixed objects, namely $(3,1,0)$ on the ordered [conjugacy classes](../../../../conjugacy-class.md) $(e,\text{transpositions},\text{three-cycles})$. Removing its constant-vector [trivial representation](../../../../trivial-representation.md) gives $(2,0,-1)$, whose [character inner product](../../../../character-inner-product.md) with itself is one. This constructs $\mathbf2$ and gives the [character table](../../../../character-table.md)

$$
\boxed{\begin{array}{c|rrr}
\text{class}&e&(12)&(123)\\
\text{class size}&1&3&2\\\hline
\chi_{\mathbf1}&1&1&1\\
\chi_{\varepsilon}&1&-1&1\\
\chi_{\mathbf2}&2&0&-1
\end{array}.}
$$

To obtain every [Clebsch-Gordan decomposition of group representations](../../../../clebsch-gordan-decomposition-of-group-representations.md), multiply the [characters](../../../../character-of-a-representation.md) pointwise. In particular, $\chi_\varepsilon^2=\chi_{\mathbf1}$, $\chi_\varepsilon\chi_{\mathbf2}=\chi_{\mathbf2}$ and

$$
\chi_{\mathbf2}^2=(4,0,1)=\chi_{\mathbf1}+\chi_\varepsilon+\chi_{\mathbf2}.
$$

Thus all ordered pairs of [irreducible representations](../../../../irreducible-representation.md) are covered by

$$
\boxed{\begin{array}{c|ccc}
\otimes&\mathbf1&\varepsilon&\mathbf2\\\hline
\mathbf1&\mathbf1&\varepsilon&\mathbf2\\
\varepsilon&\varepsilon&\mathbf1&\mathbf2\\
\mathbf2&\mathbf2&\mathbf2&\mathbf1\oplus\varepsilon\oplus\mathbf2
\end{array}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the groups and representations course of the University of Oxford](../../../split.md)
5. [Groups and representations course of the University of Oxford](../../../../groups-and-representations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
