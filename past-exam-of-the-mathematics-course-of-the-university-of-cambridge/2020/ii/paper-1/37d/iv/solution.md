<h1 id="37d/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Because $u^0=c,dt/d\tau=\gamma c$ is constant, $dt/d\tau=\gamma$. The coordinate speed along the circle is consequently

$$
v=\frac{R|\omega|}{\gamma},
$$

so

$$
\boxed{R(v)=\frac{\gamma(v)v}{|\omega|}
=\frac{\gamma(v)mv}{|q|B}.}
$$

For the convention in the question, take $qB>0$, so $\omega>0$ and $\Delta\tau=2\pi/\omega$.

On the circular solution, the free part of the [relativistic charged-particle action](../../../../../../relativistic-charged-particle-action.md) is

$$
S_{\rm free}=-mc^2\Delta\tau=-\frac{2\pi mc^2}{\omega}.
$$

In the gauge $A_y=Bx$, the interaction is the closed [line integral](../../../../../../line-integral.md)

$$
S_{\rm int}=q\oint A_\mu dx^\mu
=qB\oint x\,dy.
$$

The orbit is clockwise for $qB>0$, so $\oint x\,dy=-\pi R^2$. Thus

$$
S_{\rm int}=-\pi qBR^2
=-\frac{\pi m\gamma^2v^2}{\omega}.
$$

Combining the two terms and using $\gamma^2v^2=c^2(\gamma^2-1)$ gives the [charged-particle action over one relativistic cyclotron orbit](../../../../../../charged-particle-action-over-one-relativistic-cyclotron-orbit.md)

$$
\boxed{
S(v)=-\frac{\pi m}{\omega}\left(2c^2+\gamma(v)^2v^2\right)
=-\frac{\pi mc^2}{\omega}\left(1+\gamma(v)^2\right).
}
$$

Although the intermediate magnetic line integral depends on the chosen [magnetic vector potential](../../../../../../magnetic-vector-potential.md), the closed-orbit result is [gauge invariant](../../../../../../gauge-transformation.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [37D](../../37d.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
