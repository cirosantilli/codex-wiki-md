<h1 id="8/solution">Solution</h1>

↑ **Parent:** [8](../8.md)

For the zero initial data, the [Green function of an undamped oscillator](../../../../green-function-of-an-undamped-oscillator.md) is $G_0(x,s)=\sin[k(x-s)]/k$ for $0\leq s\leq x$, and zero for $s>x$. It is continuous at the source and its first derivative jumps by one. The resulting [convolution](../../../../convolution.md) is

$$
y(x)=2\int_0^x\sin[k(x-s)]\cos(ks)ds=\boxed{x\sin kx.}
$$

It vanishes together with its first derivative at zero and has the required resonant forcing.

For the two-endpoint problem, write $L=\pi/(6k)$, $a=\min(0,L)$, $b=\max(0,L)$ and $\kappa=|k|$. This covers both signs of the supplied nonzero $k$. Left and right homogeneous solutions are $\sin[\kappa(x-a)]$ and $\sin[\kappa(b-x)]$, with [Wronskian](../../../../wronskian.md) $-\kappa\sin[\kappa(b-a)]$. The [Dirichlet Green function](../../../../dirichlet-green-function.md) is therefore

$$
G_D(x,s)=-\frac{\sin[\kappa(x_<-a)]\sin[\kappa(b-x_>)]}{\kappa\sin[\kappa(b-a)]},\qquad x_<=\min(x,s),\ x_>=\max(x,s).
$$

Its endpoint values are zero and its first derivative jumps by one. Here $\kappa(b-a)=\pi/6$, so the denominator does not vanish. Integrating the constant forcing gives

$$
\boxed{y(x)=\frac{k^2}{2}\int_a^bG_D(x,s)ds=\frac12\left[1-\frac{\cos(k(x-L/2))}{\cos(\pi/12)}\right].}
$$

Equivalently $y=(1-\cos kx)/2+(\sqrt3/2-1)\sin kx$. The negative interior response is consistent with the negative kernel for this short Dirichlet interval.

## ↑ Ancestors (12)

1. [8](../8.md)
2. [Paper 1](../../paper-1-split.md)
3. [2006](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
