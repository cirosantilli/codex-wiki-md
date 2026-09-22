<h1 id="2/2/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\tau_n$ be the first exit from a compact interval on which $H<n$, chosen so that $\tau_n\uparrow T$, and let $m=\inf H> -\infty$. By [Itô formula](../../../../../../../ito-s-lemma.md),

$$
dH(X_t)=H'(X_t)dB_t+\left(\frac12H''(X_t)-H'(X_t)^2\right)dt.
$$

The assumption gives the drift bound $\frac12H''-(H')^2\leq C$. After stopping,

$$
\mathbb E[H(X_{t\wedge\tau_n})]\leq H(x)+Ct.
$$

If $h_n=\inf\{H(y):y\text{ lies outside the }n\text{th compact interval}\}$, then $h_n\to\infty$ because $H$ is [coercive](../../../../../../../coercive-bilinear-form.md), and

$$
(h_n-m)\mathbb P(\tau_n\leq t)
\leq H(x)+Ct-m.
$$

Thus $\mathbb P(T\leq t)=0$ for every $t$, and **$T=\infty$ almost surely**.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2](../../2.md)
3. [2](../../../2.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
