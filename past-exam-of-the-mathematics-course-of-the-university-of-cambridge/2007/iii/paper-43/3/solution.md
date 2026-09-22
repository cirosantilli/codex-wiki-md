<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [logit link](../../../../../logit.md) makes the probability constant within each group: write $p_i=\{1+\exp[-(\mu+\alpha_i)]\}^{-1}$, with $\alpha_1=0$. Let $S_i=\sum_{j=1}^kY_{ij}$ and $N=km$. [Independence](../../../../../independent-random-variables.md) gives $S_i\sim\operatorname{Bin}(N,p_i)$. Up to terms independent of the parameters, the log [likelihood](../../../../../likelihood-function.md) is

$$
\ell(\mu,\alpha)=\sum_{i=1}^n\{S_i(\mu+\alpha_i)-N\log(1+e^{\mu+\alpha_i})\}.
$$

The [likelihood](../../../../../likelihood-function.md) equations are

$$
\boxed{\sum_{i=1}^n(S_i-N\widehat p_i)=0,\qquad S_i-N\widehat p_i=0\quad(i=2,\ldots,n).}
$$

Together they also imply $S_1-N\widehat p_1=0$. Thus, when all totals satisfy $0<S_i<N$,

$$
\widehat p_i=S_i/N,\qquad
\boxed{\widehat\mu=\log\frac{S_1}{N-S_1},\qquad\widehat\alpha_i=\log\frac{S_i}{N-S_i}-\widehat\mu.}
$$

The group logits are unconstrained apart from their parametrization, and each binomial log [likelihood](../../../../../likelihood-function.md) is strictly concave in its logit, so these equations give the unique finite maximum. A total of $0$ or $N$ instead gives a boundary probability and an infinite logit; a finite [MLE](../../../../../maximum-likelihood-estimator.md) need not exist in that case.

For $n=2$, keep $0<p_1,p_2<1$ fixed and let $N=km\to\infty$. Since $\widehat p_1=S_1/N$, the [central limit theorem](../../../../../central-limit-theorem.md) gives $\sqrt N(\widehat p_1-p_1)\xrightarrow{d}N(0,p_1(1-p_1))$. The [derivative](../../../../../derivative.md) of the logit is $1/[p_1(1-p_1)]$, so the [delta method](../../../../../delta-method.md) gives the [baseline logit estimator in a group-factor binomial model](../../../../../baseline-logit-estimator-in-a-group-factor-binomial-model.md) law

$$
\boxed{\sqrt{km}(\widehat\mu-\mu)\xrightarrow{d}N\left(0,\frac1{p_1(1-p_1)}\right),\qquad
\widehat\mu\ \dot\sim\ N\left(\mu,\frac1{km\,p_1(1-p_1)}\right).}
$$

The second group does not improve the baseline estimate because it has its own free offset. Equivalently, the [Fisher information matrix](../../../../../fisher-information-matrix.md) for $(\mu,\alpha_2)$ is

$$
I=\begin{pmatrix}w_1+w_2&w_2\\w_2&w_2\end{pmatrix},\qquad
I^{-1}=\begin{pmatrix}1/w_1&-1/w_1\\-1/w_1&1/w_1+1/w_2\end{pmatrix},\qquad
w_i=km\,p_i(1-p_i).
$$

Its first diagonal entry confirms the same asymptotic [variance](../../../../../variance-split.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
