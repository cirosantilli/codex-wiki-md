<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The class sizes sum to $|G|=36$. A degree-one [character](../../../../../character-of-a-representation.md) is a homomorphism into $\mathbb C^\times$. The supplied $\chi_2$ has order four and $\chi_2^2=\chi_1$, so $1,\chi_2,\chi_1,\bar\chi_2$ are four distinct [irreducible characters](../../../../../irreducible-character.md). A finite [group](../../../../../group-split.md) has as many complex [irreducible characters](../../../../../irreducible-character.md) as [conjugacy classes](../../../../../conjugacy-class.md), so there are exactly two more. Their degrees $d,e$ satisfy $d^2+e^2=36-4=32$, whose only positive-integer solution is $d=e=4$.

The [column orthogonality](../../../../../column-orthogonality.md) give $\sum_\chi|\chi(g)|^2=|C_G(g)|$. Each of the last three classes has centralizer order $36/9=4$, already exhausted by the four degree-one rows. Thus both new rows vanish on $C_4,C_5,C_6$.

To justify that their remaining values are real, put $P=\ker\chi_2$. The supplied values show $P=C_1\cup C_2\cup C_3$, a normal subgroup of order nine, with $G/P\cong C_4$. A group of order nine is [Abelian](../../../../../abelian-group.md), by the standard [p-group](../../../../../p-group.md) center argument and the fact that a cyclic quotient by the center forces the group to be [Abelian](../../../../../abelian-group.md). If $P$ were cyclic of order nine, conjugation through $G/P$ would act by an automorphism of order dividing both four and $|\operatorname{Aut}(C_9)|=6$, hence dividing two. Its nontrivial conjugacy classes could not have size four. Therefore $P\cong C_3^2$.

Let $h$ map to a generator of $G/P$, and let $A$ be its conjugation action on the two-dimensional [vector space](../../../../../vector-space-split.md) $P$ over $\mathbb F_3$. The two nonzero orbits have length four, so $A^2$ fixes no nonzero vector, while $A^4=I$. Since $t^2-1$ has distinct roots in characteristic three, the involution $A^2$ is diagonalizable; the absence of a $+1$ eigenvector gives $A^2=-I$. Thus conjugation by $h^2$ inverts every element of $P$. Every element in $C_2,C_3$ is therefore conjugate to its inverse, so every [character](../../../../../character-of-a-representation.md) value there is real.

Write one new row as $(4,a,b,0,0,0)$. Its orthogonality with the trivial row gives $4+4a+4b=0$, so $a+b=-1$. Its squared [character inner product](../../../../../character-inner-product.md) one gives $16+4a^2+4b^2=36$, so $a^2+b^2=5$ and $ab=-2$. Thus $a,b$ are $1,-2$ in some order. Column orthogonality with the identity column forces the other row's entries to be interchanged. Up to relabelling these two new characters, the completed [character table](../../../../../character-table.md) is

$$
\boxed{\begin{array}{c|rrrrrr}
&C_1&C_2&C_3&C_4&C_5&C_6\\\hline
1&1&1&1&1&1&1\\
\chi_1&1&1&1&1&-1&-1\\
\chi_2&1&1&1&-1&i&-i\\
\bar\chi_2&1&1&1&-1&-i&i\\
\chi_3&4&1&-2&0&0&0\\
\chi_4&4&-2&1&0&0&0
\end{array}.}
$$

The reality argument prevents an unjustified assumption when solving the orthogonality equations. This is [character table from a cyclic quotient and two elementary-abelian orbits](../../../../../character-table-from-a-cyclic-quotient-and-two-elementary-abelian-orbits.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the algebra course of the University of Oxford](../../../../split.md)
6. [Algebra course of the University of Oxford](../../../../../algebra-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
