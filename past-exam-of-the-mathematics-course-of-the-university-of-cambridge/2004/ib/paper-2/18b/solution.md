<h1 id="18b/solution">Solution</h1>

↑ **Parent:** [18B](../18b.md)

Put $\mathbf R=\mathbf r-\mathbf r'$. The [magnetic field](../../../../../magnetic-field.md) is the [curl](../../../../../curl.md) of the [magnetic vector potential](../../../../../magnetic-vector-potential.md). Since $\mathbf J(\mathbf r')$ does not depend on the differentiated variable $\mathbf r$,

$$
\nabla_{\mathbf r}\times\frac{\mathbf J(\mathbf r')}{R}
=\nabla_{\mathbf r}(R^{-1})\times\mathbf J(\mathbf r')
=-\frac{\mathbf R}{R^3}\times\mathbf J(\mathbf r')
=\frac{\mathbf J(\mathbf r')\times\mathbf R}{R^3}.
$$

Taking the [curl](../../../../../curl.md) under the source [integral](../../../../../integral.md) consequently gives the [Biot-Savart law](../../../../../biot-savart-law.md),

$$
\mathbf B(\mathbf r)=\frac{\mu_0}{4\pi}\int\frac{\mathbf J(\mathbf r')\times(\mathbf r-\mathbf r')}{|\mathbf r-\mathbf r'|^3}\,d^3r'.
$$

Outside the compact source this differentiation is ordinary differentiation of a smooth kernel. For regular volume currents, the locally integrable $R^{-2}$ derivative kernel gives the same formula at interior points.

For the loop, choose positive current circulating counterclockwise as viewed from the positive $z$-axis. Parametrize its source position and directed line element by

$$
\mathbf r'=a(\cos\varphi,\sin\varphi,0),\qquad d\boldsymbol\ell'=a(-\sin\varphi,\cos\varphi,0)\,d\varphi.
$$

At $(0,0,z)$ the denominator is the constant $(a^2+z^2)^{3/2}$, while

$$
d\boldsymbol\ell'\times\mathbf R=(az\cos\varphi,az\sin\varphi,a^2)\,d\varphi.
$$

The transverse terms integrate to zero around the loop. The [Biot-Savart law](../../../../../biot-savart-law.md) therefore yields

$$
\boxed{\mathbf B(0,0,z)=\frac{\mu_0Ia^2}{2(a^2+z^2)^{3/2}}\,\mathbf e_z.}
$$

The [magnetic field](../../../../../magnetic-field.md) is axial, with the stated magnitude for $I>0$; reversing the [electric current](../../../../../electric-current.md) reverses its direction.

## ↑ Ancestors (10)

1. [18B](../18b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
