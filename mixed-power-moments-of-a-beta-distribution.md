# Mixed power moments of a beta distribution

↑ **Parent:** [Beta distribution](beta-distribution.md)

For $X\sim\operatorname{Beta}(\alpha,\beta)$ with positive parameters, and real $s>-\alpha$, $t>-\beta$, multiply its density by $x^s(1-x)^t$. The resulting integral is a [beta function](beta-function.md) with shifted parameters, hence

$$
\mathbb E[X^s(1-X)^t]=\frac{\Gamma(\alpha+\beta)\Gamma(\alpha+s)\Gamma(\beta+t)}{\Gamma(\alpha)\Gamma(\beta)\Gamma(\alpha+\beta+s+t)}.
$$

The restrictions on the powers are exactly the endpoint-[integrability](integrability.md) conditions. This includes ordinary [moments](moment.md), reciprocal [moments](moment.md) when they exist, and quantities involving both the occupied fraction $X$ and remaining fraction $1-X$. In particular, $s=1,t=0$ gives $\mathbb E[X]=\alpha/(\alpha+\beta)$.[NIST DLMF §5.12, equation 5.12.1](nist-digital-library-of-mathematical-functions/5-12-beta-function.md)

## ↑ Ancestors (7)

1. [Beta distribution](beta-distribution.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/9/b/ii/solution.md)
