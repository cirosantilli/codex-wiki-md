<h1 id="1c/solution">Solution</h1>

↑ **Parent:** [1C](../1c.md)

Using the [Levi-Civita symbol](../../../../../levi-civita-symbol.md) and the [contraction of two Levi-Civita symbols](../../../../../contraction-of-two-levi-civita-symbols.md), the $i$th component of the [vector triple product](../../../../../vector-triple-product.md) is

$$
\epsilon_{ijk}a_j\epsilon_{klm}b_lc_m
=(\delta_{il}\delta_{jm}-\delta_{im}\delta_{jl})a_jb_lc_m
=b_i(a_jc_j)-c_i(a_jb_j).
$$

Thus **the triple-product identity is** $a\times(b\times c)=(a\cdot c)b-(a\cdot b)c$.

Apply this with the unit vector $n$ to obtain $\Pi(x)=x-(n\cdot x)n$. [Dot products](../../../../../dot-product.md) and scalar multiplication are linear in $x$, so $\Pi(sx+ty)=s\Pi(x)+t\Pi(y)$. Its [matrix representation](../../../../../matrix-representation.md) is

$$
\boxed{P=I-nn^T,\qquad P_{ij}=\delta_{ij}-n_in_j.}
$$

The fixed-vector equation is equivalent to $(n\cdot x)n=0$. Since $n\ne0$, **all its solutions are** $x\in n^\perp$. Also $\boxed{\Pi(n)=0}$. Every vector decomposes as $x=\Pi(x)+(n\cdot x)n$, with $\Pi(x)$ orthogonal to $n$. Hence $\Pi$ is the [orthogonal projection](../../../../../orthogonal-projection.md) onto the plane through the origin normal to $n$: it fixes that plane and removes the perpendicular component.

## ↑ Ancestors (10)

1. [1C](../1c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
