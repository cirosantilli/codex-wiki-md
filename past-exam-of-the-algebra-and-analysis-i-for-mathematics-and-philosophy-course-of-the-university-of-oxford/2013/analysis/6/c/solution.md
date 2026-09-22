<h1 id="analysis/6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The complex sine has simple zeros exactly at $z=k\pi$, $k\in\mathbb Z$, because $\sin(k\pi)=0$ and $\cos(k\pi)=(-1)^k\neq0$. Hence the denominator has a zero of order three at each of these points and nowhere else.

At $0$, the numerator has order two, so the quotient has a [simple pole](../../../../../simple-pole.md). Indeed its leading term is $-\pi^4/z$. At $\pi$, the numerator has order one, so there is a [pole](../../../../../pole.md) of order two. At $-\pi$, the numerator has order three, cancelling the denominator's order-three zero, so the singularity is removable. Its extension value is

$$
\lim_{z\to-\pi}\frac{z^2(z-\pi)(z+\pi)^3}{\sin^3z}
=\frac{(-\pi)^2(-2\pi)}{\cos^3(-\pi)}=2\pi^3.
$$

At every remaining $k\pi$, the numerator is nonzero, giving a [pole](../../../../../pole.md) of order three. Thus the complete finite-plane classification is

$$
\boxed{\begin{array}{c|c}
z&\text{classification}\\\hline
0&\text{pole of order }1\\
\pi&\text{pole of order }2\\
-\pi&\text{removable, extension value }2\pi^3\\
k\pi,\quad k\in\mathbb Z\setminus\{-1,0,1\}&\text{pole of order }3
\end{array}}
$$

Away from this discrete set the denominator is nonzero, so the quotient is holomorphic.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Analysis](../../../analysis.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra and analysis I for mathematics and philosophy course of the University of Oxford](../../../../split.md)
6. [Algebra and analysis I for mathematics and philosophy course of the University of Oxford](../../../../../algebra-and-analysis-i-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Mathematics and philosophy course of the University of Oxford](../../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
