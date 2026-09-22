<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an exact failure half an hour after entry, use the conditional density, rather than the probability of an event at one exact time:

$$
\boxed{\frac{f(\tau+1/2)}{F(\tau)}=\lambda e^{-\lambda/2}.}
$$

Again this is independent of $\tau$ by [memorylessness of the exponential distribution](../../../../../../../memorylessness-of-the-exponential-distribution.md). Whether successive observed lecture segments came from the same bulb does not affect the conditional [likelihood](../../../../../../../likelihood-function.md): surviving segments of one bulb multiply into its survival exposure, and replacement starts another memoryless lifetime. Assume no unrecorded use relevant to the exposure calculation or, equivalently, condition on the bulb being alive at each observed lecture's start; unobserved ages themselves need not be known.

The observed working exposure is $12+1/2=12.5$ bulb-hours with one failure. Thus

$$
L(\lambda)\propto\lambda e^{-12.5\lambda},\qquad
\boxed{\widehat\lambda=\frac1{12.5}=0.08\ \text{hour}^{-1}.}
$$

Strict concavity of $\log\lambda-12.5\lambda$ verifies the maximum. **Immediate replacement would increase observed working exposure to 13 hours**, since the replacement survives the remaining half hour, giving

$$
\boxed{L_{\mathrm{replaced}}(\lambda)\propto\lambda e^{-13\lambda},\qquad
\widehat\lambda_{\mathrm{replaced}}=\frac1{13}\approx0.07692\ \text{hour}^{-1}.}
$$

For the alternative [Weibull distribution](../../../../../../../weibull-distribution.md) and [unknown entry age in a Weibull survival segment](../../../../../../../unknown-entry-age-in-a-weibull-survival-segment.md), keep its different inverse-scale convention: $F(t)=\exp[-(\lambda t)^p]$. Conditional survival for an additional duration $u$ is

$$
\frac{F(\tau+u)}{F(\tau)}
=\exp\{-\lambda^p[(\tau+u)^p-\tau^p]\},
$$

and the conditional failure density after $u$ is

$$
p\lambda^p(\tau+u)^{p-1}
\exp\{-\lambda^p[(\tau+u)^p-\tau^p]\}.
$$

Both depend on the unknown age unless $p=1$. The available segment data, with ages and bulb identity unrecorded, do not specify the usual Weibull likelihood needed to estimate $\lambda,p$. **Merely collecting more of the same unknown-age records does not fix the missing age/design information.** A larger dataset with documented ages or identities, or a justified model for the entry-age distribution, could permit estimation. If $p=1$ is imposed, the exponential calculation remains valid. The issue is loss of memorylessness and unspecified entry history, not a universal impossibility of learning from any larger bulb experiment.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 35](../../../../paper-35-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
