<h1 id="10b/solution">Solution</h1>

↑ **Parent:** [10B](../10b.md)

Expanding with the Levi-Civita symbol and the product rule gives

$$
\nabla\times(a\times b)=a\,\nabla\cdot b-b\,\nabla\cdot a
+(b\cdot\nabla)a-(a\cdot\nabla)b.
$$

The [Stokes theorem](../../../../../stokes-theorem.md) states

$$
\int_S(\nabla\times F)\cdot n\,dS=\oint_C F\cdot dx,
$$

where the boundary orientation follows the right-hand rule about $n$.

Apply it to $F=m\times v$. On $S$, $m=n$ and $v\cdot n=0$. Substitution of the [vector](../../../../../vector.md) identity and contraction with $n$ leaves

$$
(\delta_{ij}-n_in_j)\partial_jv_i.
$$

The boundary integrand satisfies $(n\times v)\cdot dx=v\cdot(dx\times n)$, proving the formula. The [vector](../../../../../vector.md) $dx\times n$ is the outward co-normal in the tangent plane of $S$.

For the hemisphere, $n=e_r$ and $v=r\sin\theta e_\theta$. The projected divergence is $2\cos\theta$, so the left side is

$$
\int_0^{2\pi}\int_0^{\pi/2}2\cos\theta R^2\sin\theta\,d\theta d\phi=2\pi R^2.
$$

On the positively oriented equator, $dx=Re_\phi d\phi$, hence $dx\times n=Re_\theta d\phi$ and the boundary [integral](../../../../../integral.md) is also $2\pi R^2$.

## ↑ Ancestors (10)

1. [10B](../10b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
