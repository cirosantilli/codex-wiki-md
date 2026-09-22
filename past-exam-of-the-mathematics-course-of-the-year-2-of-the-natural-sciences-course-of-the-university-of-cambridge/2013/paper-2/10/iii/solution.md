<h1 id="10/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write the finite [cyclic group](../../../../../cyclic-group.md) as $C_n=\langle g:g^n=e\rangle$, the source's $Z_n$. It is Abelian, so $hgh^{-1}=g$ and every [conjugacy class](../../../../../conjugacy-class.md) is a singleton: there are $n$ such classes.

Over the complex numbers, all its [irreducible representations](../../../../../irreducible-representation.md) are one-dimensional. One direct proof is that the matrix representing $g$ has an eigenvector over $\mathbb C$; its line is preserved by every power of that matrix and hence by the whole group. Irreducibility forces the line to be the whole representation space. Its eigenvalue must be an $n$th root of unity.

The [complex irreducible representations of a finite cyclic group](../../../../../complex-irreducible-representations-of-a-finite-cyclic-group.md) are therefore

$$
\boxed{D_j(g^r)=\chi_j(g^r)=\exp\left(\frac{2\pi ijr}{n}\right),\qquad j=0,1,\ldots,n-1.}
$$

Their generator values are distinct, so no two are equivalent. There are $n$ of them, and $n$ squared dimensions equal one, exhausting the [sum of squares of irreducible representation dimensions](../../../../../sum-of-squares-of-irreducible-representation-dimensions.md): $\sum_jd_j^2=n=|G|$. Thus the list is complete.

For $n=3$, let $\omega=e^{2\pi i/3}$, so $\omega^3=1$ and $1+\omega+\omega^2=0$. The [character table](../../../../../character-table.md) is

$$
\boxed{\begin{array}{c|ccc}
&I&g&g^2\\\hline
\chi_0&1&1&1\\
\chi_1&1&\omega&\omega^2\\
\chi_2&1&\omega^2&\omega
\end{array}.}
$$

The complex-field convention is essential. The preceding part used real matrices, but that does not make the one-dimensional classification valid over $\mathbb R$: conjugate nonreal characters combine into the two-dimensional [irreducible real representations of a finite cyclic group](../../../../../irreducible-real-representations-of-a-finite-cyclic-group.md). The character table and dimension-sum result used here have their usual complex meaning.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
