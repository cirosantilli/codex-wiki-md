<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For the [travelling wave](../../../../travelling-wave.md) $\xi=s+ct$, continuity gives $(ch+hu)'=0$. The upstream state fixes the constant as $1+c$, hence

$$
\boxed{u=-c+\frac{1+c}{h},\qquad u'=-\frac{1+c}{h^2}h'.}
$$

Substituting in [momentum](../../../../momentum-split.md) yields

$$
-\frac{F^2(1+c)^2}{h^3}h'=1-\frac{(1+c-ch)^2}{h^3}-h',
$$

so

$$
\boxed{h'=\frac{h^3-(1+c-ch)^2}{h^3-(1+c)^2F^2}.}
$$

A constant downstream state $H=h_+>1$ requires $H^3=(1+c-cH)^2$. The positive square-root choice would give $c<0$, so the upstream-moving [wave](../../../../wave-split.md) uses $1+c-cH=-H^{3/2}$. Thus

$$
\boxed{c=\frac{H^{3/2}+1}{H-1},\qquad u(H)=-\sqrt H.}
$$

The downstream flow reverses. Where the numerator is positive in $1<h<H$, a smooth increasing profile requires a positive denominator. Its minimum occurs at $h=1$, giving

$$
1-(1+c)^2F^2>0,\qquad\boxed{F<\frac1{1+c}=\frac{H-1}{H+H^{3/2}}.}
$$

Equality does not give the prescribed asymptotic upstream state: cancellation of the two simple zeros at $h=1$ leaves a nonzero slope there. For the strict inequality, separation of variables constructs the monotone profile whenever the numerator remains positive between its endpoint zeros.

**There is an additional restriction hidden in the printed positivity hint.** Put $r=\sqrt h$ and $R=\sqrt H$. Since $c=R+1/(R-1)$, the potentially vanishing factor of the numerator is

$$
h^{3/2}+1+c-ch=(r+1)(r-R)\left(r-\frac{R}{R-1}\right).
$$

The other factor, $h^{3/2}-(1+c-ch)$, is positive for $h>1$. Therefore the asserted positivity throughout $1<h<H$ holds precisely for $1<R\leq2$, that is $1<H\leq4$. For $H>4$, the zero at $h=[R/(R-1)]^2$ intervenes before $H$, preventing the requested monotone connection. For example $H=9$, $c=3.5$, $h=4$ gives $h^3-(1+c-ch)^2=-26.25$. Thus the [smooth upstream tidal-wave admissibility](../../../../smooth-upstream-tidal-wave-admissibility.md) conditions are

$$
\boxed{1<h_+\leq4,\qquad F<\frac{h_+-1}{h_++h_+^{3/2}}.}
$$

At $h_+=4$ the downstream zero is double, giving an algebraic approach; below four the endpoint approaches are exponential. The displayed [Froude number](../../../../froude-number.md) bound is the requested necessary condition, with the source's missing amplitude qualification made explicit.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the mathematics and the environment course of the University of Oxford](../../../split.md)
5. [Mathematics and the environment course of the University of Oxford](../../../../mathematics-and-the-environment-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
