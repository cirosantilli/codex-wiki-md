<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the two semi-infinite cracks, choose instead

$$
\chi(z)=\sqrt{a^2-z^2},\qquad \chi(x)>0\quad(-a<x<a),
$$

with cuts on the two crack segments. Approaching from above gives

$$
\chi^+(t)=\begin{cases}-i\sqrt{t^2-a^2},&t>a,\\+i\sqrt{t^2-a^2},&t<-a,\end{cases}\qquad \chi^-(t)=-\chi^+(t).
$$

These opposite signs on the two cracks are essential. Multiplying the [Hilbert problem for an antiplane crack](../../../../../../hilbert-problem-for-an-antiplane-crack.md) by $\chi$ gives

$$
H^+-H^-=\begin{cases}+2i\sqrt{t^2-a^2}\,p(t),&t>a,\\-2i\sqrt{t^2-a^2}\,p(t),&t<-a.\end{cases}
$$

The [Sokhotski–Plemelj theorem](../../../../../../sokhotski-plemelj-theorem.md) therefore yields the [antiplane ligament Cauchy solution](../../../../../../antiplane-ligament-cauchy-solution.md)

$$
H(z)=\frac1\pi\left(\int_a^\infty-\int_{-\infty}^{-a}\right)\frac{\sqrt{t^2-a^2}\,p(t)}{t-z}\,dt,\qquad G(z)=\frac{H(z)}{\chi(z)}.
$$

For $-a<x=x_1<a$, $\chi(x)=\sqrt{a^2-x^2}$ and the kernel has no pole on either crack. Hence

$$
\boxed{\sigma_{23}(x,0)+i\sigma_{13}(x,0)=\frac1{\pi\sqrt{a^2-x^2}}\left(\int_a^\infty-\int_{-\infty}^{-a}\right)\frac{\sqrt{t^2-a^2}\,\sigma_{23}^A(t,0)}{t-x}\,dt.}
$$

Again this is the additional stress, and $\sigma_{13}=0$ on the intact ligament. The integrals have the [Cauchy principal value](../../../../../../cauchy-principal-value.md) interpretation wherever required, and their convergence at infinity is assumed. For a point on the right crack, the upper value of $H$ has imaginary part $+\sqrt{t^2-a^2}p(t)$; division by $-i\sqrt{t^2-a^2}$ gives real part $-p(t)$. On the left crack both signs reverse and the same cancellation follows.

The homogeneous ambiguity here is physically different from the finite-crack displacement period. A real term

$$
G_{\mathrm{hom}}(z)=\frac{C}{\sqrt{a^2-z^2}}
$$

has zero real traction on the crack faces but adds ligament shear with resultant

$$
\int_{-a}^a\frac{C}{\sqrt{a^2-x^2}}\,dx=\pi C.
$$

Its potential is $(C/\mu)\arcsin(z/a)$, producing logarithmic displacement growth at infinity. Thus it represents a separately imposed load transfer between the two sides, even though its stress tends to zero pointwise at infinity. The induced correction with no added remote resultant selects $C=0$, giving the boxed formula. Merely requiring pointwise decay of stress would not fix this constant; the far-field load normalization is needed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
