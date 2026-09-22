<h1 id="2/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the deterministic weights $a_{n,k}=\sqrt{k}/n$. Their squared sum and maximum are

$$
\sum_{k=1}^na_{n,k}^2=\frac{n+1}{2n}\longrightarrow\frac12,
\qquad \max_{k\leq n}|a_{n,k}|=n^{-1/2}\longrightarrow0.
$$

To apply the [quadratic expansion of a cumulant-generating function](../../../../../quadratic-expansion-of-a-cumulant-generating-function.md) rigorously, write $\log M_X(u)=u^2/2+r(u)$, with $r(u)=o(u^2)$. Fix $t\ne0$ and let

$$
\eta_n=\sup_{0<|u|\leq|t|/\sqrt n}\frac{|r(u)|}{u^2}\longrightarrow0.
$$

All arguments $t\sqrt{k}/n$ lie in this shrinking interval. Consequently

$$
\left|\sum_{k=1}^nr\!\left(\frac{t\sqrt{k}}n\right)\right|
\leq\eta_n\frac{t^2}{n^2}\sum_{k=1}^nk
=\eta_n\frac{t^2(n+1)}{2n}\longrightarrow0.
$$

Taking logs of the [moment-generating function](../../../../../moment-generating-function.md) and using [independence of random variables](../../../../../independent-random-variables.md) now gives

$$
\log M_{T_n}(t)=\frac{t^2}{2n^2}\sum_{k=1}^nk+o(1)
\longrightarrow\frac{t^2}{4}.
$$

The case $t=0$ is immediate. Since $e^{t^2/4}$ is the [moment-generating function](../../../../../moment-generating-function.md) of a [normal distribution](../../../../../normal-distribution.md) of variance $1/2$, the [convergence theorem for moment-generating functions](../../../../../convergence-theorem-for-moment-generating-functions.md) gives

$$
\boxed{T_n\xrightarrow dN\!\left(0,\frac12\right).}
$$

This is a [weighted central limit theorem with negligible maximum weight](../../../../../weighted-central-limit-theorem-with-negligible-maximum-weight.md). Its limit variance also agrees with the exact value $\operatorname{Var}(T_n)=(n+1)/(2n)$ from [variance additivity for independent random variables](../../../../../variance-additivity-for-independent-random-variables.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
