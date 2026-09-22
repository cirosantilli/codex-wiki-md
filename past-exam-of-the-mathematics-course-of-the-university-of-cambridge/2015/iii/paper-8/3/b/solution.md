<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a smooth test function $\varphi$, [integration by parts](../../../../../../integration-by-parts.md) gives the moment identity

$$
\frac d{dt}\int\varphi(v)f(t,v)\,dv
=\int\bigl(\Delta\varphi-v\cdot\nabla\varphi\bigr)f(t,v)\,dv.
$$

The assumed decay removes all boundary terms. Apply it to $1$, $v_i$ and $|v|^2/2$. Writing $m_i=\int v_if=M u_i$ gives the [Ornstein-Uhlenbeck moment equations](../../../../../../ornstein-uhlenbeck-moment-equations.md)

$$
\boxed{M'=0,\qquad m_i'=-m_i,\qquad E'=dM-2E.}
$$

Assume $M(0)\ne0$ when using the normalized mean $u$; otherwise $u$ is undefined, while the unnormalized [momentum](../../../../../../momentum.md) equation still holds. Since $M$ is constant, $u_i'=-u_i$. **Their solutions are**

$$
\boxed{M(t)=M_0,\qquad
u_i(t)=e^{-t}u_i(0),\qquad
E(t)=\frac{dM_0}{2}+
\left(E(0)-\frac{dM_0}{2}\right)e^{-2t}.}
$$

Thus [mass](../../../../../../mass.md) is conserved, the [mean velocity](../../../../../../mean-velocity-of-a-kinetic-distribution.md) tends to zero, and $E(t)\to dM_0/2$. This includes the [mean velocity](../../../../../../mean-velocity-of-a-kinetic-distribution.md) conclusion omitted from the converted TeX.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
