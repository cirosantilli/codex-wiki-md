<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**Rado's criterion.** Let $A$ be a [matrix](../../../../../matrix.md) over the [rational numbers](../../../../../rational-number.md), with columns $a_1,\ldots,a_q$. A [partition regular matrix](../../../../../partition-regular-matrix.md) is one for which every [finite coloring](../../../../../finite-coloring.md) of the [positive integers](../../../../../positive-integer.md) gives a [monochromatic](../../../../../monochromatic-set.md) positive vector $x\in\mathbb N^q$ with $Ax=0$; repeated coordinates are allowed. The [columns condition](../../../../../columns-property.md) is the existence of an ordered [set partition](../../../../../set-partition.md) $B_1,\ldots,B_s$ of $[q]$ into nonempty blocks such that

$$
\sum_{i\in B_1}a_i=0,\qquad
\sum_{i\in B_j}a_i\in\operatorname{span}_{\mathbb Q}\{a_i:i\in B_1\cup\cdots\cup B_{j-1}\}\quad(j>1).
$$

[Rado's theorem](../../../../../rado-s-theorem.md) states

$$
\boxed{A\text{ is partition regular if and only if it satisfies the columns condition}.}
$$

**Necessity.** Clear denominators so the columns are integer vectors. For each pair of disjoint index sets $I,B$, with $B\ne\varnothing$, for which $v_B=\sum_{i\in B}a_i$ is outside the [linear span](../../../../../linear-span.md) of the $I$-columns, choose an integer [linear functional](../../../../../linear-functional.md) $\phi_{I,B}$ that vanishes on those columns and satisfies $\phi_{I,B}(v_B)\ne0$. Such a functional exists by extending a [basis](../../../../../basis.md) of the span to one also containing $v_B$, defining a functional on that [basis](../../../../../basis.md), and clearing its rational denominators.

There are only finitely many such pairs. Choose a [prime number](../../../../../prime-number.md) $p$ dividing none of these nonzero integer evaluations. If there are no such pairs, any prime will do. Use the [last nonzero digit coloring](../../../../../last-nonzero-digit-coloring.md): write $x=p^{v_p(x)}u$, with $p\nmid u$, and color $x$ by $u\bmod p\in\{1,\ldots,p-1\}$. Since $A$ is a [partition regular matrix](../../../../../partition-regular-matrix.md), this coloring supplies a [monochromatic](../../../../../monochromatic-set.md) positive solution, so all its unit parts have a common nonzero residue $d$.

Group the coordinates by increasing [P-adic valuation](../../../../../p-adic-valuation.md), obtaining blocks $B_1,\ldots,B_s$ with valuations $e_1<\cdots<e_s$. Suppose for some $j$ the sum $v_{B_j}$ lay outside the [linear span](../../../../../linear-span.md) of the earlier columns, with earlier index set $I$. Apply $\phi_{I,B_j}$ to $Ax=0$. Earlier terms vanish exactly. Divide the remaining integer equation by $p^{e_j}$ and reduce modulo $p$. Later terms vanish modulo $p$, while the current block gives

$$
0\equiv d\,\phi_{I,B_j}(v_{B_j})\pmod p,
$$

contrary to the choice of $p$. Thus every block sum lies in the earlier [linear span](../../../../../linear-span.md), and for the first block this means it is zero. This proves the [columns condition](../../../../../columns-property.md) by the [finite separating-functional proof of the columns condition](../../../../../finite-separating-functional-proof-of-the-columns-condition.md).

**Sufficiency.** Suppose the [columns condition](../../../../../columns-property.md) holds. For $j>1$, choose rational coefficients $\lambda_{ij}$, indexed by earlier columns, such that

$$
\sum_{i\in B_j}a_i+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i=0.
$$

Take a positive integer $c$ clearing their denominators and $p\geq1$ bounding all $|c\lambda_{ij}|$. We use the allowed [monochromatic m-p-c set theorem](../../../../../monochromatic-m-p-c-set-theorem.md) with $s$ levels. Its [M-p-c set](../../../../../m-p-c-set.md) is the full set

$$
D=\bigcup_{h=1}^s\left\{cz_h+\sum_{j>h}\mu_jz_j:\mu_j\in\mathbb Z,\ |\mu_j|\leq p\right\},
$$

where the generators make every displayed expression positive. Positivity is part of this convention, rather than a rule that discards nonpositive expressions. For $i\in B_h$, set

$$
x_i=cz_h+\sum_{j>h}c\lambda_{ij}z_j.
$$

All these numbers lie in the [monochromatic](../../../../../monochromatic-set.md) set $D$. The coefficient of $z_j$ in $Ax$ is

$$
c\left(\sum_{i\in B_j}a_i+\sum_{i\in B_1\cup\cdots\cup B_{j-1}}\lambda_{ij}a_i\right)=0,
$$

with the first coefficient zero by $\sum_{i\in B_1}a_i=0$. Hence $Ax=0$. This [Rado solution inside an m-p-c set](../../../../../rado-solution-inside-an-m-p-c-set.md) proves sufficiency.

**The equality-or-inequality dichotomy.** If every [finite coloring](../../../../../finite-coloring.md) gives a [monochromatic](../../../../../monochromatic-set.md) solution with $x_1=x_2$, the first alternative holds. Otherwise fix a [finite coloring](../../../../../finite-coloring.md) $\chi$ admitting no such solution. Given any other [finite coloring](../../../../../finite-coloring.md) $\psi$, use the [refinement of a finite coloring](../../../../../refinement-of-a-finite-coloring.md) $n\mapsto(\chi(n),\psi(n))$. Since $A$ is a [partition regular matrix](../../../../../partition-regular-matrix.md), it supplies a solution [monochromatic](../../../../../monochromatic-set.md) for both colorings. Its first two coordinates cannot be equal, by the defining property of $\chi$, so it is the required unequal solution for $\psi$. Thus one of the two universal alternatives always holds. This is the [partition regularity dichotomy under an extra constraint](../../../../../partition-regularity-dichotomy-under-an-extra-constraint.md); the alternatives are not asserted to be mutually exclusive.

**Both restrictions can fail.** The Schur [matrix](../../../../../matrix.md)

$$
A=(1\ \ 1\ \ {-1})
$$

is a [partition regular matrix](../../../../../partition-regular-matrix.md): blocks $\{1,3\}$ and $\{2\}$ satisfy the [columns condition](../../../../../columns-property.md). Color $n$ by $v_2(n)\bmod2$, using the [2-adic valuation](../../../../../2-adic-valuation.md). An equal-coordinate solution would have $x_3=2x_1$, and $v_2(2x_1)=v_2(x_1)+1$, so its coordinates cannot be [monochromatic](../../../../../monochromatic-set.md). This exhibits failure of the equality restriction.

Conversely, $A=(1\ \ {-1})$ satisfies the [columns condition](../../../../../columns-property.md) in one block. Every solution has $x_1=x_2$, so even the constant one-color [finite coloring](../../../../../finite-coloring.md) admits no unequal-coordinate solution. Consequently

$$
\boxed{\text{equality can be impossible for one coloring, and inequality can be impossible for every coloring}.}
$$

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 130](../../paper-130-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
