<h1 id="26i/solution">Solution</h1>

↑ **Parent:** [26I](../26i.md)

An [exponential family](../../../../../exponential-family-split.md) has density $h(x)\exp\{\phi\cdot T(x)-k(\phi)\}$ on a parameter-independent support. For an [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md) sample, its [likelihood](../../../../../likelihood-function.md) factorizes through $\sum_iT(X_i)$, so the [Fisher-Neyman factorization theorem](../../../../../fisher-neyman-factorization-theorem.md) gives a [sufficient statistic](../../../../../sufficient-statistic.md) whose dimension is the fixed dimension of $T$, independent of sample size.

Expanding the normal log-density gives $\phi_1=\mu/v$, $\phi_2=-1/(2v)$, and

$$
\boxed{k(\phi)=\frac12\log\frac\pi{-\phi_2}-\frac{\phi_1^2}{4\phi_2},\qquad\mathcal F=\{(\phi_1,\phi_2):\phi_1\in\mathbb R,\ \phi_2<0\}.}
$$

The [mean-value parameter](../../../../../mean-parameter-of-an-exponential-family.md) is $\nabla k=(\mathbb EX,\mathbb EX^2)$, hence

$$
\boxed{H_1=-\frac{\Phi_1}{2\Phi_2}=\mu,\qquad H_2=-\frac1{2\Phi_2}+\frac{\Phi_1^2}{4\Phi_2^2}=v+\mu^2.}
$$

For $n\geq2$ and positive sample variance, $\widehat\mu=\bar X$ and $\widehat v=n^{-1}\sum_i(X_i-\bar X)^2$, so $\widehat\Phi_1=\bar X/\widehat v$. For this [normal natural-mean parameter ratio estimator](../../../../../normal-natural-mean-parameter-ratio-estimator.md), the [central limit theorem](../../../../../central-limit-theorem.md) gives asymptotic independent errors for $\widehat\mu$ and $\widehat v$, with variances $v/n$ and $2v^2/n$. Applying the [delta method](../../../../../delta-method.md) to $\mu/v$ yields

$$
\boxed{\sqrt n(\widehat\Phi_1-\Phi_1)\ \xrightarrow{d}\ N\left(0,\frac1v+\frac{2\mu^2}{v^2}\right).}
$$

If $v=v_0$ is known, $\Phi_2=-1/(2v_0)$ is fixed and $\widehat\Phi_1=\bar X/v_0$ has exact distribution $\boxed{N(\Phi_1,1/(nv_0))}$. The variance-estimation contribution $2\mu^2/v^2$ disappears.

## ↑ Ancestors (10)

1. [26I](../26i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
