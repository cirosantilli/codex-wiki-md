<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The initial [function](../../../../../function-split.md) is [odd](../../../../../odd-function.md), so all $a_n$, including $a_0$, vanish. Set $k_n=n\pi/L$. For $k_n\ne1$, product-to-sum and [integration by parts](../../../../../integration-by-parts.md) give

$$
\int_0^L\sin x\sin(k_nx)\,dx=\frac{(-1)^nk_n\sin L}{1-k_n^2},\qquad\int_0^Lx\sin(k_nx)\,dx=-\frac{L(-1)^n}{k_n}.
$$

Consequently the coefficients of the [periodic sine with an endpoint-correcting linear term](../../../../../periodic-sine-with-an-endpoint-correcting-linear-term.md) are

$$
\boxed{b_n=\frac{2(-1)^n\sin L}{n\pi[1-(n\pi/L)^2]}.}
$$

Insert them into the sine terms of the preceding solution. If $L=m\pi$ for a positive [integer](../../../../../integer-split.md) $m$, the original initial profile is simply $\sin x$, with $k_m=1$. The apparent $0/0$ in the displayed coefficient has removable [limit](../../../../../limit-of-a-function.md) $b_m=1$, while $b_n=0$ for $n\ne m$. In that case

$$
\boxed{u(x,t)=e^{-\kappa t}\sin x.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
