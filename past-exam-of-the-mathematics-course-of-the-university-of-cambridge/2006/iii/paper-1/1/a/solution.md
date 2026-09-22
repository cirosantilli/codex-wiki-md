<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the standard [sl2 triple](../../../../../../sl2-triple.md) $H=x\partial_x-y\partial_y$, $X=x\partial_y$, $Y=y\partial_x$. In the [tensor product of Lie algebra representations](../../../../../../tensor-product-of-lie-algebra-representations.md), each operator acts on both factors. Put

$$
u_{ij}=x^{3-i}y^i\otimes x^{2-j}y^j,\quad0\leq i\leq3,\quad0\leq j\leq2.
$$

These twelve vectors form a [weight basis](../../../../../../weight-basis.md), and $Hu_{ij}=(5-2(i+j))u_{ij}$. Thus the bases of the [weight spaces](../../../../../../weight-space.md) are

$$
\begin{array}{c|l}
\text{weight}&\text{basis}\\\hline
5&u_{00}\\
3&u_{10},u_{01}\\
1&u_{20},u_{11},u_{02}\\
-1&u_{30},u_{21},u_{12}\\
-3&u_{31},u_{22}\\
-5&u_{32}
\end{array}
$$

There are no other weights. The [weight diagram](../../../../../../weight-diagram.md) shows their multiplicities, with the decomposition also displayed for comparison.

<a id="1/a/image-weights-and-multiplicities-of-the-cubic-by-quadratic-sl2-tensor-product-and-its-irreducible-summands"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-1-sl2-weights.png)

**[Figure 1](#1/a/image-weights-and-multiplicities-of-the-cubic-by-quadratic-sl2-tensor-product-and-its-irreducible-summands). Weights and multiplicities of the cubic by quadratic sl2 tensor product and its irreducible summands**.

The [raising operator](../../../../../../raising-operator.md) acts by

$$
Xu_{ij}=i\,u_{i-1,j}+j\,u_{i,j-1},
$$

with out-of-range terms omitted. At weights five, three and one its kernels are respectively spanned by

$$
\boxed{h_5=u_{00},\qquad h_3=u_{10}-u_{01},\qquad h_1=u_{20}-2u_{11}+u_{02}.}
$$

At weight one the kernel equations are $2a+b=0$ and $b+2c=0$ for $au_{20}+bu_{11}+cu_{02}$. At weight minus one they are $3a+b=0$, $2b+2c=0$, $c=0$, which force zero; the maps on the two remaining negative-weight spaces are injective as well. Thus these three lines give **all nonzero [highest-weight vectors](../../../../../../highest-weight-vector.md) up to scalar**, at their respective weights. A linear combination of different lines is killed by $X$ but is not a [weight vector](../../../../../../weight-vector.md), so is not a [highest-weight vector](../../../../../../highest-weight-vector.md).

The [lowering operator](../../../../../../lowering-operator.md) is

$$
Yu_{ij}=(3-i)u_{i+1,j}+(2-j)u_{i,j+1}.
$$

In particular,

$$
\boxed{h_1=u_{20}-2u_{11}+u_{02},\qquad Yh_1=u_{30}-2u_{21}+u_{12}}
$$

is an explicit [basis](../../../../../../basis.md) for the submodule $\Gamma_1$. Indeed $Y^2h_1=0$, $Xh_1=0$, $X(Yh_1)=h_1$, and the two vectors have weights $1,-1$. The analogous strings from $h_5,h_3$ have dimensions six and four. Their distinct irreducible highest weights and total dimension twelve give the [sl2 tensor product of cubic and quadratic symmetric powers](../../../../../../sl2-tensor-product-of-cubic-and-quadratic-symmetric-powers.md)

$$
\boxed{U\cong\Gamma_5\oplus\Gamma_3\oplus\Gamma_1.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
