<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the uniform probability measure on the [Boolean hypercube](../../../../../../boolean-hypercube.md). In the [Fourier-Walsh transform](../../../../../../fourier-walsh-transform.md) convention $\chi_S(x)=(-1)^{\sum_{i\in S}x_i}$, write $f=\sum_S\alpha_S\chi_S$ with $\alpha_S=\mathbb E[f\chi_S]$. For the indicator $f$, [Parseval's identity](../../../../../../parseval-identity.md) gives

$$
\alpha_\varnothing=t,\qquad\sum_S\alpha_S^2=t,\qquad\sum_{S\ne\varnothing}\alpha_S^2=t(1-t).
$$

The flip-probability [influence](../../../../../../influence-of-a-variable.md) satisfies $\beta_i=4\sum_{S\ni i}\alpha_S^2$, and summing gives $\sum_{S\ne\varnothing}|S|\alpha_S^2=\frac14\sum_i\beta_i$.

For $p=1+\delta\in(1,2)$, [Beckner's inequality](../../../../../../beckner-s-inequality.md) says $\|T_{\sqrt\delta}g\|_2\leq\|g\|_p$. Apply it to the [discrete derivative of a Boolean function](../../../../../../discrete-derivative-of-a-boolean-function.md) in coordinate $i$, viewed on the other $n-1$ coordinates. Its nonzero magnitude is $1/2$ and occurs with probability $\beta_i$, so

$$
\sum_{S\ni i}\delta^{|S|-1}\alpha_S^2\leq\frac14\beta_i^{2/p}.
$$

Summing over $i$ gives the [hypercontractive weighted influence bound](../../../../../../hypercontractive-weighted-influence-bound.md)

$$
\boxed{\sum_{S\ne\varnothing}|S|\delta^{|S|-1}\alpha_S^2\leq\frac14\sum_i\beta_i^{2/p}.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
