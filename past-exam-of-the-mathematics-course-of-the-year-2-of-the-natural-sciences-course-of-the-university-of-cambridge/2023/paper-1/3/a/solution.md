<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Set $L=d^2/dt^2-4$ and choose $L_tG(t,t')=\delta(t-t')$, with the [Green's function](../../../../../green-s-function-split.md) decaying at both ends. Away from the source, its homogeneous solutions are $e^{\pm2t}$. Decay at each end and continuity at $t=t'$ therefore give $G=C e^{-2|t-t'|}$. Integrating its equation across the source gives a unit jump in its first [derivative](../../../../../derivative.md):

$$
\partial_tG(t'^+,t')-\partial_tG(t'^-,t')=-2C-2C=1.
$$

Thus

$$
\boxed{A=-2,\qquad C=-\frac14,\qquad G(t,t')=-\frac14e^{-2|t-t'|}.}
$$

The solution of the [boundary value problem](../../../../../boundary-value-problem-split.md) is the [convolution](../../../../../convolution.md)

$$
\boxed{x(t)=-\frac14\int_{-\infty}^{\infty}e^{-2|t-\tau|}f(\tau)\,d\tau.}
$$

There is no extra homogeneous term: no nonzero combination of $e^{2t},e^{-2t}$ decays at both infinities. The forcing must of course permit the imposed decay; integrable $f$, including part (b), is sufficient. Literally arbitrary forcing need not do so: constant nonzero forcing admits no solution vanishing at both ends.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
