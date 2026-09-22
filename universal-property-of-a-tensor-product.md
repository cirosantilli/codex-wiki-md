# Universal property of a tensor product

↑ **Parent:** [Tensor product](tensor-product.md)

For a [bilinear map](bilinear-map.md) $B:V\times W\to U$, there is exactly one [linear map](linear-map.md) $L:V\otimes_F W\to U$ satisfying $L(v\otimes w)=B(v,w)$. Equivalently, $B=L\circ\tau$, where $\tau(v,w)=v\otimes w$. The [universal property of a tensor product](universal-property-of-a-tensor-product.md) concerns the [vector space](vector-space-split.md) together with this distinguished [bilinear map](bilinear-map.md).[§9D, Theorem 9.79(a), printed p. 375: unique linear factorization](linear-algebra-done-right-by-sheldon-axler-4th-edition.md)

Here is a complete calculation over the [real numbers](real-number.md). Define the [bilinear map](bilinear-map.md)

$$
B(v,w)=\bigl(v_1w_1+2v_1w_2+v_2w_2,\ v_2w_1-v_1w_2\bigr).
$$

Its values on pairs of [basis vectors](basis-vector.md) determine $L$ on the four [tensor-product basis](tensor-product-basis.md) elements:

$$
\begin{aligned}
L(e_1\otimes f_1)&=(1,0),&L(e_1\otimes f_2)&=(2,-1),\\
L(e_2\otimes f_1)&=(0,1),&L(e_2\otimes f_2)&=(1,0).
\end{aligned}
$$

Consequently, for $t=\sum_{i,j=1}^2c_{ij}e_i\otimes f_j$,

$$
L(t)=(c_{11}+2c_{12}+c_{22},\ c_{21}-c_{12}).
$$

For $v=(2,1)$ and $w=(-1,3)$, the direct calculation gives $B(v,w)=(-2+12+3,-1-6)=(13,-7)$. Using the expansion of $v\otimes w$ instead gives $L(v\otimes w)=-2(1,0)+6(2,-1)-(0,1)+3(1,0)=(13,-7)$. The [linear map](linear-map.md) also handles a nonseparable [tensor](tensor.md) such as $t=e_1\otimes f_1+e_2\otimes f_2$: $L(t)=(2,0)$, even though no single pair has $v\otimes w=t$.

<a id="image-a-bilinear-calculation-factors-through-one-linear-map-on-four-tensor-coefficients"></a>
![](tensor-product-bilinear-factorization.png)

**[Figure 36](#image-a-bilinear-calculation-factors-through-one-linear-map-on-four-tensor-coefficients). A bilinear calculation factors through one linear map on four tensor coefficients**.

A short proof uses a [tensor-product basis](tensor-product-basis.md): assign $L(e_i\otimes f_j)=B(e_i,f_j)$ and extend by [linearity](linearity.md). Expanding both inputs verifies $L(v\otimes w)=B(v,w)$ by [bilinearity](bilinearity.md); the assigned values on a [basis](basis.md) force uniqueness. More generally, every [multilinear map](multilinear-map.md) $F:V_1\times\cdots\times V_r\to U$ factors uniquely through a [linear map](linear-map.md) from $V_1\otimes\cdots\otimes V_r$. This lets formulas involving several inputs define [linear maps](linear-map.md) without choosing [coordinates](coordinate-linear-algebra.md); [tensor contraction](tensor-contraction.md) uses the evaluation pairing between a [vector](vector.md) and a [covector](covector.md).

## ↑ Ancestors (7)

1. [Tensor product](tensor-product.md)
2. [Multilinear algebra](multilinear-algebra.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Multilinear map](multilinear-map.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-115/2/a/solution.md)
- [Universal property of a tensor product](universal-property-of-a-tensor-product.md)
