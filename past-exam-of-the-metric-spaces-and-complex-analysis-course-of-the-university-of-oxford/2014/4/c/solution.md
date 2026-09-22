<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $z\notin\mathbb Z$, integrate

$$
F(w)=\frac{\pi\cot(\pi w)}{w^2-z^2}
$$

counterclockwise around the specified square of half-side $R_N=N+1/2$, choosing $N>|z|$. The integer poles inside it are $-N,\ldots,N$, and their residues are $1/(n^2-z^2)$ because $\pi\cot(\pi w)$ has [residue](../../../../residue.md) one at each integer.

The two other possible poles are $w=z$ and $w=-z$. Their residues are each $\pi\cot(\pi z)/(2z)$, hence sum to $\pi\cot(\pi z)/z$. This formula still applies when the numerator vanishes and a possible [pole](../../../../pole.md) is removable. The [residue theorem](../../../../residue-theorem.md) gives

$$
\frac1{2\pi i}\int_{\Gamma_N}F(w)\,dw
=\sum_{n=-N}^N\frac1{n^2-z^2}+\frac{\pi\cot(\pi z)}z.
$$

On the square, $|w|\geq R_N$, its perimeter is $8R_N$, and the supplied cotangent bound gives

$$
\left|\int_{\Gamma_N}F(w)\,dw\right|
\leq\frac{8CR_N}{R_N^2-|z|^2}\longrightarrow0.
$$

The series converges absolutely by part (b), so its symmetric partial sums have the same limit as the full sum. Therefore

$$
\boxed{\sum_{n=-\infty}^{\infty}\frac1{n^2-z^2}=-\frac{\pi\cot(\pi z)}z=-\frac\pi{z\tan(\pi z)},\qquad z\notin\mathbb Z.}
$$

At half-integers the cotangent form makes the value zero explicit; the reciprocal-tangent notation is understood by its [continuous](../../../../continuous-function.md) extension there. The [cotangent contour summation](../../../../cotangent-contour-summation.md) rests on the [contour](../../../../complex-integration-contour.md) estimate, not only on formally matching poles.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
