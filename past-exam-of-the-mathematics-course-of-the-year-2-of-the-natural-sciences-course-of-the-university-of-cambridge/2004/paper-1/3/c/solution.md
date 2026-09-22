<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [convolution](../../../../../convolution.md) is $(u*v)(x)=\int_{-\infty}^\infty u(t)v(x-t)dt$. In this transform convention, the [convolution theorem](../../../../../convolution-theorem.md) says $\widehat{u*v}=\widehat u\,\widehat v$, and [Parseval's identity](../../../../../parseval-identity.md) says

$$
\int_{-\infty}^\infty|u(x)|^2dx=\frac1{2\pi}\int_{-\infty}^\infty|\widehat u(k)|^2dk.
$$

To match the integral's scale exactly, set $u=f/2$ and $h(x)=\tfrac12\mathbf1_{[-1,1]}(x)=g(2\pi x)/2$. Then $\widehat u=1/(1+k^2)$ and $\widehat h=\sin k/k$, using the value one at zero. Their convolution is the [box smoothing of a two-sided exponential](../../../../../box-smoothing-of-a-two-sided-exponential.md) with both scales equal to one:

$$
w(x)=(u*h)(x)=\begin{cases}\tfrac12(1-e^{-1}\cosh x),&|x|\leq1,\\\tfrac12\sinh1\,e^{-|x|},&|x|\geq1.\end{cases}
$$

Its transform is precisely $\sin k/[k(1+k^2)]$. Since $w$ is even, [Parseval's identity](../../../../../parseval-identity.md) reduces the requested integral to

$$
J=\pi\left[\int_0^1(1-e^{-1}\cosh x)^2dx+\sinh^2(1)\int_1^\infty e^{-2x}dx\right].
$$

Use $\int_0^1\cosh x\,dx=\sinh1$, $\int_0^1\cosh^2x\,dx=1/2+\sinh2/4$ and $\int_1^\infty e^{-2x}dx=e^{-2}/2$. Simplifying gives

$$
\boxed{J=\frac\pi4(1+5e^{-2}).}
$$

The apparent singularity at $k=0$ is removable, and the integrand decays as $O(|k|^{-6})$, so the integral converges.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
