<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use [Dynkin labels](../../../../../dynkin-label.md) $(a,b)$ for the [highest weight](../../../../../highest-weight-of-a-representation.md) $a\omega_1+b\omega_2$ of the complex [special linear Lie algebra](../../../../../special-linear-lie-algebra.md) $\mathfrak{sl}_3$. The [A2 root system](../../../../../a2-root-system.md) has $\alpha_1=(2,-1)$ and $\alpha_2=(-1,2)$ in these coordinates. In the drawings, $\omega_1$ and $\omega_2$ have equal lengths and angle $60^\circ$; a label at a point records its [weight multiplicity](../../../../../weight-multiplicity.md), not a further copy at a different position.

The defining [fundamental representation](../../../../../fundamental-representation.md) has the three [weights](../../../../../weight-representation-theory.md)

$$
\boxed{\Gamma_{1,0}:\quad(1,0),\ (-1,1),\ (0,-1),\quad\text{each of multiplicity }1.}
$$

For $\Gamma_{2,1}$, lower from its [highest weight](../../../../../highest-weight-of-a-representation.md) by the [simple roots](../../../../../simple-root.md), retaining multiplicities. One convenient way to calculate them is the [sl3 interlacing character formula](../../../../../sl3-interlacing-character-formula.md): for shape $(3,1,0)$ the integer patterns satisfy $1\le p\le3$, $0\le q\le1$, $q\le r\le p$, and contribute the [weight](../../../../../weight-representation-theory.md)

$$
(r-(p+q-r),\ (p+q-r)-(4-p-q)).
$$

Enumerating these patterns gives the [weight diagram](../../../../../weight-diagram.md)

$$
\begin{array}{c|l}
\text{multiplicity}&\text{weights of }\Gamma_{2,1}\\\hline
2&(1,0),\ (-1,1),\ (0,-1)\\
1&(2,1),\ (3,-1),\ (2,-2),\ (1,-3),\ (-1,-2),\ (-2,0),\ (-3,2),\ (-2,3),\ (0,2).
\end{array}
$$

Its dimension is $3\cdot2+9=15$. The diagram below draws all twelve distinct positions, with the three inner multiplicities equal to two. The extra panel gives the [symmetric square](../../../../../symmetric-square.md) used in the calculation.

<a id="3/image-a2-weight-diagrams-for-gamma-2-1-the-defining-gamma-1-0-and-its-symmetric-square-with-every-weight-multiplicity"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-2-input-weight-diagrams.png)

**[Figure 1](#3/image-a2-weight-diagrams-for-gamma-2-1-the-defining-gamma-1-0-and-its-symmetric-square-with-every-weight-multiplicity). A2 weight diagrams for Gamma(2,1), the defining Gamma(1,0), and its symmetric square, with every weight multiplicity**.

The six symmetric monomials in the defining [basis](../../../../../basis.md) give $S^2\Gamma_{1,0}=\Gamma_{2,0}$, with [weights](../../../../../weight-representation-theory.md)

$$
(2,0),\ (0,1),\ (1,-1),\ (-2,2),\ (-1,0),\ (0,-2),
$$

each occurring once. Thus **the tensor product has dimension**

$$
\boxed{\dim V=15\cdot6=90.}
$$

In a [tensor product of Lie algebra representations](../../../../../tensor-product-of-lie-algebra-representations.md), [weights](../../../../../weight-representation-theory.md) add and their multiplicities multiply. In terms of [formal characters](../../../../../formal-character-of-a-weight-module.md), $\operatorname{ch}V=\operatorname{ch}\Gamma_{2,1}\operatorname{ch}\Gamma_{2,0}$. Consequently $m_V(\mu)=\sum_\nu m_{2,1}(\mu-\nu)$, summing over the six [weights](../../../../../weight-representation-theory.md) just listed. To show the indicated dominant multiplicities explicitly, the contributions in that order are

$$
\begin{array}{c|rrrrrr|r}
\mu& (2,0)&(0,1)&(1,-1)&(-2,2)&(-1,0)&(0,-2)&m_V(\mu)\\\hline
(4,1)&1&0&0&0&0&0&1\\
(2,2)&1&1&0&0&0&0&2\\
(3,0)&2&1&1&0&0&0&4\\
(0,3)&1&1&0&1&0&0&3\\
(1,1)&2&2&1&1&1&0&7
\end{array}
$$

The [tensor-product weight diagram](../../../../../tensor-product-weight-diagram.md) below includes every position, and highlights these dominant [weights](../../../../../weight-representation-theory.md). It also records the zero-weight multiplicity nine; that multiplicity is not a count of trivial summands.

<a id="3/image-all-weights-of-the-ninety-dimensional-sl3-tensor-product-gamma-2-1-tensor-sym2-gamma-1-0-with-dominant-weights-highlighted-and-multiplicities-labelled"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-2-tensor-weight-diagram.png)

**[Figure 2](#3/image-all-weights-of-the-ninety-dimensional-sl3-tensor-product-gamma-2-1-tensor-sym2-gamma-1-0-with-dominant-weights-highlighted-and-multiplicities-labelled). All weights of the ninety-dimensional sl3 tensor product Gamma(2,1) tensor Sym2 Gamma(1,0), with dominant weights highlighted and multiplicities labelled**.

Apply the [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md) and subtract irreducible [formal characters](../../../../../formal-character-of-a-weight-module.md) in decreasing [dominance order](../../../../../dominance-order.md). The multiplicities at these five dominant positions in the potential summands are

$$
\begin{array}{c|rrrrr|r}
& (4,1)&(2,2)&(3,0)&(0,3)&(1,1)&\text{dimension}\\\hline
\Gamma_{4,1}&1&1&2&1&2&35\\
\Gamma_{2,2}&0&1&1&1&2&27\\
\Gamma_{3,0}&0&0&1&0&1&10\\
\Gamma_{0,3}&0&0&0&1&1&10\\
\Gamma_{1,1}&0&0&0&0&1&8
\end{array}
$$

These entries can be obtained by the same interlacing enumeration or by [weight strings](../../../../../weight-string.md). Starting with $(1,2,4,3,7)$, subtracting $\Gamma_{4,1}$ leaves $(0,1,2,2,5)$; subtracting $\Gamma_{2,2}$ leaves $(0,0,1,1,3)$; then the two ten-dimensional modules leave a single copy of the dominant [weight](../../../../../weight-representation-theory.md) $(1,1)$. This is [highest-weight character subtraction](../../../../../highest-weight-character-subtraction.md). Therefore

$$
\boxed{V\cong\Gamma_{4,1}\oplus\Gamma_{2,2}\oplus\Gamma_{3,0}\oplus\Gamma_{0,3}\oplus\Gamma_{1,1}.}
$$

Every summand occurs once. The [Weyl dimension formula](../../../../../weyl-dimension-formula.md) gives $35+27+10+10+8=90$, exhausting the dimension of $V$ and ruling out further irreducible summands. Computing the complete [formal character](../../../../../formal-character-of-a-weight-module.md) also leaves no residual [weight multiplicities](../../../../../weight-multiplicity.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
