<h1 id="34a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the mostly-plus metric, so $\Box$ reduces to $\nabla^2$ for static fields. Seek a [Green function](../../../../../../green-s-function.md) satisfying $(\nabla^2-\lambda^2)G=\delta^{(3)}$. Convolving it with $-\mu_0\mathbf J$ gives the required solution.

For $R>0$, write $G=f(R)/R$. The homogeneous equation is $f''-\lambda^2f=0$. Decay discards the growing exponential, while the normalization at the origin follows from $\nabla^2(1/R)=-4\pi\delta^{(3)}$. Therefore **for every $\lambda\geq0$**,

$$
\boxed{G(R)=-\frac{e^{-\lambda R}}{4\pi R},\qquad \mathbf A(\mathbf x)=\frac{\mu_0}{4\pi}\int\frac{e^{-\lambda|\mathbf x-\mathbf x'|}}{|\mathbf x-\mathbf x'|}\mathbf J(\mathbf x')\,d^3x'.}
$$

The $1/R$ singularity fixes the delta coefficient; the extra factor is smooth to leading order at zero. For a conserved localized static current, integration by parts also gives $\nabla\cdot\mathbf A=0$, as required by the constraint.

At $\lambda=0$ the far field has algebraic multipole decay; for an ordinary localized steady current the vector potential starts at dipole order. At $\lambda>0$ the [Yukawa potential](../../../../../../yukawa-potential.md) gives exponential suppression on length scale $\lambda^{-1}$, with an overall bound of order $e^{-\lambda|\mathbf x|}/|\mathbf x|$ for bounded source support.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [34A](../../34a.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
