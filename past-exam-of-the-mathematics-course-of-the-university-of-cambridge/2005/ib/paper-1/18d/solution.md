<h1 id="18d/solution">Solution</h1>

↑ **Parent:** [18D](../18d.md)

A [simple hypothesis](../../../../../simple-hypothesis.md) specifies the entire probability distribution. A [critical region](../../../../../rejection-region.md) $C$ is the set of observations for which the [null hypothesis](../../../../../null-hypothesis.md) is rejected. The [size of a statistical test](../../../../../size-of-a-statistical-test.md) is $\sup_{\theta\in H_0}\Pr_\theta(X\in C)$, which reduces to $\Pr_0(C)$ for a [simple hypothesis](../../../../../simple-hypothesis.md). The [power function](../../../../../power-function-of-a-statistical-test.md) is $\Pr_\theta(C)$ as a function of the true parameter or distribution. At a specified alternative, the [Type II error](../../../../../type-i-and-type-ii-errors.md) probability is $\Pr_\theta(C^c)=1-\Pr_\theta(C)$, the chance of failing to reject a false [null hypothesis](../../../../../null-hypothesis.md). The [Type I error](../../../../../type-i-and-type-ii-errors.md) probability is the corresponding rejection probability under the [null hypothesis](../../../../../null-hypothesis.md).

The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) says that, for two [simple hypotheses](../../../../../simple-hypothesis.md), a test rejecting where $f_1>kf_0$, accepting where $f_1<kf_0$, and if necessary randomizing on equality to achieve prescribed size $\alpha$, has maximal [statistical power](../../../../../statistical-power.md) among tests of size at most $\alpha$. Conversely a most powerful test can be taken in this [likelihood ratio](../../../../../likelihood-ratio.md) form, up to equality sets and null sets.

Here the [likelihood ratio](../../../../../likelihood-ratio.md) for $x\ne0$ is

$$
\frac{f_1(x)}{f_0(x)}=\sqrt{\frac2\pi}\frac1{|x|}.
$$

Its value is infinite at $0$, which has probability zero under both continuous distributions. Large [likelihood ratios](../../../../../likelihood-ratio.md) correspond to small $|x|$. Thus the best [critical region](../../../../../rejection-region.md) is $|X|<c_\alpha$, where

$$
\alpha=\int_{-c_\alpha}^{c_\alpha}\frac12|x|e^{-x^2/2}\,dx
=1-e^{-c_\alpha^2/2}.
$$

There is no boundary randomization to worry about. The complete answer is

$$
\boxed{\text{reject if }|X|<\sqrt{-2\log(1-\alpha)},\qquad
\text{power}=2\Phi\!\left(\sqrt{-2\log(1-\alpha)}\right)-1}.
$$

For the [minimum sum of errors in a simple hypothesis test](../../../../../minimum-sum-of-errors-in-a-simple-hypothesis-test.md), write the error sum as $\int_Cf_0+\int_{C^c}f_1$. At each observation its smaller contribution is obtained by rejecting exactly where $f_1>f_0$. This proves optimality over all tests, including randomized ones, rather than just optimizing within an assumed family. Here it gives $c_*=\sqrt{2/\pi}$, and therefore

$$
\boxed{\alpha_*=1-e^{-1/\pi}\approx0.2726}.
$$

The minimum error sum is $1-e^{-1/\pi}+2[1-\Phi(\sqrt{2/\pi})]$. This criterion weights the two error probabilities equally; it does not impose a conventional $5\%$ [significance level](../../../../../significance-level.md).

## ↑ Ancestors (10)

1. [18D](../18d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
