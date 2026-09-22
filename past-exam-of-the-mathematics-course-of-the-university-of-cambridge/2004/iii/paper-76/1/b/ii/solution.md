<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The locally integrable function $\log|x|$ defines a [tempered distribution](../../../../../../../tempered-distribution.md). Its [distributional derivative](../../../../../../../distributional-derivative.md) is $\operatorname{PV}(1/x)$: perform [integration by parts](../../../../../../../integration-by-parts.md) outside $(-a,a)$, and observe that the boundary contribution $\log a[\varphi(a)-\varphi(-a)]$ tends to zero. By the [Fourier transform of a derivative](../../../../../../../fourier-transform-of-a-derivative.md) and the preceding result,

$$
ik\widehat{\log|x|}=-i\pi\operatorname{sgn}k.
$$

Division by $|k|$ needs a [finite-part inverse-absolute-value distribution](../../../../../../../finite-part-inverse-absolute-value-distribution.md), since $1/|k|$ is not locally integrable at zero. One possible normalization is

$$
\left\langle\operatorname{Pf}\frac1{|k|},\varphi\right\rangle
=\int_{|k|<1}\frac{\varphi(k)-\varphi(0)}{|k|}\,dk
+\int_{|k|\ge1}\frac{\varphi(k)}{|k|}\,dk.
$$

It satisfies $k\operatorname{Pf}(1/|k|)=\operatorname{sgn}k$. The general solution of $kT=0$ is a multiple of the [Dirac delta distribution](../../../../../../../dirac-delta-function.md): a [test function](../../../../../../../test-function.md) vanishing at zero can be written $k\psi(k)$, so $T$ depends only on its value at zero. Consequently the [Fourier transform of the absolute logarithm](../../../../../../../fourier-transform-of-the-absolute-logarithm.md) is

$$
\boxed{\widehat{\log|x|}(k)=-\pi\operatorname{Pf}\frac1{|k|}+C\delta(k)}.
$$

Changing the finite-part normalization changes $C$. The printed reciprocal expression is meaningful with this interpretation, not as an ordinary function at $k=0$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
