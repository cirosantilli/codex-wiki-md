<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the traceless diagonal [Cartan subalgebra](../../../../../cartan-subalgebra.md) of the [special linear Lie algebra](../../../../../special-linear-lie-algebra.md) $\mathfrak{sl}_n(\mathbb C)$. Write $\varepsilon_i(\operatorname{diag}(h_1,\ldots,h_n))=h_i$, so $\sum_i\varepsilon_i=0$. The standard coordinate vectors $e_i$ are [weight vectors](../../../../../weight-vector.md) of weights $\varepsilon_i$, and the [tensor product of Lie algebra representations](../../../../../tensor-product-of-lie-algebra-representations.md) has basis

$$
e_i\otimes(e_j\wedge e_k),\qquad 1\le i\le n,\quad j<k.
$$

The [weight](../../../../../weight-representation-theory.md) of this basis vector is $\varepsilon_i+\varepsilon_j+\varepsilon_k$. There are two possibilities:

$$
\boxed{\begin{array}{c|c|c}
\text{weight}&\text{indices}&\text{weight-space dimension}\\\hline
2\varepsilon_a+\varepsilon_b&a\ne b&1\\
\varepsilon_a+\varepsilon_b+\varepsilon_c&a<b<c&3
\end{array}}
$$

The first has basis $e_a\otimes(e_a\wedge e_b)$, with the wedge ordered if necessary. In the second, the tensor's first factor can be any one of the three indicated coordinate vectors. No two different listed coefficient patterns restrict to the same functional on the traceless diagonal [Cartan subalgebra](../../../../../cartan-subalgebra.md): their difference would have to be a multiple of $(1,\ldots,1)$, but its coefficient sum is zero. All unlisted [weight spaces](../../../../../weight-space.md) are zero. As a check,

$$
n(n-1)+3\binom n3=\frac{n^2(n-1)}2=\dim(V\otimes\Lambda^2V).
$$

For $n=3$, the distinct-index [weight](../../../../../weight-representation-theory.md) is zero and has multiplicity three.

To determine the irreducible summands, take the upper triangular [raising operators](../../../../../raising-operator.md). The vector $v_1=e_1\otimes(e_1\wedge e_2)$ is killed by every such operator and has [highest weight](../../../../../highest-weight-of-a-representation.md) $2\varepsilon_1+\varepsilon_2=\omega_1+\omega_2$. The [exterior product](../../../../../exterior-product.md) map

$$
A:V\otimes\Lambda^2V\longrightarrow\Lambda^3V,\qquad A(v\otimes(u\wedge w))=v\wedge u\wedge w
$$

is a [Lie algebra representation homomorphism](../../../../../lie-algebra-representation-homomorphism.md). It has an equivariant right inverse

$$
\iota(e_a\wedge e_b\wedge e_c)=\frac13\left[e_a\otimes(e_b\wedge e_c)-e_b\otimes(e_a\wedge e_c)+e_c\otimes(e_a\wedge e_b)\right].
$$

Indeed $A\iota=I$. The vector $\iota(e_1\wedge e_2\wedge e_3)$ is a [highest-weight vector](../../../../../highest-weight-vector.md) of [weight](../../../../../weight-representation-theory.md) $\varepsilon_1+\varepsilon_2+\varepsilon_3$.

The [Weyl complete reducibility theorem](../../../../../weyl-complete-reducibility-theorem.md) and [highest-weight representation](../../../../../highest-weight-representation.md) theory show that $v_1$ generates an irreducible summand in $\ker A$. To check that it exhausts this [kernel](../../../../../kernel-of-a-linear-map.md), use the [Weyl dimension formula](../../../../../weyl-dimension-formula.md) with the partition $(2,1,0,\ldots,0)$:

$$
\dim L(\omega_1+\omega_2)=\prod_{i<j}\frac{\lambda_i-\lambda_j+j-i}{j-i}
=2\prod_{j=3}^n\frac{j+1}{j-1}\prod_{j=3}^n\frac{j-1}{j-2}
=\frac{n(n^2-1)}3.
$$

This equals $\dim\ker A=n\binom n2-\binom n3$. The [exterior-power Lie algebra representation](../../../../../exterior-power-lie-algebra-representation.md) $\Lambda^3V$ is irreducible, with [highest weight](../../../../../highest-weight-of-a-representation.md) $\omega_3$ for $n\ge4$, and is the one-dimensional trivial representation for $n=3$. Therefore the [tensor product of the standard representation with its exterior square](../../../../../tensor-product-of-the-standard-representation-with-its-exterior-square.md) gives

$$
\boxed{V\otimes\Lambda^2V\cong\begin{cases}
L(\omega_1+\omega_2)\oplus L(\omega_3),&n\ge4,\\
L(\omega_1+\omega_2)\oplus L(0),&n=3.
\end{cases}}
$$

Each summand occurs once; their [dimensions](../../../../../dimension-vector-space.md) are $n(n^2-1)/3$ and $\binom n3$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
