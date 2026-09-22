<h1 id="18h/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The unrestricted [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md) remain $(\bar X,\bar Y)$. Subject to the null constraint, minimizing $(\mu_X-\bar X)^2$ on $[A,\infty)$ gives $\widehat\mu_X=\max(A,\bar X)$, while $\widehat\mu_Y=0$. Consequently

$$
\boxed{T=-2\log\Lambda=n[\bar Y^2+(A-\bar X)_+^2],\qquad \text{reject if }T>c_\alpha.}
$$

We must calibrate this [likelihood-ratio test](../../../../../../likelihood-ratio-test.md) over the entire composite null. Under that null let $W=\sqrt n(\bar X-A)$ and $Z=\sqrt n\bar Y$. Then $W\sim N(\delta,1)$ with $\delta=\sqrt n(\mu_X-A)\geq0$, while $Z\sim N(0,1)$ independently, and $T=Z^2+(-W)_+^2$. Couple all null distributions by $W=W_0+\delta$, with a fixed standard Gaussian $W_0$. Increasing $\delta$ decreases $(-W_0-\delta)_+^2$ pointwise, so the largest rejection probability occurs at $\delta=0$, namely $\mu_X=A$.

At this boundary the sign of $W$ is independent of $W^2$, with each sign having probability one half. On $W\geq0$, $T=Z^2\sim\chi_1^2$; on $W<0$, $T=Z^2+W^2\sim\chi_2^2$. Thus the least favourable [null hypothesis](../../../../../../null-hypothesis.md) law is the exact [chi-bar-squared distribution](../../../../../../chi-bar-squared-distribution.md) $\tfrac12\chi_1^2+\tfrac12\chi_2^2$. Choose $c_\alpha>0$ by

$$
\boxed{\frac12\mathbb P(\chi_1^2>c_\alpha)+\frac12\mathbb P(\chi_2^2>c_\alpha)=\alpha,\quad\text{equivalently }1-\Phi(\sqrt{c_\alpha})+\frac12e^{-c_\alpha/2}=\alpha.}
$$

The tail is a [continuous function](../../../../../../continuous-function.md) and strictly decreasing from one to zero, so this threshold is unique for $0<\alpha<1$. The null rejection probability is at most $\alpha$ and equals $\alpha$ at $\mu_X=A$. This proves the required size, rather than using an interior chi-squared approximation.

To compare, put $c_1=z_{1-\alpha/2}^2$, the threshold in (i). Since $\chi_2^2$ is stochastically larger than $\chi_1^2$ (add an independent squared standard Gaussian), the mixture threshold obeys $c_\alpha>c_1$. When $\bar X\geq A$, test (ii) therefore requires stronger evidence from $\bar Y$ than test (i). When $\bar X<A$, test (ii) also responds to violation of the mean constraint and can reject even with $\bar Y=0$. **Neither critical region contains the other.** In the coordinates $(W,Z)$, the acceptance region in (i) is the strip $|Z|\leq\sqrt{c_1}$; in (ii) it is the right half-strip $W\geq0$, $|Z|\leq\sqrt{c_\alpha}$ together with the left half-disk $W<0$, $W^2+Z^2\leq c_\alpha$. The extra constraint changes both the statistic and its correct null calibration.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [18H](../../18h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
