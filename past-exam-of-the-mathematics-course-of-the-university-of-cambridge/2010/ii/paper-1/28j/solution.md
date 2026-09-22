<h1 id="28j/solution">Solution</h1>

↑ **Parent:** [28J](../28j.md)

For $1\leq x\leq n$, conditional binomial probabilities can be written

$$
p_\phi(x)=\binom nx\exp\{\phi x-k(\phi)\},\qquad
\boxed{T=X,\quad\phi=\log\frac{\Pi}{1-\Pi},\quad
k(\phi)=\log\bigl[(1+e^\phi)^n-1\bigr].}
$$

This [zero-truncated binomial distribution](../../../../../zero-truncated-binomial-distribution.md) is an [exponential family](../../../../../exponential-family-split.md). Write $q=1-\pi$ and $s=1-q^n$. The cumulant identities $\mathbb EX=k'$ and $\operatorname{Var}X=k''$, with $d\pi/d\phi=\pi q$, give

$$
\boxed{\mathbb EX=\frac{n\pi}s,\qquad
\operatorname{Var}X=\frac{n\pi q}s-
\frac{n^2\pi^2q^n}{s^2}.}
$$

The [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md) score equation is $X=k'(\widehat\phi)$, or

$$
\boxed{X=\frac{n\widehat\Pi}{1-(1-\widehat\Pi)^n}.}
$$

For $n\geq2$ and $1<X<n$ the increasing mean function gives a unique interior solution; $X=1$ and $X=n$ instead give limiting estimates zero and one, respectively. If $n=1$, $X=1$ always and the parameter is unidentifiable.

For fixed $\pi\in(0,1)$ and large $n$, the excluded event has exponentially small probability $(1-\pi)^n$. Conditioning therefore does not change the central-limit approximation for $X/n$, and the score equation differs from $\widehat\Pi=X/n$ only by an exponentially small correction with high probability. The binomial [central limit theorem](../../../../../central-limit-theorem.md) consequently gives

$$
\boxed{\widehat\Pi\ \dot\sim\ \mathcal N\left(\pi,\frac{\pi(1-\pi)}n\right).}
$$

The suggested inference after observing one is **incorrect for the stated sampling model**. Its conditional likelihood is the unconditioned likelihood divided by $1-(1-\Pi)^n$, a parameter-dependent factor. They are not proportional likelihoods: the unconditioned estimate is $1/n$, whereas the conditional likelihood for $X=1$ is maximized as $\Pi\downarrow0$ for $n>1$. Knowing that the observed value is positive does not remove the selection mechanism from the model.

## ↑ Ancestors (10)

1. [28J](../28j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
