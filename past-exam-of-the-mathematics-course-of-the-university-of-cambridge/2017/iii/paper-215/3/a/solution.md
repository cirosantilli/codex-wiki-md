<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On a finite state space with at least two states, as in the surrounding questions, for a real function write $\pi(f)=\sum_x\pi(x)f(x)$ and $\operatorname{Var}_\pi(f)=\sum_x\pi(x)(f(x)-\pi(f))^2$. The [Poincare inequality for a reversible Markov chain](../../../../../../poincare-inequality-for-a-reversible-markov-chain.md) with constant $C$ is

$$
\boxed{\operatorname{Var}_\pi(f)\leq C\mathcal E(f,f)\quad\text{for every }f,}
$$

where the [Dirichlet form of a Markov chain](../../../../../../dirichlet-form-of-a-markov-chain.md) is

$$
\mathcal E(f,f)=\frac12\sum_{x,y}\pi(x)P(x,y)(f(x)-f(y))^2=\langle f,(I-P)f\rangle_\pi.
$$

The associated [spectral gap](../../../../../../spectral-gap.md) is the ordinary gap $\gamma=1-\lambda_2$, with variational formula

$$
\boxed{\gamma=\inf_{\operatorname{Var}_\pi(f)>0}\frac{\mathcal E(f,f)}{\operatorname{Var}_\pi(f)}.}
$$

Equivalently minimize $\mathcal E(f,f)$ subject to $\pi(f)=0$ and $\langle f,f\rangle_\pi=1$. Thus the [Poincare inequality for a reversible Markov chain](../../../../../../poincare-inequality-for-a-reversible-markov-chain.md) holds precisely for $C\geq1/\gamma$, and the optimal constant is $1/\gamma$. It controls the ordinary rather than absolute [spectral gap](../../../../../../spectral-gap.md), so negative [eigenvalues](../../../../../../eigenvalue.md) do not invalidate it. If the unspecified state space in this part is infinite, the [Poincare inequality for a reversible Markov chain](../../../../../../poincare-inequality-for-a-reversible-markov-chain.md) and the variational infimum still make sense on nonconstant functions in $L^2(\pi)$, using the [self-adjoint operator](../../../../../../self-adjoint-operator.md) on that [Hilbert space](../../../../../../hilbert-space-split.md); the resulting [spectral gap](../../../../../../spectral-gap.md) need not be represented by an actual second [eigenvalue](../../../../../../eigenvalue.md). The finite-state formula above is the intended specialization.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 215](../../../paper-215-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
