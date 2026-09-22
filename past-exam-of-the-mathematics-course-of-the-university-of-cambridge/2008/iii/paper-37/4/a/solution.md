<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Brownian reflection principle](../../../../../../reflection-principle-wiener-process.md) gives, for $t>0$,

$$
\mathbb P(\tau_x\leq t)=\mathbb P\left(\sup_{s\leq t}X_s\geq x\right)=2\mathbb P(X_t\geq x)=2\left(1-\Phi\left(\frac x{\sqrt t}\right)\right).
$$

For a standard [normal random variable](../../../../../../gaussian-random-variable.md) $N'$, this is also $\mathbb P(|N'|\geq x/\sqrt t)=\mathbb P(x^2/(N')^2\leq t)$. Thus the [inverse-square Gaussian law of Brownian first passage](../../../../../../inverse-square-gaussian-law-of-brownian-first-passage.md) is

$$
\boxed{\tau_x\overset d=\frac{x^2}{(N')^2}.}
$$

In particular, $\tau_x$ is finite almost surely.

The [Brownian motions](../../../../../../brownian-motion-split.md) $X,Y$ are independent, so conditional on $\tau_x=s$, the ordinate $Y_{\tau_x}$ has the same distribution as $\sqrt s\,N$, with $N$ a standard normal independent of the random time. By [Brownian scaling](../../../../../../brownian-scaling.md) and the hitting-time identity,

$$
Y_{\tau_x}\overset d=\frac{xN}{|N'|}\overset d=\frac{xN}{N'}.
$$

The last equality uses symmetry of $N$ and independence of $N,N'$: inserting the independent sign of $N'$ does not change the distribution of the numerator. Therefore

$$
\boxed{Y_{\tau_x}\overset d=xC,\qquad C\text{ standard Cauchy}.}
$$

For completeness, the ratio has density $\int_{\mathbb R}|v|\varphi(cv)\varphi(v)\,dv=1/(\pi(1+c^2))$, where $\varphi$ is the standard normal density. The scaled exit ordinate has density $x/(\pi(x^2+y^2))$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
