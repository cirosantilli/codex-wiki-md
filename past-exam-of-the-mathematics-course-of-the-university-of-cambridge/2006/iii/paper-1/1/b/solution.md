<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $f_1,f_2,f_3$ be the [dual basis](../../../../../../dual-basis.md) of $W^*$, and use $L_1+L_2+L_3=0$. The elementary tensors $e_i\otimes e_j\otimes f_k$ have weight $L_i+L_j-L_k$. Grouping them gives every [weight space](../../../../../../weight-space.md) explicitly:

$$
\begin{array}{c|c|l}
\text{weight}&\text{multiplicity}&\text{basis}\\\hline
2L_i-L_k\ (i\ne k)&1&e_i\otimes e_i\otimes f_k\\
-2L_k\ (\{i,j,k\}=\{1,2,3\},\ i<j)&2&e_i\otimes e_j\otimes f_k,\ e_j\otimes e_i\otimes f_k\\
L_i&5&e_i\otimes e_i\otimes f_i,\ e_i\otimes e_j\otimes f_j,\ e_j\otimes e_i\otimes f_j\ (j\ne i)
\end{array}
$$

The counts are $6+3\cdot2+3\cdot5=27$, so this table exhausts the [tensor product](../../../../../../tensor-product.md). The diagrams below use equilateral coordinates $L_1=(1,0)$, $L_2=(-1/2,\sqrt3/2)$, $L_3=(-1/2,-\sqrt3/2)$; numbers at points are [weight multiplicities](../../../../../../weight-multiplicity.md).

To decompose the module, first split the first two factors into their symmetric and alternating parts. Put $t_{ij}=(e_i\otimes e_j+e_j\otimes e_i)/2$, including $t_{ii}=e_i\otimes e_i$. The equivariant contraction

$$
C:S^2W\otimes W^*\to W,\qquad C(t_{ij}\otimes f_k)=\delta_{ik}e_j+\delta_{jk}e_i
$$

is onto, since $C(t_{ii}\otimes f_i)=2e_i$. Its kernel $K$ has dimension fifteen and contains the [highest-weight vector](../../../../../../highest-weight-vector.md) $t_{11}\otimes f_3$ of weight $2L_1-L_3$.

Here is an explicit [weight basis of the trace-free symmetric-square dual tensor module](../../../../../../weight-basis-of-the-trace-free-symmetric-square-dual-tensor-module.md), and thus the requested fifteen-vector [basis](../../../../../../basis.md):

$$
\boxed{\begin{array}{ll}
t_{ii}\otimes f_k,&i\ne k\quad(6\text{ vectors}),\\
t_{ij}\otimes f_k,&i<j,\ \{i,j,k\}=\{1,2,3\}\quad(3\text{ vectors}),\\
t_{ij}\otimes f_j-\tfrac12t_{ii}\otimes f_i,&i\ne j\quad(6\text{ vectors}).
\end{array}}
$$

Every displayed vector contracts to zero. The first two families occupy distinct one-dimensional weights; at each weight $L_i$ the two vectors in the last family are independent because their respective $t_{ij}\otimes f_j$ terms are distinct. Thus all fifteen are independent and span $K$.

For completeness, $K$ is irreducible, not just an invariant kernel of the right dimension. On elementary tensors the raising action is

$$
E_{ab}(e_i\otimes e_j\otimes f_k)=\delta_{bi}e_a\otimes e_j\otimes f_k+\delta_{bj}e_i\otimes e_a\otimes f_k-\delta_{ak}e_i\otimes e_j\otimes f_b.
$$

At the six weights $2L_i-L_k$, both $E_{12}$ and $E_{23}$ kill the vector only for $(i,k)=(1,3)$. At each weight $-2L_k$, at least one of those operators is nonzero. At weight $L_1$, write a vector as $a(t_{12}\otimes f_2-t_{11}\otimes f_1/2)+b(t_{13}\otimes f_3-t_{11}\otimes f_1/2)$. The two raising equations are $3a+b=0$ and $-a+b=0$, forcing zero. On the two-dimensional weight-$L_2$ space $E_{12}$ is injective, and on the weight-$L_3$ space $E_{23}$ is injective, as substitution in the same action formula shows. Therefore the common raising kernel in $K$ is the single line $\mathbb C(t_{11}\otimes f_3)$. By [Weyl complete reducibility theorem](../../../../../../weyl-complete-reducibility-theorem.md), every irreducible summand supplies a highest-weight line, so $K$ has only one summand and is irreducible.

The symmetric-factor contraction splits off a defining copy $W$; explicitly $e_i\mapsto\sum_jt_{ij}\otimes f_j$ is equivariant and its contraction is $4e_i$. For the alternating factor, the invariant volume form identifies $\Lambda^2W\cong W^*$, sending $e_1\wedge e_2$ to $f_3$, $e_2\wedge e_3$ to $f_1$ and $e_3\wedge e_1$ to $f_2$. Therefore

$$
\Lambda^2W\otimes W^*\cong W^*\otimes W^*=S^2W^*\oplus\Lambda^2W^*\cong S^2W^*\oplus W.
$$

The symmetric dual module is irreducible of dimension six and highest weight $-2L_3$; its symmetric-monomial [basis](../../../../../../basis.md) has weights $-2L_i$ and $-L_i-L_j=L_k$, all of multiplicity one. In the original [tensor product](../../../../../../tensor-product.md) its [highest-weight vector](../../../../../../highest-weight-vector.md) is

$$
\boxed{(e_1\otimes e_2-e_2\otimes e_1)\otimes f_3.}
$$

The raising action above annihilates it, and its weight is $L_1+L_2-L_3=-2L_3$.

Altogether the [Triple tensor decomposition for the defining sl3 representation](../../../../../../triple-tensor-decomposition-for-the-defining-sl3-representation.md) is

$$
\boxed{Z\cong V(2\omega_1+\omega_2)\oplus V(2\omega_2)\oplus W\oplus W,\qquad27=15+6+3+3.}
$$

The fifteen-dimensional module has multiplicity one at each $2L_i-L_k$ and $-2L_i$, and multiplicity two at each $L_i$. The six-dimensional module has multiplicity one at $-2L_i$ and $L_i$. Each defining module has the three weights $L_i$, once each. These add to the original table of multiplicities.

<a id="1/b/image-weight-diagrams-of-the-27-dimensional-sl3-tensor-product-and-its-irreducible-summands-of-dimensions-fifteen-six-three-and-three"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-1-sl3-weights.png)

**[Figure 2](#1/b/image-weight-diagrams-of-the-27-dimensional-sl3-tensor-product-and-its-irreducible-summands-of-dimensions-fifteen-six-three-and-three). Weight diagrams of the 27-dimensional sl3 tensor product and its irreducible summands of dimensions fifteen, six, three and three**.

The two defining summands are not intrinsically distinguished: other diagonal copies inside their isotypic component have the same three-point [weight diagram](../../../../../../weight-diagram.md). Thus the displayed diagrams account for every irreducible submodule type, as well as showing both copies in this decomposition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
