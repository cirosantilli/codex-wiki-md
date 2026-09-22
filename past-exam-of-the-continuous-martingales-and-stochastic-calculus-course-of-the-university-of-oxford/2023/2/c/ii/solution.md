<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret the ordered [Iterated Itô integral](../../../../../iterated-ito-integral.md) recursively as $I_0(t)=1$ and

$$
I_n(t)=\int_0^t I_{n-1}(s)\,dB_s.
$$

The diagonal boundary of the ordered region does not affect this recursive definition. For $n=1$, $I_1(t)=B_t$. For $n=2$, part (a)(iii) gives $I_2(t)=\tfrac12(B_t^2-t)$. For $n=3$, use parts (b)(ii) and (b)(iii):

$$
\begin{aligned}
I_3(t)
&=\frac12\int_0^t(B_s^2-s)\,dB_s\\
&=\frac12\left(\frac13B_t^3-\int_0^tB_s\,ds
-tB_t+\int_0^tB_s\,ds\right)
=\frac16(B_t^3-3tB_t).
\end{aligned}
$$

Thus the three [Probabilists' Hermite polynomials](../../../../../probabilists-hermite-polynomial.md) give

$$
\boxed{\begin{aligned}
1!I_1(t)&=B_t=t^{1/2}h_1(B_t/\sqrt t),\\
2!I_2(t)&=B_t^2-t=t\,h_2(B_t/\sqrt t),\\
3!I_3(t)&=B_t^3-3tB_t=t^{3/2}h_3(B_t/\sqrt t).
\end{aligned}}
$$

The right sides are interpreted as their polynomial extensions at $t=0$. These [space-time Hermite polynomials](../../../../../space-time-hermite-polynomial.md) arise here directly from ordered [Iterated Itô integrals](../../../../../iterated-ito-integral.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the continuous martingales and stochastic calculus course of the University of Oxford](../../../../split.md)
6. [Continuous martingales and stochastic calculus course of the University of Oxford](../../../../../continuous-martingales-and-stochastic-calculus-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
