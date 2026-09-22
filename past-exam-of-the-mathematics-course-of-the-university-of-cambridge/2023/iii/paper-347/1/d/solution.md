<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $w=1/r$ and $h=r^2\dot\theta=bv_\infty$. Since $\dot r=-h\,dw/d\theta$, the radial equation becomes the [Binet equation](../../../../../../binet-equation.md)

$$
\frac{d^2w}{d\theta^2}+w=\frac{GM}{h^2},
$$

whose solution is

$$
w=c_1\cos\theta+c_2\sin\theta+\frac{GM}{b^2v_\infty^2}.
$$

Choose the incoming asymptote at $\theta=\pi$ and the downstream axis at $\theta=0$. Then $w\to0$ as $\theta\to\pi$, while $r\sin\theta\to b$. These two conditions give

$$
c_1=\frac{GM}{b^2v_\infty^2},
\qquad c_2=\frac1b.
$$

The mirror-image streamlines meet on the downstream axis at

$$
\boxed{r_{\rm coll}=\frac{b^2v_\infty^2}{2GM}.}
$$

At that point each streamline has radial velocity $-v_\infty$ and equal and opposite azimuthal velocity. An inelastic collision cancels the latter, so the specific energy afterwards is

$$
E_{\rm after}=\frac{v_\infty^2}{2}-\frac{GM}{r_{\rm coll}}
=\frac{v_\infty^2}{2}-\frac{2G^2M^2}{b^2v_\infty^2}.
$$

The gas is bound when $E_{\rm after}<0$, or

$$
\boxed{b<b_{\rm crit}=\frac{2GM}{v_\infty^2}.}
$$

Sweeping the corresponding capture cylinder through gas of density $\rho_\infty$ gives the [Bondi--Hoyle--Lyttleton accretion rate](../../../../../../bondi-hoyle-lyttleton-accretion-rate.md)

$$
\boxed{\dot M=\pi b_{\rm crit}^2\rho_\infty v_\infty
=\frac{4\pi G^2M^2\rho_\infty}{v_\infty^3}.}
$$

Unlike stationary spherical [Bondi accretion](../../../../../../bondi-accretion.md), this is a directed, supersonic flow with a downstream focusing wake; bulk speed replaces sound speed as the main resistance to capture.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 347](../../../paper-347-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
