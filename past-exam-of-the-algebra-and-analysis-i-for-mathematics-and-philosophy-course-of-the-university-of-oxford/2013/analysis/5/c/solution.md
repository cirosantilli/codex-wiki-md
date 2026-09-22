<h1 id="analysis/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the branch from part (b) and close the real interval $[-R,R]$ with the upper semicircle, oriented counterclockwise. For $\operatorname{Im}z\geq0$, the number $z+i\alpha$ has positive imaginary part, so the numerator is a [holomorphic logarithm](../../../../../holomorphic-logarithm.md) throughout a neighbourhood of the contour and its interior. The branch point $-i\alpha$ lies strictly below the contour. The only enclosed [pole](../../../../../pole.md) of

$$
H(z)=\frac{\operatorname{Log}(z+i\alpha)}{z^2+\beta^2}
$$

is the [simple pole](../../../../../simple-pole.md) at $i\beta$, with [residue](../../../../../residue.md)

$$
\operatorname{Res}_{z=i\beta}H=\frac{\operatorname{Log}(i(\alpha+\beta))}{2i\beta}
=\frac{\log(\alpha+\beta)+i\pi/2}{2i\beta}.
$$

To justify discarding the arc, take $R>\max\{\beta,\alpha+1\}$. On it, $|z+i\alpha|$ lies between $R-\alpha$ and $R+\alpha$, and the argument has bounded absolute value. Hence

$$
\left|\int_{\text{arc}}H(z)\,dz\right|
\leq\frac{\pi R\{\log(R+\alpha)+3\pi/2\}}{R^2-\beta^2}\longrightarrow0.
$$

The real-axis integral is absolutely convergent, since its integrand is $O(\log|x|/x^2)$ at infinity and has no real singularities. The [residue theorem](../../../../../residue-theorem.md) therefore gives

$$
\boxed{\int_{-\infty}^{\infty}\frac{\operatorname{Log}(x+i\alpha)}{x^2+\beta^2}\,dx
=\frac\pi\beta\log(\alpha+\beta)+\frac{i\pi^2}{2\beta}.}
$$

Finally, $\operatorname{Re}\operatorname{Log}(x+i\alpha)=\tfrac12\log(x^2+\alpha^2)$. Taking twice the real part yields

$$
\boxed{\int_{-\infty}^{\infty}\frac{\log(x^2+\alpha^2)}{x^2+\beta^2}\,dx
=\frac{2\pi}{\beta}\log(\alpha+\beta).}
$$

The branch choice affects the first integral's imaginary part; the second integral is real and independent of that choice.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
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
