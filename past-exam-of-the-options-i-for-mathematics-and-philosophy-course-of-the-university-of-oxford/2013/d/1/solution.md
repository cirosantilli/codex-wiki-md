<h1 id="d/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a nonnegative [measurable function](../../../../measurable-function.md), the [Lebesgue integral](../../../../lebesgue-integral.md) is defined through nonnegative [simple functions](../../../../simple-function.md):

$$
\boxed{\int_{\mathbb R}f\,dx=\sup\left\{\int_{\mathbb R}s\,dx:s\text{ simple},\ 0\leq s\leq f\right\}.}
$$

The value may be infinite. A real measurable $g$ is [Lebesgue integrable](../../../../lebesgue-integrable-function.md) when $\int|g|dx<\infty$; then $\int g=\int g^+-\int g^-$, where $g^+=\max(g,0)$ and $g^-=\max(-g,0)$.

If $|g|\leq h$, every simple function below $|g|$ is also below $h$. Taking the defining suprema proves [monotonicity of the Lebesgue integral](../../../../monotonicity-of-the-lebesgue-integral.md):

$$
0\leq\int|g|\,dx\leq\int h\,dx<\infty.
$$

Hence **$g$ is integrable**, and both its positive and negative parts have finite [integrals](../../../../integral-split.md).

The oscillatory function $k$ is measurable because it is continuous off the singleton $\{0\}$ and has a specified value there. The elementary bounds $|\sin u|\leq\min(1,|u|)$ give the integrable majorant

$$
|k(x)|\leq H(x)=\begin{cases}1,&|x|\leq1,\\|x|^{-3},&|x|>1.\end{cases}
$$

Indeed, $\int H=2+2\int_1^\infty x^{-3}dx=3$. The comparison just proved gives $\int|k|\leq3$, so **$k$ is Lebesgue integrable over the whole real line**, despite its oscillations near zero. Its [odd](../../../../odd-function.md) symmetry also gives $\int k=0$, now legitimately because absolute integrability has been established.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [D](../../d.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options I for mathematics and philosophy course of the University of Oxford](../../../split.md)
5. [Options I for mathematics and philosophy course of the University of Oxford](../../../../options-i-for-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and philosophy course of the University of Oxford](../../../../year-2-of-the-mathematics-and-philosophy-course-of-the-university-of-oxford.md)
7. [Mathematics and philosophy course of the University of Oxford](../../../../mathematics-and-philosophy-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
