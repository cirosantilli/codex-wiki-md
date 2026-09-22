<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $S=\sum_iY_i$ and $V_H=\sum_i(b_i-a_i)^2$. To prove the [Hoeffding lemma](../../../../../hoeffding-lemma.md), take a centered [random variable](../../../../../random-variable-split.md) $Y\in[a,b]$ and its [cumulant-generating function](../../../../../cumulant-generating-function.md) $\psi(t)=\log\mathbb E e^{tY}$. Under [exponential tilting](../../../../../exponential-tilting.md), $\psi''(t)$ is the [variance](../../../../../variance-split.md) of $Y$. The [Popoviciu inequality on variances](../../../../../popoviciu-s-inequality-on-variances.md) gives

$$
\psi''(t)\leq\frac{(b-a)^2}{4},
$$

since under any such tilt the support remains $[a,b]$, and $\operatorname{Var}(Y)\leq\mathbb E(Y-(a+b)/2)^2\leq(b-a)^2/4$. Because $\psi(0)=\psi'(0)=0$, integrating twice gives $\psi(t)\leq t^2(b-a)^2/8$ for $t\geq0$; applying the same argument to $-Y$ handles the opposite tail.

The [independence](../../../../../independent-random-variables.md) of the $Y_i$ gives $\mathbb E e^{tS}\leq\exp(t^2V_H/8)$. The [Markov inequality](../../../../../markov-inequality.md), in the [Chernoff bound](../../../../../chernoff-bound.md) argument, yields

$$
\mathbb P(S>\epsilon)\leq\inf_{t>0}\exp\left(-t\epsilon+\frac{t^2V_H}{8}\right)
=\exp\left(-\frac{2\epsilon^2}{V_H}\right),
$$

where the minimum is at $t=4\epsilon/V_H$ when $V_H>0$. Apply the same argument to $-S$ and add the bounds to obtain the [Hoeffding inequality](../../../../../hoeffding-inequality.md):

$$
\boxed{\mathbb P(|S|>\epsilon)\leq2\exp\left(-\frac{2\epsilon^2}{\sum_i(b_i-a_i)^2}\right).}
$$

If $V_H=0$, every centered $Y_i$ is identically zero and the tail probability is zero; the displayed exponential is interpreted by its zero-variance limit.

For the [Bennett inequality](../../../../../bennett-inequality.md), write $v=n\sigma^2$, and first assume $M>0$ and $v>0$. For $j\geq2$, boundedness and centering give

$$
\mathbb E Y_i^j\leq\mathbb E|Y_i|^j\leq M^{j-2}\mathbb EY_i^2\leq\sigma^2M^{j-2}.
$$

For $t\geq0$, expanding the [moment-generating function](../../../../../moment-generating-function.md) and using the permitted interchange of sum and [expected value](../../../../../expected-value.md),

$$
\begin{aligned}
\mathbb E e^{tY_i}
&=1+\sum_{j=2}^\infty\frac{t^j\mathbb EY_i^j}{j!}\\
&\leq1+\frac{\sigma^2}{M^2}(e^{tM}-1-tM)\\
&\leq\exp\left(\frac{\sigma^2}{M^2}(e^{tM}-1-tM)\right).
\end{aligned}
$$

Negative odd [moments](../../../../../moment.md) cause no difficulty because the estimate is an upper bound term by term. The [independence](../../../../../independent-random-variables.md) of the $Y_i$ and the [Chernoff bound](../../../../../chernoff-bound.md) then give

$$
\mathbb P(S>\epsilon)\leq
\inf_{t>0}\exp\left[-t\epsilon+\frac v{M^2}(e^{tM}-1-tM)\right].
$$

The derivative vanishes at $t_*=M^{-1}\log(1+M\epsilon/v)$, and substitution gives $-(v/M^2)\phi(M\epsilon/v)$ with the [Bennett rate function](../../../../../bennett-rate-function.md) $\phi(u)=(1+u)\log(1+u)-u$. The same absolute bounds apply to $-Y_i$, so

$$
\boxed{\mathbb P(|S|>\epsilon)\leq2\exp\left[-\frac{n\sigma^2}{M^2}\phi\left(\frac{M\epsilon}{n\sigma^2}\right)\right].}
$$

If $\sigma^2=0$, all centered $Y_i$ are zero [almost surely](../../../../../almost-sure-convergence.md); if $M=0$, the same is immediate. Handle those cases directly rather than divide by zero. Both derived [concentration inequalities](../../../../../concentration-inequality.md) also hold with $\geq\epsilon$, by the same [Markov inequality](../../../../../markov-inequality.md) argument or by letting a smaller positive threshold increase to $\epsilon$.

For the [binomial distribution](../../../../../binomial-distribution.md), write $X=\sum_{i=1}^nZ_i$ with [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) $Z_i$ having the [Bernoulli distribution](../../../../../bernoulli-distribution.md) with parameter $p=p_n$. Then $Y_i=Z_i-p$ has range $[-p,1-p]$, width one, and [variance](../../../../../variance-split.md) $p(1-p)$. For large $n$, $p<1/2$, so $M=1-p$ and $v=np(1-p)$. Set $\epsilon=C\sqrt v$.

The [Hoeffding inequality](../../../../../hoeffding-inequality.md) gives

$$
H_n=2\exp[-2C^2p(1-p)]\longrightarrow2.
$$

After truncation at one, this is asymptotically the trivial probability bound. The [Bennett inequality](../../../../../bennett-inequality.md) instead gives

$$
B_n=2\exp\left[-\frac v{(1-p)^2}\phi\left(\frac{C(1-p)}{\sqrt v}\right)\right].
$$

Since $v\to\infty$ and $\phi(u)=u^2/2+O(u^3)$ by a [Taylor expansion](../../../../../taylor-expansion.md),

$$
\frac v{(1-p)^2}\phi\left(\frac{C(1-p)}{\sqrt v}\right)
=\frac{C^2}{2}+O(v^{-1/2})\longrightarrow\frac{C^2}{2}.
$$

Thus the [Bennett bounds for sparse binomial fluctuations](../../../../../bennett-bounds-for-sparse-binomial-fluctuations.md) yield

$$
\boxed{B_n\longrightarrow2e^{-C^2/2},\qquad H_n\longrightarrow2.}
$$

**The [Bennett inequality](../../../../../bennett-inequality.md) supplies the smaller raw exponential bound for every fixed $C>0$ and all sufficiently large $n$.** If $C\leq\sqrt{2\log2}$, clipping probability upper bounds at one makes both eventually trivial; for $C>\sqrt{2\log2}$, the [Bennett inequality](../../../../../bennett-inequality.md) retains a nontrivial limiting bound. This distinction avoids claiming a probability improvement after clipping when both raw bounds exceed one.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
