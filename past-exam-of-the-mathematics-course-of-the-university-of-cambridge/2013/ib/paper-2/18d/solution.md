<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

For a thin wire carrying current $I$, the given [magnetic vector potential](../../../../../magnetic-vector-potential.md) reduces to $\mathbf A=(\mu_0I/4\pi)\oint_Cd\mathbf r'/|\mathbf r-\mathbf r'|$. Taking its [curl](../../../../../curl.md) and using $\nabla_{\mathbf r}(1/|\mathbf r-\mathbf r'|)=-(\mathbf r-\mathbf r')/|\mathbf r-\mathbf r'|^3$ gives the [Biot-Savart law](../../../../../biot-savart-law.md)

$$
\boxed{\mathbf B(\mathbf r)=\frac{\mu_0I}{4\pi}\oint_C\frac{d\mathbf r'\times(\mathbf r-\mathbf r')}{|\mathbf r-\mathbf r'|^3}.}
$$

This is exactly the sign convention in the printed form using $\mathbf r'-\mathbf r$.

Let $\mathbf v=(\mathbf r-\mathbf r')/|\mathbf r-\mathbf r'|^3$. Away from the wire, $\nabla\cdot\mathbf v=0$. The supplied [divergence and curl of a cross product](../../../../../divergence-and-curl-of-a-cross-product.md) therefore gives $\nabla\times(d\mathbf r'\times\mathbf v)=-(d\mathbf r'\cdot\nabla_{\mathbf r})\mathbf v$. But $\nabla_{\mathbf r}\mathbf v=-\nabla_{\mathbf r'}\mathbf v$, so the integrand is the total differential of $\mathbf v$ along the source loop. Its closed-loop integral is zero. Thus **$\nabla\times\mathbf B=0$ at every point outside $C$**, as demanded by the current-free magnetostatic [Ampère's law](../../../../../ampere-s-circuital-law.md).

For $r'=f(\theta)>0$, $z'=0$, and counterclockwise current, $d\mathbf r'=(f'\mathbf e_r+f\mathbf e_\theta)d\theta$. At the origin, $\mathbf v=-\mathbf e_r/f^2$, so

$$
\boxed{\mathbf B(0)=\widehat{\mathbf z}\,\frac{\mu_0I}{4\pi}\int_0^{2\pi}\frac{d\theta}{f(\theta)}.}
$$

For the [ellipse](../../../../../ellipse.md) expressed relative to a focus, $1/f=(1-e\cos\theta)/\ell$. The cosine integrates to zero, giving

$$
\boxed{\mathbf B_{\mathrm{focus}}=\widehat{\mathbf z}\,\frac{\mu_0I}{2\ell}.}
$$

Here $\ell$ is the [semilatus rectum](../../../../../semilatus-rectum.md). Reversing the current reverses the field direction.

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
