<h1 id="28l/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Given $X=x$, the [posterior expected loss](../../../../../../../posterior-expected-loss.md) from reporting $d$ is

$$
\begin{aligned}
\mathbb E\!\left[\theta^{-1}(\theta-d)^2\mid X=x\right]
&=\mathbb E(\theta\mid X=x)-2d
+d^2\mathbb E(\theta^{-1}\mid X=x).
\end{aligned}
$$

This is a strictly convex quadratic in $d$ whenever the conditional inverse moment is finite and positive. Differentiating with respect to $d$ gives

$$
-2+2d\,\mathbb E(\theta^{-1}\mid X=x)=0,
$$

so the [Bayes estimator under reciprocal weighted quadratic loss](../../../../../../../bayes-estimator-under-reciprocal-weighted-quadratic-loss.md) is

$$
\boxed{\delta_\pi(x)
=\big(\mathbb E(\theta^{-1}\mid X=x)\big)^{-1}}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [28L](../../../28l.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
