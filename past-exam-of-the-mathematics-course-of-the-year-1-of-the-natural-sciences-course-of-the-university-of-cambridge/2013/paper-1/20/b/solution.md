<h1 id="20/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The triangular roof has height $(w/2)\tan\theta$ and two slopes of length $(w/2)\sec\theta$. Hence the area constraint and cost are

$$
A=wh+\frac{w^2}{4}\tan\theta,
\qquad C=2\alpha h+\beta w\sec\theta.
$$

The wall height is fixed, so its cost is constant. Assume the physical case $A,h,\beta>0$. Minimize $C$ subject to the area constraint by [Lagrange multipliers](../../../../../lagrange-multiplier.md):

$$
\beta\sec\theta=\lambda\left(h+\frac w2\tan\theta\right),\qquad
\beta w\sec\theta\tan\theta=\lambda\frac{w^2}{4}\sec^2\theta.
$$

Eliminating the positive common factors gives

$$
w\sec^2\theta=4h\tan\theta+2w\tan^2\theta,
\qquad w(1-\tan^2\theta)=4h\tan\theta.
$$

Thus the optimum has $0<\theta<\pi/4$ and

$$
\boxed{2\tan2\theta=\frac wh.}
$$

Set $D=A-wh>0$, so the area constraint gives $\tan\theta=4D/w^2$. Substituting into the preceding equation and multiplying by $w^3$ yields $w^4-16D^2=16hwD$. Therefore

$$
\boxed{w^4=16D(D+wh)=16A(A-wh).}
$$

For a global check, the square of the total roof length is

$$
Q(w)=w^2+\frac{16(A-wh)^2}{w^2},\qquad0<w<A/h.
$$

Its [derivative](../../../../../derivative.md) has the sign of $P(w)=w^4+16Ahw-16A^2$. Since $P'(w)>0$, $P(0)<0$ and $P(A/h)>0$, it has one root in this interval, with $Q$ decreasing before that root and increasing afterwards. This proves the unique global minimum, rather than merely a stationary design. The [minimum roof length at fixed wall height and cross-sectional area](../../../../../minimum-roof-length-at-fixed-wall-height-and-cross-sectional-area.md) is independent of $\alpha$ and of the positive factor $\beta$. If $\beta=0$, every feasible shape has equal cost; the displayed conditions then describe a possible minimizer but are not necessary.

<a id="20/b/image-an-original-cross-section-construction-showing-the-fixed-wall-height-roof-rise-and-sloping-lengths"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2013/paper-1-roof-optimization.png)

**[Figure 6](#20/b/image-an-original-cross-section-construction-showing-the-fixed-wall-height-roof-rise-and-sloping-lengths). An original cross-section construction showing the fixed wall height, roof rise and sloping lengths**.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [20](../../20.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
