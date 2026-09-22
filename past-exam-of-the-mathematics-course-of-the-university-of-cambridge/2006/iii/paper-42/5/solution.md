<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Write $R(v)=\int_{\mathbb R}v(u)^2\,du$. The [kernel density estimator](../../../../../kernel-density-estimation.md) with bandwidth $h>0$ is

$$
\widehat f_h(x)=\frac1{nh}\sum_{i=1}^nK\!\left(\frac{x-X_i}{h}\right).
$$

Sufficient conditions are that $K$ be a nonnegative symmetric [probability density function](../../../../../probability-density-function.md) with $R(K)<\infty$ and finite nonzero [second moment](../../../../../second-moment.md) $\mu_2(K)=\int u^2K(u)\,du$, and that $h\to0$, $nh\to\infty$. Symmetry and the second-moment assumption give $\int uK(u)\,du=0$. The [expectation](../../../../../expected-value.md) is a [convolution](../../../../../convolution.md):

$$
\mathbb E\widehat f_h(x)=\int K(u)f(x-hu)\,du.
$$

[Taylor's theorem](../../../../../taylor-theorem.md) with integral remainder gives

$$
f(x-hu)=f(x)-hu f'(x)+h^2u^2\int_0^1(1-s)f''(x-shu)\,ds.
$$

The zeroth-order term integrates to $f(x)$, and the [first-order term](../../../../../first-order-term.md) vanishes. The [second derivative](../../../../../second-derivative.md) is bounded and continuous, so [dominated convergence](../../../../../dominated-convergence-theorem.md), with dominating function proportional to $u^2K(u)$, yields

$$
\boxed{\operatorname{Bias}\{\widehat f_h(x)\}=\tfrac12h^2\mu_2(K)f''(x)+o(h^2).}
$$

Combining this with the supplied leading [variance](../../../../../variance-split.md) gives the [asymptotic mean squared error](../../../../../asymptotic-mean-squared-error.md)

$$
\operatorname{AMSE}_x(h)=\frac{R(K)f(x)}{nh}+\frac{\mu_2(K)^2f''(x)^2h^4}4.
$$

When $f(x)>0$ and $f''(x)\ne0$, its derivative is $-R(K)f(x)/(nh^2)+\mu_2(K)^2f''(x)^2h^3$. It changes sign exactly once, giving the [pointwise optimal kernel bandwidth](../../../../../pointwise-optimal-kernel-bandwidth.md)

$$
\boxed{h_{\rm AMSE}(x)=\left\{\frac{R(K)f(x)}{n\mu_2(K)^2f''(x)^2}\right\}^{1/5}.}
$$

**Positivity of $f(x)$ is needed for this positive interior optimum.** The printed condition $f''(x)\ne0$ alone does not ensure it. For instance, $f(x)=x^2\phi(x)$ is a normalized bounded [probability density function](../../../../../probability-density-function.md) with bounded continuous square-integrable [second derivative](../../../../../second-derivative.md), but $f(0)=0$ and $f''(0)=2\phi(0)>0$. At this point the displayed leading [variance](../../../../../variance-split.md) vanishes and the two-term AMSE has no positive interior minimizer; finer [variance](../../../../../variance-split.md) terms are needed to determine an appropriate bandwidth. The formal formula there gives zero, which does not satisfy the bandwidth assumptions.

For integrated error, the same expansion holds in $L^2$: translation [continuity](../../../../../continuous-function.md) of $f''\in L^2$ applied to the integral remainder gives

$$
\|\mathbb E\widehat f_h-f-\tfrac12h^2\mu_2(K)f''\|_2=o(h^2).
$$

Indeed Minkowski's integral inequality bounds the norm of the difference, divided by $h^2$, by the integral of $u^2K(u)\int_0^1(1-s)\|f''(\cdot-shu)-f''\|_2\,ds\,du$; each translated difference tends to zero and is bounded by $2\|f''\|_2$. This proves the claimed integrated [bias expansion](../../../../../bias-expansion.md) without assuming a uniform pointwise remainder over the whole [real line](../../../../../real-line.md).

If $K_h(x)=h^{-1}K(x/h)$, direct integration of the [variance](../../../../../variance-split.md) gives

$$
\int\operatorname{Var}\{\widehat f_h(x)\}\,dx=\frac{R(K)}{nh}-\frac{R(K_h*f)}n.
$$

The last term is $O(n^{-1})$ because $f$ is bounded and integrable, hence square integrable, and [convolution](../../../../../convolution.md) with a [probability density function](../../../../../probability-density-function.md) does not increase its $L^2$ norm. It is negligible compared with $1/(nh)$. Thus the [asymptotic mean integrated squared error](../../../../../asymptotic-mean-integrated-squared-error.md) and its minimizer are

$$
\operatorname{AMISE}(h)=\frac{R(K)}{nh}+\frac{\mu_2(K)^2R(f'')h^4}4,\qquad \boxed{h_{\rm AMISE}=\left\{\frac{R(K)}{n\mu_2(K)^2R(f'')}\right\}^{1/5}.}
$$

Here $R(f'')>0$: otherwise the continuous [second derivative](../../../../../second-derivative.md) vanishes everywhere, making $f$ affine, impossible for a [probability density function](../../../../../probability-density-function.md) on the whole [real line](../../../../../real-line.md).

Now take the [standard normal density](../../../../../standard-normal-density.md) $f=\phi$. Differentiation gives $\phi''(x)=(x^2-1)\phi(x)$. Gaussian integration gives

$$
R(\phi'')=\frac1{2\pi}\int(x^2-1)^2e^{-x^2}\,dx=\frac3{8\sqrt\pi}.
$$

The kernel constants cancel from the bandwidth ratio. At $x\ne\pm1$,

$$
\left(\frac{h_{\rm AMSE}(x)}{h_{\rm AMISE}}\right)^5=\frac{\phi(x)R(\phi'')}{\phi''(x)^2}=\frac{3\sqrt2}{8}\frac{e^{x^2/2}}{(x^2-1)^2}.
$$

Put $t=x^2$. The [logarithmic derivative](../../../../../logarithmic-derivative.md) of $e^{t/2}/(t-1)^2$ is $1/2-2/(t-1)$. On $0\leq t<1$ the function increases, giving its minimum at $t=0$, with value one. On $t>1$ it decreases up to $t=5$ and then increases, giving its minimum $e^{5/2}/16<1$. Thus the [global minimizers](../../../../../global-minimizer.md) are $x=\pm\sqrt5$, and the [normal-density local-to-global bandwidth ratio](../../../../../normal-density-local-to-global-bandwidth-ratio.md) is

$$
\boxed{\inf_{x\ne\pm1}\frac{h_{\rm AMSE}(x)}{h_{\rm AMISE}}=\left(\frac{3\sqrt2 e^{5/2}}{128}\right)^{1/5}=\left(\frac{9e^5}{8192}\right)^{1/10}.}
$$

The ratio diverges at the two [inflection points](../../../../../inflection-point.md) $\pm1$, where the second-order pointwise bias approximation vanishes and needs a higher-order replacement.

<a id="5/image-normal-density-pointwise-bandwidth-relative-to-the-integrated-error-optimum-minima-at-plus-and-minus-square-root-of-five"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-42-bandwidth-ratio.png)

**[Figure 1](#5/image-normal-density-pointwise-bandwidth-relative-to-the-integrated-error-optimum-minima-at-plus-and-minus-square-root-of-five). Normal-density pointwise bandwidth relative to the integrated-error optimum; minima at plus and minus square root of five**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
