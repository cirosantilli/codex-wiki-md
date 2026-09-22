<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $x_1,x_2,x_3$ be the coordinate basis of the [defining representation](../../../../../../../defining-representation-of-a-matrix-lie-algebra.md) $W$ of $\mathfrak{sl}_3$. Write $s_{ij}=x_ix_j$ for $1\leq i\leq j\leq3$. The six $s_{ij}$ form a basis of the [symmetric power](../../../../../../../symmetric-power.md) $\operatorname{Sym}^2W$, with weight $L_i+L_j$. A basis for the [tensor product of Lie algebra representations](../../../../../../../tensor-product-of-lie-algebra-representations.md) $T$ consists of all 36 ordered tensors

$$
\boxed{s_{ij}\otimes s_{k\ell}\quad(1\leq i\leq j\leq3,\ 1\leq k\leq\ell\leq3).}
$$

The order of the two factors matters; there is no quotient identifying their interchange.

Each [weight of a representation](../../../../../../../weight-of-a-representation.md) has the form $k_1L_1+k_2L_2+k_3L_3$, where the nonnegative [integers](../../../../../../../integer.md) satisfy $k_1+k_2+k_3=4$. Its [weight multiplicity](../../../../../../../weight-multiplicity.md) is the number of ways to split this triple into two nonnegative triples, each summing to two. The possible patterns, including every permutation, are

$$
\begin{array}{c|c|c}
(k_1,k_2,k_3)\text{ up to permutation}&\text{number of weights}&\text{multiplicity}\\\hline
(4,0,0)&3&1\\
(3,1,0)&6&2\\
(2,2,0)&3&3\\
(2,1,1)&3&4
\end{array}
$$

For example, $(2,2,0)$ splits as $(2,0,0)+(0,2,0)$, the reverse split, or $(1,1,0)+(1,1,0)$, giving multiplicity three. For $(2,1,1)$, the four splits pair $(2,0,0)$ with $(0,1,1)$ and $(1,1,0)$ with $(1,0,1)$, each in both orders. The multiplicities sum to $3+12+9+12=36$, verifying the dimension.

The following [weight diagram](../../../../../../../weight-diagram.md) uses [Dynkin labels](../../../../../../../dynkin-label.md) $(p,q)=(k_1-k_2,k_2-k_3)$; the circle numbers give multiplicities and orange points mark the [Closed dominant Weyl chamber](../../../../../../../closed-dominant-weyl-chamber.md).

<a id="1/b/i/image-the-fifteen-weights-and-multiplicities-of-sym2-c3-tensor-sym2-c3"></a>
![](../../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-3-sl3-weights.png)

**[Figure 2](#1/b/i/image-the-fifteen-weights-and-multiplicities-of-sym2-c3-tensor-sym2-c3). The fifteen weights and multiplicities of Sym2 C3 tensor Sym2 C3**.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
