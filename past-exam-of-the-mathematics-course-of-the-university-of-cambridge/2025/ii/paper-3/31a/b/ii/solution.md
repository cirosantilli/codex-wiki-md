<h1 id="31a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The polar equations are

$$
\dot r
=\frac{x\dot x+y\dot y}{r}
=r(\mu+\lambda r^2-r^4),
\qquad
\dot\theta
=\frac{x\dot y-y\dot x}{r^2}=1.
$$

Every positive zero of the radial factor is therefore a circular periodic orbit of period $2\pi$. Writing $s=r^2$, the equation is

$$
s^2-\lambda s-\mu=0,
\qquad
s_\pm=\frac{\lambda\pm\sqrt{\lambda^2+4\mu}}2.
$$

The resulting count is

$$
\begin{array}{c|c}
\text{parameter range}&\text{positive periodic orbits}\\ \hline
\mu<-\lambda^2/4&0\\
\mu=-\lambda^2/4&1\text{ double orbit}\\
-\lambda^2/4<\mu<0&2\\
\mu\geq0&1.
\end{array}
$$

For the two-orbit range, $s_-<\lambda/2<s_+$. Differentiating the radial vector field at an orbit gives

$$
\left.\frac{d\dot r}{dr}\right|_{r^2=s}
=2s(\lambda-2s),
$$

so the inner orbit is unstable and the outer orbit is stable. At

$$
\boxed{\mu=-\lambda^2/4}
$$

they meet in a [saddle-node bifurcation of periodic orbits](../../../../../../../saddle-node-bifurcation-of-periodic-orbits.md). At

$$
\boxed{\mu=0}
$$

the inner orbit shrinks into the origin, giving the second bifurcation.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [31A](../../../31a.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
