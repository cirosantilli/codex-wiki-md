<h1 id="7a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $t<0$ both inputs vanish. Eliminating $y$ gives $x''+4x=0$, and the data at $t=-\pi$ give

$$
x(t)=\cos2t.
$$

For all $t$, differentiating the first equation and using the second gives

$$
x''+4x=\delta(t)-2H(t-\pi).
$$

Thus $x$ is continuous at zero while $x'$ jumps by one. For $t>0$ the resulting solution is

$$
x(t)=\cos2t+\frac12\sin2t
+\frac12H(t-\pi)(\cos2t-1).
$$

Since $\cos2t=1-2\sin^2t$, this is

$$
x(t)=\frac12\sin2t+1+q(t)\sin^2t,
$$

where

$$
q(t)=\begin{cases}-2,&0<t<\pi,\\-3,&t\geq\pi.
\end{cases}
$$

**Thus $a=1/2$, $b=1$, and the sketch of $q$ is a downward unit step at $t=\pi$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7A](../../7a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
