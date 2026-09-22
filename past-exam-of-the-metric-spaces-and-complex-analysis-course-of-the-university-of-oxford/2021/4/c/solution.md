<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

For $a\ne b$, integrate

$$
F(z)=\frac{e^{iz}}{(z^2+a^2)(z^2+b^2)}
$$

along the [contour](../../../../complex-integration-contour.md) consisting of $[-R,R]$ and the upper [semicircle](../../../../semicircle.md), with [positive orientation of a contour](../../../../positive-orientation-of-a-contour.md) and $R>\max\{a,b\}$. Its enclosed [simple poles](../../../../simple-pole.md) are $ia$ and $ib$, with [residues](../../../../residue.md)

$$
\operatorname{Res}(F,ia)=\frac{e^{-a}}{2ia(b^2-a^2)},\qquad
\operatorname{Res}(F,ib)=\frac{e^{-b}}{2ib(a^2-b^2)}.
$$

On the upper [semicircle](../../../../semicircle.md), $|e^{iz}|=e^{-\operatorname{Im}z}\leq1$. The [reverse triangle inequality](../../../../reverse-triangle-inequality.md) gives $|z^2+a^2|\geq R^2-a^2$ and $|z^2+b^2|\geq R^2-b^2$, so the [estimation lemma](../../../../estimation-lemma.md) gives

$$
\left|\int_{\mathrm{arc}}F(z)\,dz\right|\leq\frac{\pi R}{(R^2-a^2)(R^2-b^2)}\longrightarrow0.
$$

The [integral](../../../../integral-split.md) along the [real axis](../../../../real-axis.md) is absolutely convergent: the denominator stays nonzero on bounded real [intervals](../../../../interval-mathematics.md), and the integrand is $O(x^{-4})$ at infinity. The [residue theorem](../../../../residue-theorem.md) therefore gives

$$
\int_{-\infty}^{\infty}\frac{e^{ix}}{(x^2+a^2)(x^2+b^2)}\,dx
=\frac{\pi}{a^2-b^2}\left(\frac{e^{-b}}b-\frac{e^{-a}}a\right).
$$

Take [real parts](../../../../real-part.md). The real integrand is an [even function](../../../../even-function.md), so

$$
\boxed{\int_0^\infty\frac{\cos x}{(x^2+a^2)(x^2+b^2)}\,dx
=\frac{\pi}{2(a^2-b^2)}\left(\frac{e^{-b}}b-\frac{e^{-a}}a\right).}
$$

To include $a=b$, fix $a>0$ and let $b\to a$. For $a/2\leq b\leq3a/2$, the [absolute value](../../../../absolute-value.md) of the integrand is bounded by

$$
\frac1{(x^2+a^2)(x^2+a^2/4)},
$$

an integrable [function](../../../../function-split.md) on $[0,\infty)$. The [dominated convergence theorem](../../../../dominated-convergence-theorem.md) justifies passing the limit under the [integral](../../../../integral-split.md). If $h(t)=e^{-t}/t$, then $h'(a)=-e^{-a}(a+1)/a^2$, and

$$
\lim_{b\to a}\frac{h(b)-h(a)}{a^2-b^2}=-\frac{h'(a)}{2a}=\frac{e^{-a}(a+1)}{2a^3}.
$$

Hence

$$
\boxed{\int_0^\infty\frac{\cos x}{(x^2+a^2)^2}\,dx=\frac{\pi e^{-a}(a+1)}{4a^3}.}
$$

## ↑ Ancestors (12)

1. [c](../c.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
