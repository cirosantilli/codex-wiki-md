<h1 id="b/8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

The degree-sum formula for [irreducible characters](../../../../irreducible-character.md) gives

$$
\boxed{|G|=1^2+1^2+1^2+3^2+3^2=21.}
$$

The number of [linear characters](../../../../linear-character.md) is the order of the [abelianization](../../../../abelianization.md), so **$|G/G'|=3$** and $|G'|=7$. The intersection of the kernels of all [linear characters](../../../../linear-character.md) is $G'$. Consequently $g_4,g_5$ are nonidentity elements of this order-seven subgroup and have order seven. The images of $g_2,g_3$ under a displayed [linear character](../../../../linear-character.md) have order three, so their orders are divisible by three. [Lagrange's theorem](../../../../lagrange-s-theorem.md) leaves three or twenty-one; an element of order twenty-one would make $G$ cyclic, contradicting its degree-three [irreducible characters](../../../../irreducible-character.md). Therefore

$$
\boxed{(|g_2|,|g_3|,|g_4|,|g_5|)=(3,3,7,7).}
$$

The center is trivial. A nontrivial proper center would have order three or seven, giving a cyclic quotient and hence an [abelian group](../../../../abelian-group.md), again a contradiction. Thus a [centralizer](../../../../centralizer.md) of a nonidentity element is proper. It has order three for an order-three element, and seven for an order-seven element. The class sizes are therefore $1,7,7,3,3$.

Column orthogonality says $\sum_i|\chi_i(g)|^2=|C_G(g)|$. For $g_2,g_3$, the three [linear characters](../../../../linear-character.md) already contribute three, so the remaining two entries must both vanish. Orthogonality with the identity column says $\sum_i\chi_i(1)\overline{\chi_i(g)}=0$ for $g\ne1$. At $g_4$ this gives $1+\alpha+\chi_5(g_4)=0$, so $\chi_5(g_4)=\beta$, using $\alpha+\beta=-1$. Similarly $\chi_5(g_5)=\alpha$. Thus the completed table is

$$
\boxed{\begin{array}{c|ccccc}
&e&g_2&g_3&g_4&g_5\\\hline
\text{class size}&1&7&7&3&3\\
\chi_1&1&1&1&1&1\\
\chi_2&1&\omega&\omega^2&1&1\\
\chi_3&1&\omega^2&\omega&1&1\\
\chi_4&3&0&0&\alpha&\beta\\
\chi_5&3&0&0&\beta&\alpha
\end{array}}
$$

Here $\beta=\overline\alpha$, $|\alpha|^2=|\beta|^2=2$ and $\alpha\beta=2$. These relations, together with $1+\omega+\omega^2=0$, verify all weighted row orthogonality relations and the [centralizer](../../../../centralizer.md) column norms.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
