<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Treat the channel as prismatic, with horizontal bottom datum $z=0$, uniform cross-sectional velocity, and surface height $h(x,t)$. The area and depth-integrated [hydrostatic pressure](../../../../../../hydrostatic-pressure.md) force divided by density are

$$
A(h)=\int_0^h z^{1/2}\,dz=\frac23h^{3/2},\qquad
P(h)=g\int_0^h(h-z)z^{1/2}\,dz=\frac4{15}gh^{5/2}.
$$

The [prismatic-channel shallow water equations](../../../../../../prismatic-channel-shallow-water-equations.md) are

$$
A_t+(Au)_x=0,\qquad (Au)_t+(Au^2+P)_x=0.
$$

Since $P'(h)=gA(h)$, they become

$$
\boxed{h_t+uh_x+\frac23h\,u_x=0,\qquad
u_t+uu_x+gh_x=0,\qquad c^2=\frac{gA}{A'}=\frac23gh.}
$$

Their two [characteristic speeds](../../../../../../characteristic-speed.md) are $u\pm c$. Using $dc/dh=c/(2h)$ gives the [Riemann invariants](../../../../../../riemann-invariant.md)

$$
\boxed{\frac{dx}{dt}=u\pm c,\qquad \frac{d}{dt}(u\pm3c)=0.}
$$

The factor $3$ replaces the familiar $2$ for a rectangular channel. It comes from the depth-dependent width, not from a different gravitational acceleration.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
