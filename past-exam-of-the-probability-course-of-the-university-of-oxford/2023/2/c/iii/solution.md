<h1 id="2/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $X\sim\operatorname{Exp}(\lambda)$, integration gives $M_X(t)=\lambda/(\lambda-t)$ for $t<\lambda$. For $0<c<1$, the candidate remainder [moment-generating function](../../../../../moment-generating-function.md) is

$$
\frac{M_X(t)}{M_X(ct)}=\frac{\lambda-ct}{\lambda-t}=c+(1-c)\frac{\lambda}{\lambda-t}.
$$

This is the [moment-generating function](../../../../../moment-generating-function.md) of the [mixture distribution](../../../../../mixture-distribution.md)

$$
\boxed{\mathcal L(R_c)=c\delta_0+(1-c)\operatorname{Exp}(\lambda).}
$$

Construct it by taking an [exponential random variable](../../../../../exponential-distribution.md) $E$ of rate $\lambda$ and a [Bernoulli random variable](../../../../../bernoulli-distribution.md) $J$ with $\mathbb P(J=1)=1-c$, with $E,J,X$ mutually independent, and setting $R_c=JE$. Then $R_c$ is independent of $X$, and

$$
M_{cX+R_c}(t)=\frac{\lambda}{\lambda-ct}\frac{\lambda-ct}{\lambda-t}=\frac{\lambda}{\lambda-t}=M_X(t)
$$

on a neighborhood of zero. By the [uniqueness theorem for moment-generating functions](../../../../../uniqueness-theorem-for-moment-generating-functions.md), $cX+R_c\overset d=X$, so the [exponential distribution](../../../../../exponential-distribution.md) is a [self-decomposable distribution](../../../../../self-decomposable-distribution.md).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
