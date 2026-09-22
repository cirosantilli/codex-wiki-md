<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

In the order of [conjugacy classes](../../../../conjugacy-class.md) used in part (c), the elements of $H$ have the following types:

$$
\begin{array}{c|c}
\text{type in }S_4&\text{elements in }H\\\hline
1&1\\
(12)&rs=(13),\ r^3s=(24)\\
(12)(34)&r^2=(13)(24),\ s=(12)(34),\ r^2s=(14)(23)\\
(123)&\text{none}\\
(1234)&r,\ r^3
\end{array}.
$$

By part (d), only $1$ and $r^2$ have nonzero [character](../../../../character-of-a-representation.md) values. Formula (b), or equivalently the element-sum version proved there, therefore gives

$$
\chi_V(1)=[G:H]\dim W=3\cdot2=6,
\qquad
\chi_V((12)(34))=\frac{|C_G((12)(34))|}{|H|}(-2)=\frac88(-2)=-2,
$$

with zero on the other three [conjugacy classes](../../../../conjugacy-class.md). Here the [centralizer](../../../../centralizer.md) order is $24/3=8$. Thus $\chi_V=(6,0,-2,0,0)$.

Let $\varepsilon$ denote the [sign representation](../../../../sign-representation.md) and take the explicit two-dimensional $G$-[module](../../../../module-mathematics.md)

$$
U=\mathbf1\oplus\varepsilon.
$$

Its [character](../../../../character-of-a-representation.md) is $\chi_U=(2,0,2,2,0)$. The [character](../../../../character-of-a-representation.md) of a [tensor product of group representations](../../../../tensor-product-of-group-representations.md) is the pointwise product of their [characters](../../../../character-of-a-representation.md), because $\operatorname{tr}(M\otimes N)=\operatorname{tr}(M)\operatorname{tr}(N)$. Consequently

$$
\chi_{C\otimes U}
=(3,-1,-1,0,1)(2,0,2,2,0)
=(6,0,-2,0,0)=\chi_V.
$$

By [Maschke's theorem](../../../../maschke-s-theorem.md) both [complex representations](../../../../complex-representation.md) are [semisimple representations](../../../../semisimple-representation.md), and [characters distinguish finite-dimensional complex semisimple representations](../../../../characters-distinguish-finite-dimensional-complex-semisimple-representations.md). Therefore

$$
\boxed{V\cong C\otimes(\mathbf1\oplus\varepsilon)
\cong C\oplus(C\otimes\varepsilon).}
$$

This is the [induction of the planar square representation to the symmetric group on four letters](../../../../induction-of-the-planar-square-representation-to-the-symmetric-group-on-four-letters.md).

The [dimension](../../../../dimension-vector-space.md) of the [fixed-point subspace of a group action](../../../../fixed-point-subspace-of-a-group-action.md) is the multiplicity of the [trivial representation](../../../../trivial-representation.md). Its [character inner product](../../../../character-inner-product.md) here is

$$
\dim V^G=\langle\chi_V,1\rangle_G
=\frac{6+3(-2)}{24}=0.
$$

Hence **$V^G=0$**. Equivalently, [Frobenius reciprocity](../../../../frobenius-reciprocity.md) identifies this multiplicity with $\langle\chi_W,1_H\rangle_H=(2-2)/8=0$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the introduction to representation theory course of the University of Oxford](../../../split.md)
5. [Introduction to representation theory course of the University of Oxford](../../../../introduction-to-representation-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
