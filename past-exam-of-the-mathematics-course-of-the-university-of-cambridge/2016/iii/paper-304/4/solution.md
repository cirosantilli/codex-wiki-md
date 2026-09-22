<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $\mathcal G_R=\langle\mathcal O_{1,R}(x_1)\cdots\mathcal O_{n,R}(x_n)\rangle$ at separated points, with [composite operators](../../../../../composite-operator.md) chosen in a basis without operator mixing. Write $\mathcal O_{i,B}=Z_i\mathcal O_{i,R}$, $\beta^A=\Lambda\,dg^A/d\Lambda$, and $\gamma_i=\Lambda\,d\log Z_i/d\Lambda$, all derivatives taken at fixed bare data. Bare correlations are independent of the arbitrary intermediate [renormalization scale](../../../../../renormalization-scale.md). Hence **the Callan–Symanzik equation** is

$$
\boxed{\left(\Lambda\frac{\partial}{\partial\Lambda}+\sum_A\beta^A\frac{\partial}{\partial g^A}+\sum_{i=1}^n\gamma_i\right)\mathcal G_R=0.}
$$

The explicit scale derivative holds positions and renormalized parameters fixed; the [renormalization-group beta functions](../../../../../beta-function-physics.md) describe their running; and the [anomalous dimensions](../../../../../anomalous-dimension.md) account for renormalization of each insertion. Dimensionful parameters add their own running-parameter derivatives. With [composite operator mixing](../../../../../composite-operator-mixing.md), each $\gamma_i$ is a matrix acting on its operator slot. The displayed sign follows the stated convention for $Z_i$. Coincident products can additionally need [contact terms in a correlation function](../../../../../contact-term-in-a-correlation-function.md), which are important below.

In four dimensions, a [conserved current](../../../../../conserved-current.md) arising as a [Noether current](../../../../../noether-current.md) has classical [mass dimension](../../../../../mass-dimension.md) three. Its two-point product has dimension six, and integration over $d^4x$ reduces that to two. The transverse tensor $k_\mu k_\nu-\delta_{\mu\nu}k^2$ already has dimension two. Thus **the scalar coefficient has dimension zero**:

$$
\boxed{[G_0]=0.}
$$

The assumed vanishing [anomalous dimension](../../../../../anomalous-dimension.md) protects the individual current, but does not remove the logarithmic short-distance divergence of its product with another current.

Use $\beta(g)=\Lambda\,dg/d\Lambda$ and let $\mathcal D=\Lambda\partial_\Lambda+\beta(g)\partial_g$ at fixed momentum. Bare-scale independence gives $\mathcal D G_0=0$ at fixed $\Lambda_0$. Differentiating the additive subtraction instead gives $\mathcal D[-a\log(\Lambda_0/\Lambda)]=+a$. Hence **the renormalized [conserved-current two-point function](../../../../../conserved-current-two-point-function.md) obeys an inhomogeneous equation**:

$$
\boxed{\left(\Lambda\partial_\Lambda+\beta(g)\partial_g\right)G_{\mathrm{ren}}(k^2,g,\Lambda)=a.}
$$

This is the [Callan-Symanzik equation with additive renormalization](../../../../../callan-symanzik-equation-with-additive-renormalization.md). The source comes from a local [contact term in a correlation function](../../../../../contact-term-in-a-correlation-function.md) counterterm, despite the current's zero [anomalous dimension](../../../../../anomalous-dimension.md). A homogeneous equation would miss this contribution.

For $k=\sqrt{k^2}>0$, run the [renormalization scale](../../../../../renormalization-scale.md) from $\Lambda$ to $k$, keeping the physical momentum fixed. Along the [renormalization-group flow](../../../../../renormalization-group-flow.md), $dG_{\mathrm{ren}}/d\log\mu=a$, so

$$
G_{\mathrm{ren}}(k^2,g(\Lambda),\Lambda)=C(g(k))-a\log\frac{k}{\Lambda},\qquad C(g)=G_{\mathrm{ren}}(k^2,g,k).
$$

Dimensional analysis makes $C$ independent of $k$ in this massless problem. [Asymptotic freedom](../../../../../asymptotic-freedom.md) means $g(k)\to0$ as $k/\Lambda\to\infty$. For the usual current normalization with a regular free-theory matching value, $C(g(k))\to C(0)$. Consequently **the leading ultraviolet behaviour at this one-loop subtraction accuracy** is

$$
\boxed{G_{\mathrm{ren}}(k^2,g(\Lambda),\Lambda)=-\frac a2\log\frac{k^2}{\Lambda^2}+C(0)+o(1).}
$$

In particular the leading coefficient is $-a/2$, with its sign fixed by the subtraction convention in the question. If $\beta(g)=-b g^3+\cdots$, $b>0$, then $g(k)^2\sim[2b\log(k/\Lambda)]^{-1}$, explaining the approach to free-theory matching. Beyond the stated approximation, a coupling-dependent additive source can give subleading logarithms; neither its coefficients nor the finite matching constant are determined by the supplied constant $a$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 304](../../paper-304-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
