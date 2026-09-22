<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

The [indicator function](../../../../../indicator-function.md) $I_A$ equals one when the [event](../../../../../event.md) $A$ occurs and zero otherwise. Its [expected value](../../../../../expected-value.md) is $\mathbb E I_A=\mathbb P(A)$. By [linearity of expectation](../../../../../linearity-of-expectation.md), no [independence](../../../../../independent-random-variables.md) assumption is needed to obtain

$$
\boxed{\mathbb E N=\sum_{i=1}^n p_i.}
$$

Since $I_iI_j=I_{A_i\cap A_j}$, including $p_{ii}=p_i$, the [variance](../../../../../variance-split.md) is

$$
\boxed{\operatorname{Var}N=\sum_{i,j=1}^n(p_{ij}-p_ip_j)=\sum_i p_i(1-p_i)+2\sum_{i<j}(p_{ij}-p_ip_j).}
$$

In particular, correlations between the [events](../../../../../event.md) cannot simply be discarded.

Write $\mu=\mathbb E N$. If $\mu>0$, then $N=0$ implies $|N-\mu|\ge\mu$. Applying [Chebyshev's inequality](../../../../../chebyshev-inequality.md) therefore gives

$$
\boxed{\mathbb P(N=0)\le\frac{\operatorname{Var}N}{\mu^2}.}
$$

Equivalently, the contribution of $N=0$ to $\mathbb E[(N-\mu)^2]$ is $\mu^2\mathbb P(N=0)$. **A positive mean is necessary for the displayed ratio to be defined.** If $\mu=0$, nonnegativity instead gives $N=0$ almost surely, and the printed ratio would be $0/0$.

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
