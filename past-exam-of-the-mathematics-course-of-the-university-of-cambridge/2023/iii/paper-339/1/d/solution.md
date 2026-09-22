<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Define the [softmax weights](../../../../../../softmax-function.md)

$$
p_i(x)=\frac{e^{\beta z_i(x)}}{\sum_j e^{\beta z_j(x)}}.
$$

They obey $p_i\geq0$ and $\sum_i p_i=1$. The [gradient](../../../../../../gradient.md) is their weighted mean,

$$
\boxed{\nabla f_\beta(x)=\sum_i p_i(x)a_i.}
$$

Differentiating once more gives the covariance-form [Hessian matrix](../../../../../../hessian-matrix.md)

$$
\nabla^2f_\beta(x)
=\beta\left(\sum_i p_i a_i a_i^T-\bar a\bar a^T\right),
\qquad \bar a=\sum_i p_i a_i.
$$

For every unit [vector](../../../../../../vector.md) $u$,

$$
u^T\nabla^2f_\beta(x)u
=\beta\operatorname{Var}_{i\sim p}(u^Ta_i)
\leq\beta\sum_i p_i(u^Ta_i)^2
\leq\beta G^2,
$$

where $G=\max_i\|a_i\|_2$. The Hessian is a [covariance matrix](../../../../../../covariance-matrix.md), so it is [positive semidefinite](../../../../../../positive-semidefinite-matrix.md); the displayed upper bound also gives $\nabla^2f_\beta\preceq\beta G^2I$ in the [Loewner order](../../../../../../loewner-order.md). Consequently $f_\beta$ has a [Lipschitz gradient](../../../../../../lipschitz-gradient.md) with

$$
\boxed{L=\beta G^2.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
