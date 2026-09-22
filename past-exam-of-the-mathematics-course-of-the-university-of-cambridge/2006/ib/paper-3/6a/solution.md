<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

Choose the coordinate vectors $b=e_i$ and $c=e_j$ in the assumed bilinear identity. It gives $T_{ij}=0$ for each pair of indices, hence **the tensor is zero**.

Let $\Omega$ be the enclosed region. Apply the [divergence theorem](../../../../../divergence-theorem.md) to the vector [field](../../../../../field.md) $(b\cdot x)c$. Since $b,c$ are constant,

$$
\nabla\cdot[(b\cdot x)c]=b\cdot c.
$$

Therefore

$$
\boxed{\int_S(b\cdot x)(c\cdot n)\,dS=V b\cdot c.}
$$

Writing the left side as $b_i c_j\int_S x_i n_j\,dS$ and using the initial tensor argument gives the [boundary integral of position and normal components](../../../../../boundary-integral-of-position-and-normal-components.md)

$$
\boxed{\int_S x_i n_j\,dS=V\delta_{ij}.}
$$

Contract with the [Kronecker delta](../../../../../kronecker-delta.md) to obtain $\int_S x\cdot n\,dS=3V$. Contract with the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) to obtain

$$
\left(\int_S x\times n\,dS\right)_k
=\epsilon_{kij}V\delta_{ij}=0.
$$

Thus the requested integrals are **$3V$ and the zero vector**, respectively. These applications require the usual sufficiently regular closed boundary and outward-normal orientation of the divergence theorem.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
