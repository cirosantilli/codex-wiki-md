<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

Let $r$ be distance from the common centre. By [Gauss's law](../../../../../gauss-s-law.md), the [electric field](../../../../../electric-field.md) is radial and equals

$$
\boxed{
\mathbf E(r)=
\begin{cases}
0,&0\le r<R,\\[2mm]
\dfrac{Q_1}{4\pi\epsilon_0r^2}\,\widehat{\mathbf r},
&R<r<2R,\\[3mm]
\dfrac{Q_1+Q_2}{4\pi\epsilon_0r^2}\,\widehat{\mathbf r},
&r>2R.
\end{cases}}
$$

Taking the [electric potential](../../../../../electric-potential.md) to vanish at infinity and requiring continuity across each shell gives

$$
\boxed{
\Phi(r)=\frac1{4\pi\epsilon_0}
\begin{cases}
\dfrac{Q_1}{R}+\dfrac{Q_2}{2R},&0\le r\le R,\\[3mm]
\dfrac{Q_1}{r}+\dfrac{Q_2}{2R},&R\le r\le2R,\\[3mm]
\dfrac{Q_1+Q_2}{r},&r\ge2R.
\end{cases}}
$$

The [electrostatic energy](../../../../../electrostatic-energy.md) is the integral of the electric-field energy density:

$$
U=\frac{\epsilon_0}{2}\int_{\mathbb R^3}|\mathbf E|^2\,dV.
$$

Only the two nonzero-field regions contribute, so

$$
U=\frac{Q_1^2}{8\pi\epsilon_0}
\int_R^{2R}\frac{dr}{r^2}
+\frac{(Q_1+Q_2)^2}{8\pi\epsilon_0}
\int_{2R}^{\infty}\frac{dr}{r^2}.
$$

Therefore

$$
\boxed{U
=\frac{Q_1^2+(Q_1+Q_2)^2}{16\pi\epsilon_0R}
=\frac{2Q_1^2+2Q_1Q_2+Q_2^2}{16\pi\epsilon_0R}}.
$$

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
