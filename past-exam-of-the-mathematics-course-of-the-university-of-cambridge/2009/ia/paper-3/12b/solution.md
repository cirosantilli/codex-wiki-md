<h1 id="12b/solution">Solution</h1>

↑ **Parent:** [12B](../12b.md)

The [divergence theorem](../../../../../divergence-theorem.md) states that for a continuously differentiable vector field on a bounded region with outward unit normal $\mathbf n$ and suitably regular, possibly piecewise smooth, boundary,

$$
\int_V\nabla\cdot\mathbf u\,dV=\int_{\partial V}\mathbf u\cdot\mathbf n\,dS.
$$

For a differentiable [homogeneous function](../../../../../homogeneous-function.md), differentiate $f(k\mathbf x)=k^nf(\mathbf x)$ at $k=1$ to get [Euler theorem for homogeneous functions](../../../../../euler-theorem-for-homogeneous-functions.md):

$$
\boxed{\mathbf x\cdot\nabla f=nf.}
$$

Only positive $k$ near one is needed for this derivative, so no interpretation of noninteger powers at negative $k$ is required. Applying the product rule gives $\nabla\cdot(f\mathbf x)=3f+\mathbf x\cdot\nabla f=(n+3)f$. The [volume integral of a homogeneous function](../../../../../volume-integral-of-a-homogeneous-function.md) is therefore

$$
\boxed{\int_Vf\,dV=\frac1{n+3}\int_{\partial V}f\,\mathbf x\cdot\mathbf n\,dS\quad(n\ne-3).}
$$

The condition $n\ne-3$ is needed for division; at that degree the [divergence](../../../../../divergence.md) theorem instead gives only zero net boundary flux. The field $f\mathbf x$ must also be regular on the region, or singularities must be treated by excision and limiting boundary terms. Neither issue arises for the polynomial in the final calculation.

Write $r=\sqrt{x^2+y^2}$. In the cone, $0\leq z\leq\alpha$ and $0\leq r\leq z/\alpha$. The polynomial $f=z^4+\alpha^4r^4$ has degree four. Its direct volume integral is

$$
\begin{aligned}
\int_V f\,dV
&=2\pi\int_0^\alpha\int_0^{z/\alpha}(z^4+\alpha^4r^4)r\,dr\,dz\\
&=2\pi\int_0^\alpha\left(\frac{z^6}{2\alpha^2}+\frac{z^6}{6\alpha^2}\right)dz
=\boxed{\frac{4\pi\alpha^5}{21}}.
\end{aligned}
$$

On the lateral cone the outward normal is proportional to $\alpha\mathbf e_r-\mathbf e_z$, so $\mathbf x\cdot\mathbf n$ is proportional to $\alpha r-z=0$. Thus the lateral contribution vanishes. The cap is $z=\alpha$, $0\leq r\leq1$, with outward normal $\mathbf e_z$, so

$$
\int_{\partial V}f\,\mathbf x\cdot d\mathbf A
=2\pi\alpha^5\int_0^1(1+r^4)r\,dr
=\frac{4\pi\alpha^5}{3}.
$$

Multiplying by $1/(n+3)=1/7$ reproduces $4\pi\alpha^5/21$, verifying the formula. The cap edge and apex have zero surface measure, and the piecewise smooth version of the [divergence](../../../../../divergence.md) theorem applies.

## ↑ Ancestors (10)

1. [12B](../12b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
