# Separability of a tensor

↑ **Parent:** [Tensor product](tensor-product.md)

In a two-factor [tensor product](tensor-product.md) over a [field](field.md), a [pure tensor](pure-tensor.md) is also called a separable or decomposable [tensor](tensor.md): it can be expressed as one product $v\otimes w$. Every [tensor](tensor.md) is a finite sum of [pure tensors](pure-tensor.md), but a sum need not itself be a [pure tensor](pure-tensor.md).[§3, printed p. 9: elementary, simple, decomposable, and pure tensors; Example 2.1, printed pp. 4–5: outer products do not fill the matrix space](tensor-products-i-by-keith-conrad.md)

For [finite-dimensional vector spaces](finite-dimensional-vector-space.md), the [tensor-product coefficient matrix](tensor-product-coefficient-matrix.md) gives a decisive test: a nonzero [tensor](tensor.md) is a [pure tensor](pure-tensor.md) exactly when its [matrix rank](matrix-rank.md) is one. Indeed, every column of $vw^T$ is a [scalar multiple](scalar-multiple.md) of $v$. Conversely, if all columns of a nonzero [matrix](matrix.md) are multiples of one nonzero column $v$, collect their multipliers in $w$ to obtain $C=vw^T$. The zero [tensor](tensor.md) is also a [pure tensor](pure-tensor.md), for example $0\otimes w$, but its [matrix rank](matrix-rank.md) is zero.

In $\mathbb R^2\otimes_{\mathbb R}\mathbb R^2$, the [tensor](tensor.md)

$$
t=e_1\otimes f_1+e_2\otimes f_2,\qquad C(t)=\begin{pmatrix}1&0\\0&1\end{pmatrix},
$$

is nonseparable: its [matrix rank](matrix-rank.md) is two and its [determinant](determinant.md) is one, whereas $\det(vw^T)=0$. Directly, trying $t=(ae_1+be_2)\otimes(cf_1+df_2)$ requires $ac=bd=1$ and $ad=bc=0$. The first two equations force all four [scalars](scalar.md) nonzero, contradicting the others. In contrast, products sharing a factor do combine: $e_1\otimes f_1+e_1\otimes f_2=e_1\otimes(f_1+f_2)$. Thus being written as two summands alone does not establish nonseparability.

## ↑ Ancestors (7)

1. [Tensor product](tensor-product.md)
2. [Multilinear algebra](multilinear-algebra-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Tensor product](tensor-product.md)
