<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

Let $r=dim(U\cap W)$. Choose a [basis](../../../../../basis.md) $e_1,\ldots,e_r$ of the [intersection of vector subspaces](../../../../../intersection-of-vector-subspaces.md), extend it to a basis $e_1,\ldots,e_r,u_{r+1},\ldots,u_m$ of $U$, and independently extend it to a basis $e_1,\ldots,e_r,w_{r+1},\ldots,w_n$ of $W$. The combined list

$$
e_1,\ldots,e_r,u_{r+1},\ldots,u_m,w_{r+1},\ldots,w_n
$$

spans the [sum of vector subspaces](../../../../../sum-of-vector-subspaces.md) $U+W$. It is also [linearly independent](../../../../../linear-independence.md): a vanishing [linear combination](../../../../../linear-combination.md) says that a combination of the $u_i$ belongs to $U\cap W$, and its expression in the chosen basis of $U$ forces all its coefficients to vanish; the coefficients of the $w_i$ then vanish in the same way. This proves the [dimension formula for a sum of subspaces](../../../../../dimension-formula-for-a-sum-of-subspaces.md)

$$
\boxed{\dim(U+W)=\dim U+\dim W-\dim(U\cap W)}.
$$

Parametrize the two [linear subspaces](../../../../../vector-subspace.md) as

$$
U=\operatorname{span}\{(7,-5,1,0),(8,-6,0,1)\},
\qquad
W=\operatorname{span}\{(-2,1,0,0),(-3,0,1,0)\}.
$$

Putting a vector of $U$ in $W$ first forces its fourth coordinate to vanish; the remaining defining equation is then automatic. Thus

$$
U\cap W=\operatorname{span}\{(7,-5,1,0)\},
$$

and the dimension formula gives $\dim(U+W)=2+2-1=3$.

The [linear functional](../../../../../linear-functional.md)

$$
\boxed{\ell(x)=x_1+2x_2+3x_3+4x_4}
$$

vanishes on each displayed generator of $U$ and $W$. Its [kernel](../../../../../kernel-of-a-linear-map.md) is three-dimensional because $\ell\ne0$, so the inclusion $U+W\subseteq\ker\ell$ between two three-dimensional subspaces is equality.

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
