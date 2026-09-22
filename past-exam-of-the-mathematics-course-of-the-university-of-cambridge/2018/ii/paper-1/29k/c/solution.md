<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Ignoring the multinomial coefficient, the likelihood is

$$
\begin{aligned}
L(\theta)
&=(1-\theta)^{2n_{AA}}\theta^{2n_{BB}}
[2\theta(1-\theta)]^{n_{AB}}\\
&=2^{n_{AB}}
\theta^{2n_{BB}+n_{AB}}
(1-\theta)^{2n_{AA}+n_{AB}}.
\end{aligned}
$$

The score equation is

$$
\frac{2n_{BB}+n_{AB}}{\theta}
-\frac{2n_{AA}+n_{AB}}{1-\theta}=0,
$$

and strict concavity of the log-likelihood gives

$$
\boxed{\ \widehat\theta_{\rm MLE}
=\frac{2n_{BB}+n_{AB}}{2n}
=\widehat\theta_{w^*}.\ }
$$

Using the variables $Z_i$ from part (b), the [central limit theorem](../../../../../../central-limit-theorem.md) gives

$$
\sqrt n(\widehat\theta_{\rm MLE}-\theta)
=\frac1{\sqrt n}\sum_{i=1}^n(Z_i-\theta)
\xrightarrow{d}
N\left(0,\operatorname{Var}(Z_1)\right).
$$

Therefore the [allele-frequency estimator under Hardy-Weinberg equilibrium](../../../../../../allele-frequency-estimator-under-hardy-weinberg-equilibrium.md) has limiting law

$$
\boxed{\ \sqrt n(\widehat\theta_{\rm MLE}-\theta)
\xrightarrow{d}N\left(0,\frac{\theta(1-\theta)}2\right).\ }
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
