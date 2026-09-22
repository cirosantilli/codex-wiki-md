<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Work on the unbiased [Boolean hypercube](../../../../../../boolean-hypercube.md) with values $\{-1,1\}$ for the coordinates and $\{0,1\}$ for $f$. Write its [Fourier-Walsh transform](../../../../../../fourier-walsh-transform.md) as

$$
f=\sum_{A\subseteq[n]}\alpha_A\chi_A,\qquad v=t(1-t)=\sum_{A\ne\varnothing}\alpha_A^2.
$$

The flip-probability [influences](../../../../../../influence-of-a-variable.md) satisfy

$$
\beta_i=4\sum_{A\ni i}\alpha_A^2,\qquad I:=\sum_i\beta_i=4\sum_A|A|\alpha_A^2.
$$

These factors of four are essential for zero-one $f$. If $v=0$, the conclusion is immediate. Otherwise suppose, for a contradiction, that $I<2bv$, where $b=\log(1/\beta)/3$. Take $\beta$ small enough that $b\geq1$. The high-level [Fourier weight](../../../../../../fourier-weight.md) obeys

$$
\sum_{|A|>b}\alpha_A^2\leq\frac{I}{4b}<\frac v2,
\qquad\text{so}\qquad
\sum_{1\leq|A|\leq b}\alpha_A^2>\frac v2.
$$

This proves the first intermediate claim, including when $b$ is not an integer.

Set $\delta=e^{-1}$ and $r=2/(1+\delta)$. For the [discrete derivative of a Boolean function](../../../../../../discrete-derivative-of-a-boolean-function.md), $D_i f$ has magnitude $1/2$ exactly on a set of measure $\beta_i$. [Beckner's inequality](../../../../../../beckner-s-inequality.md), in the precise form $\|T_{\sqrt\delta}g\|_2\leq\|g\|_{1+\delta}$ for the [noise operator on the Boolean hypercube](../../../../../../noise-operator-on-the-boolean-hypercube.md), yields

$$
\sum_A|A|\delta^{|A|-1}\alpha_A^2
=\sum_i\|T_{\sqrt\delta}D_i f\|_2^2
\leq\frac14\sum_i\beta_i^r.
$$

For $1\leq s\leq b$, concavity of $\log s-s+1$ shows that $s\delta^{s-1}$ is at least the smaller endpoint value $\min(1,b\delta^{b-1})$, and this is at least $b\delta^b$ since $be^{-b}\leq1$. Therefore the low-level [Fourier weight](../../../../../../fourier-weight.md) gives the second required intermediate bound:

$$
\sum_i\beta_i^{2/(1+\delta)}\geq2b\delta^b v.
$$

On the other hand, $\beta_i\leq\beta$ and the assumed bound on $I$ give

$$
\sum_i\beta_i^r\leq\beta^{r-1}I<2b\beta^{r-1}v.
$$

Combining these inequalities would imply $\beta^{r-1}>\delta^b=\beta^{1/3}$. But $r-1=(1-\delta)/(1+\delta)>1/3$ and $0<\beta<1$, so the inequality is impossible. Consequently

$$
\boxed{\sum_i\beta_i\geq\frac23t(1-t)\log(1/\beta).}
$$

In fact, this proof needs sufficiently small $\beta$ but no separate lower bound on $n$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
