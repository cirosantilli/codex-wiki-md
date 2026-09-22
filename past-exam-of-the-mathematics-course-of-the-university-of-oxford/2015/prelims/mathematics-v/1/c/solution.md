<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [spherical coordinates](../../../../../../spherical-coordinate-system.md) parametrization

$$
\mathbf R(\phi,\theta)=(\sin\phi\cos\theta,\sin\phi\sin\theta,\cos\phi),
\qquad \alpha\leq\phi\leq\beta,\quad0\leq\theta\leq2\pi.
$$

Then $\mathbf R_\phi\times\mathbf R_\theta=\sin\phi\,\mathbf R$, so the outward [unit normal vector](../../../../../../unit-normal.md) is $\mathbf n=\mathbf R=\sin\phi\,\mathbf e_r+\cos\phi\,\mathbf e_z$ and the [surface area element](../../../../../../surface-area-element.md) is $\sin\phi\,d\phi\,d\theta$. Since $\sin\phi>0$ throughout this band, the [vector field](../../../../../../vector-field.md) is smooth near it. The [surface integral](../../../../../../surface-integral.md) of the [curl](../../../../../../curl.md) is

$$
\begin{aligned}
\iint_\Sigma(\nabla\times\mathbf F)\cdot\mathbf n\,dS
&=2\pi\int_\alpha^\beta\bigl[f(\cos\phi)\cos\phi-f'(\cos\phi)\sin^2\phi\bigr],d\phi\\
&=2\pi\int_\alpha^\beta\frac{d}{d\phi}\bigl[\sin\phi f(\cos\phi)\bigr],d\phi\\
&=\boxed{2\pi\bigl[\sin\beta f(\cos\beta)-\sin\alpha f(\cos\alpha)\bigr].}
\end{aligned}
$$

For the induced [boundary orientation](../../../../../../boundary-orientation.md), the lower circle $\phi=\beta$ is traversed with increasing $\theta$, and the upper circle $\phi=\alpha$ with decreasing $\theta$. One way to check the signs is that the outward [conormal](../../../../../../conormal.md) is $\mathbf e_\phi$ at the lower circle and $-\mathbf e_\phi$ at the upper circle; the positive [unit tangent vector](../../../../../../unit-tangent-vector.md) is $\mathbf n\times\text{conormal}$.

Along a circle of fixed $\phi$, $d\mathbf r=\sin\phi\,\mathbf e_\theta\,d\theta$. Therefore the [circulation](../../../../../../circulation-physics.md) is

$$
\oint_{\partial\Sigma}\mathbf F\cdot d\mathbf r
=\int_0^{2\pi} f(\cos\beta)\sin\beta\,d\theta
-\int_0^{2\pi}f(\cos\alpha)\sin\alpha\,d\theta,
$$

which equals the boxed [surface integral](../../../../../../surface-integral.md) and verifies [Stokes theorem](../../../../../../stokes-theorem.md) with the required [orientation](../../../../../../orientation-of-a-simplex.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
