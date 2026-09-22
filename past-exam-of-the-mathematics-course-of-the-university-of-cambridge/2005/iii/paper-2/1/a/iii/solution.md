<h1 id="1/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the [exterior-power Lie algebra representation](../../../../../../../exterior-power-lie-algebra-representation.md):

$$
F(e_i\wedge e_j)=(4-i)e_{i+1}\wedge e_j+(4-j)e_i\wedge e_{j+1},\qquad
E(e_i\wedge e_j)=i e_{i-1}\wedge e_j+j e_i\wedge e_{j-1}.
$$

Reorder wedge factors when necessary and interpret repeated factors as zero. The [explicit weight basis of the exterior square of Sym4 for sl2](../../../../../../../explicit-weight-basis-of-the-exterior-square-of-sym4-for-sl2.md) is

$$
\begin{aligned}
v_0&=w_{01},&v_1&=w_{02},&v_2&=w_{03}+2w_{12},\\
v_3&=w_{04}+8w_{13},&v_4&=w_{14}+2w_{23},&
v_5&=w_{24},\quad v_6=w_{34},
\end{aligned}
$$

for $L(6)$, and

$$
t_0=w_{03}-3w_{12},\qquad t_1=w_{04}-2w_{13},\qquad
t_2=w_{14}-3w_{23},
$$

for $L(2)$. Their [weights](../../../../../../../weight-representation-theory.md) are $6-2j$ and $2-2j$, respectively.

Direct application of the displayed operators gives $Ev_0=Et_0=0$ and the lowering chains

$$
v_0\xrightarrow{\,F\,}3v_1,\quad
v_1\mapsto2v_2,\quad v_2\mapsto v_3,\quad
v_3\mapsto12v_4,\quad v_4\mapsto5v_5,\quad
v_5\mapsto2v_6,\quad v_6\mapsto0,
$$



$$
Ft_0=t_1,\qquad Ft_1=2t_2,\qquad Ft_2=0.
$$

The raising coefficients along the first chain are $2,5,12,1,2,3$; along the second, $Et_1=2t_0$ and $Et_2=t_1$. Thus each span is stable and is the required irreducible module. At the common [weights](../../../../../../../weight-representation-theory.md) $2,0,-2$, the $v$ and $t$ vectors are independent; the other [weight spaces](../../../../../../../weight-space.md) occur only in the first span. This proves that the ten vectors are a [basis](../../../../../../../basis.md) of $U$ and that the two spans are complementary. The [highest-weight vectors](../../../../../../../highest-weight-vector.md) are

$$
\boxed{v_0=e_0\wedge e_1\text{ of weight }6,\qquad
t_0=e_0\wedge e_3-3e_1\wedge e_2\text{ of weight }2.}
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
