<h1 id="analysis/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [residue](../../../../residue.md) at $a$ is the coefficient $c_{-1}$ of $(z-a)^{-1}$ in the [Laurent series](../../../../laurent-series.md). A [simple pole](../../../../simple-pole.md) means $f(z)=c_{-1}/(z-a)+h(z)$ near $a$, with $c_{-1}\neq0$ and $h$ holomorphic across $a$.

For the specified positively oriented arc, direct parametrization gives $\int_{\gamma_\epsilon}(z-a)^{-1}\,dz=i(\beta-\alpha)$. The remaining integral is bounded by $\epsilon(\beta-\alpha)\sup|h|$, which tends to zero because $h$ is bounded near $a$. Therefore

$$
\boxed{\int_{\gamma_\epsilon}f(z)\,dz\longrightarrow i(\beta-\alpha)\operatorname{res}(f;a).}
$$

The simple-pole hypothesis matters. For $f(z)=(z-a)^{-2}$, with $\alpha=0$, $\beta=\pi$, the [residue](../../../../residue.md) is zero but

$$
\int_{\gamma_\epsilon}\frac{dz}{(z-a)^2}=\frac2\epsilon\longrightarrow\infty.
$$

For the particular function, expanding the exponential gives

$$
1+iz-e^{iz}=\frac{z^2}{2}+\frac{iz^3}{6}+O(z^4),\qquad
f(z)=\frac1{2z}+\frac i6+O(z).
$$

Thus $\boxed{\operatorname{res}(f;0)=1/2}$, and the pole is simple. On the large upper semicircle, $|e^{iz}|\leq1$, giving

$$
\left|\int_{\Gamma_R}f(z)\,dz\right|
\leq\pi R\frac{R+2}{R^3}=\frac{\pi(R+2)}{R^2}\longrightarrow0.
$$

Close the real-axis path from $-R$ to $-\epsilon$ and $\epsilon$ to $R$ by this upper arc and a clockwise upper indentation at zero. The function is holomorphic in the indented region, so the sum of all four integrals is zero. The clockwise indentation tends to $-i\pi/2$. For real $x$,

$$
f(x)=\frac{1-\cos x}{x^3}+i\frac{x-\sin x}{x^3}.
$$

The real part is odd and cancels on the symmetric real pieces; the imaginary part is even. Its integral converges since $(x-\sin x)/x^3\to1/6$ at zero and is $O(x^{-2})$ at infinity. Letting $\epsilon\to0$ and $R\to\infty$ therefore yields $2iI-i\pi/2=0$, where $I$ is the requested real integral. Hence

$$
\boxed{\int_0^\infty\frac{x-\sin x}{x^3}\,dx=\frac\pi4.}
$$

## ↑ Ancestors (12)

1. [5](../5.md)
2. [Analysis](../../analysis.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
