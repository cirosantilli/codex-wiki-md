<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

To repeat [integration by parts](../../../../../integration-by-parts.md) across whole periods, choose [periodic primitives with zero mean](../../../../../periodic-primitive-with-zero-mean.md). Set $h_0=f$, and recursively define

$$
h_{r+1}=Rh_r-\int_0^1Rh_r.
$$

Every $h_r$ has zero mean. Part (i) gives $h_{r+1}'=-h_r$ [almost everywhere](../../../../../almost-everywhere.md), and $h_{r+1}(0)=h_{r+1}(1)$ because $Rh_r$ vanishes at both endpoints. Its [periodic extension](../../../../../periodic-extension.md) is consequently locally an [absolutely continuous function](../../../../../absolutely-continuous-function.md), with no jump at the integers. Part (ii) gives the uniform estimate

$$
\|h_{r+1}\|_{L^1}\leq2\|Rh_r\|_{L^1}\leq\|h_r\|_{L^1}\leq\|f\|_{L^1}.
$$

The [weak derivative](../../../../../weak-derivative.md) identity on the whole line is $D\overline h_{r+1}=-\overline h_r$. After scaling by the integer $j$ and repeating [integration by parts](../../../../../integration-by-parts.md) $N$ times,

$$
\int_0^1\overline f(jx)\phi(x)\,dx
=j^{-N}\int_0^1\overline h_N(jx)\phi^{(N)}(x)\,dx.
$$

The [boundary terms](../../../../../boundary-term.md) vanish because $\phi$ has [compact support](../../../../../compact-support.md) in $(0,1)$. The interval contains exactly $j$ periods, so

$$
\int_0^1|\overline h_N(jx)|\,dx=\int_0^1|h_N(t)|\,dt.
$$

Taking $N=m+1$ therefore yields

$$
\boxed{\left|j^m\int_0^1f_j\phi\right|
\leq j^{-1}\|f\|_{L^1}\|\phi^{(m+1)}\|_\infty\longrightarrow0.}
$$

This [rapid distributional decay of periodic oscillations](../../../../../rapid-distributional-decay-of-periodic-oscillations.md) uses only [integrability](../../../../../integrability.md) of $f$ and smoothness of the [test function](../../../../../test-function.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the distribution theory course of the University of Oxford](../../../../split.md)
6. [Distribution theory course of the University of Oxford](../../../../../distribution-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
