<h1 id="question-6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $0<y<\pi$, define $J(y)=\int_0^\pi u_y(x,y)\,dx$. Differentiate under the [integral](../../../../../../integral-split.md) and use [Laplace's equation](../../../../../../laplace-equation.md):

$$
J'(y)=\int_0^\pi u_{yy}(x,y)\,dx
=-\int_0^\pi u_{xx}(x,y)\,dx
=-\bigl[u_x(\pi,y)-u_x(0,y)\bigr]=0.
$$

Thus $J$ is constant. The top [Neumann boundary condition](../../../../../../neumann-boundary-condition.md) gives $J(\pi)=0$, so

$$
\boxed{\int_0^\pi u_y(x,y^*)\,dx=0,\qquad0<y^*<\pi.}
$$

For the included endpoint $y^*=0$, the [integral](../../../../../../integral-split.md) is interpreted as an [improper integral](../../../../../../improper-integral.md) at the bottom corners if necessary. The [Fourier series](../../../../../../fourier-series-split.md) constructed in [c](../c.md) gives, on $0<x<\pi$,

$$
u_y(x,0)=-2\log(2\sin x)
+2\sum_{m=1}^\infty\frac{\tanh(2m\pi)-1}{m}\cos(2mx).
$$

The second [series](../../../../../../series-mathematics.md) is absolutely and uniformly convergent; the first term has only integrable [logarithmic singularities](../../../../../../logarithmic-singularity.md). Its [integral](../../../../../../integral-split.md) is zero since $\int_0^\pi\log(2\sin x)\,dx=0$, while every [cosine](../../../../../../cosine.md) term also has zero [integral](../../../../../../integral-split.md). This proves the endpoint as well:

$$
\boxed{\int_0^\pi u_y(x,y^*)\,dx=0,\qquad0\leq y^*<\pi.}
$$

For completeness, the logarithmic [integral](../../../../../../integral-split.md) follows without any endpoint differentiation. Put $I=\int_0^{\pi/2}\log(\sin x)\,dx$ and substitute $x\mapsto\pi/2-x$ to obtain $I=\int_0^{\pi/2}\log(\cos x)\,dx$. Adding and using $\sin x\cos x=\sin(2x)/2$ gives $2I=I-(\pi/2)\log2$, hence $I=-(\pi/2)\log2$ and the required full-interval result.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Question 6](../../question-6.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
