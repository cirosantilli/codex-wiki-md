<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

In the sense of [distribution theory](../../../../../distribution-theory-split.md), $H'(t)=\delta(t)$. Since $\sin(\alpha t)$ vanishes at zero,

$$
\psi'(t)=H(t)\cos(\alpha t),
\qquad
\psi''(t)=\delta(t)-\alpha H(t)\sin(\alpha t),
$$

and therefore

$$
\boxed{\psi''+\alpha^2\psi=\delta(t)}.
$$

Let $G_{\rm ret}(\mathbf x,t;\mathbf y)$ solve

$$
(\partial_t^2-c^2\nabla^2)G_{\rm ret}
=\delta(t)\delta^{(3)}(\mathbf x-\mathbf y),
\qquad G_{\rm ret}=0\quad(t<0).
$$

The spatial [Fourier transform](../../../../../fourier-transform.md) turns this into the preceding oscillator equation with $\alpha=ck$, so

$$
\widehat G(\mathbf k,t)=H(t)\frac{\sin(ckt)}{ck}.
$$

Inverting with the supplied radial integral gives the three-dimensional [retarded Green function](../../../../../retarded-green-function.md)

$$
\boxed{G_{\rm ret}(\mathbf x,t;\mathbf y)
=\frac{H(t)}{4\pi c|\mathbf x-\mathbf y|}
\delta(|\mathbf x-\mathbf y|-ct)
=\frac{\delta(t-|\mathbf x-\mathbf y|/c)}{4\pi c^2|\mathbf x-\mathbf y|}}.
$$

For zero initial displacement and initial velocity $f$, convolution with this kernel gives the [Kirchhoff formula](../../../../../kirchhoff-formula.md)

$$
\begin{aligned}
u(\mathbf x,t)
&=\int_{\mathbb R^3}G_{\rm ret}(\mathbf x,t;\mathbf y)f(\mathbf y)\,d^3y\\
&=\frac{t}{4\pi}\int_{S^2}f(\mathbf x+ct\,\boldsymbol\omega)\,d\Omega
=t\langle f\rangle_t.
\end{aligned}
$$

**Thus the value at $(\mathbf x,t)$ depends only on the initial data on the sphere of radius $ct$, not on its interior. This is the [Huygens principle](../../../../../strong-huygens-principle.md) and describes propagation at the finite wave speed $c$.**

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
