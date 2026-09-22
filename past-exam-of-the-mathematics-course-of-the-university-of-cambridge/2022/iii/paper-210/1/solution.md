<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $\lambda\in\mathbb R$, convexity of $u\mapsto e^{\lambda u}$ on $[0,1]$ gives

$$
e^{\lambda u}\leq1-u+ue^\lambda.
$$

Consequently

$$
\mathbb Ee^{\lambda X_i}\leq1-\mu_i+\mu_i e^\lambda.
$$

For $\lambda\geq0$, independence and concavity of $u\mapsto\log\{1+u(e^\lambda-1)\}$ yield

$$
\mathbb Ee^{\lambda n\bar X}
\leq\prod_{i=1}^n\{1-\mu_i+\mu_i e^\lambda\}
\leq\{1-\bar\mu+\bar\mu e^\lambda\}^n.
$$

The [Chernoff bound](../../../../../chernoff-bound.md) therefore gives, for $a=\bar\mu+x$,

$$
\mathbb P(\bar X\geq a)
\leq\inf_{\lambda\geq0}
\exp\left[n\{\log(1-\bar\mu+\bar\mu e^\lambda)-\lambda a\}\right].
$$

For $\bar\mu<a<1$, the minimizer satisfies

$$
e^{\lambda_*}=\frac{a(1-\bar\mu)}{\bar\mu(1-a)}.
$$

Substitution gives the [binary relative entropy](../../../../../binary-relative-entropy.md)

$$
\mathbb P(\bar X-\bar\mu\geq x)
\leq e^{-n\operatorname{kl}(\bar\mu+x,\bar\mu)}.
$$

The endpoint cases follow by continuity.

Put $a=(1+\delta)\bar\mu$. The same calculation, followed by $\log(1-z)\leq-z$, gives

$$
\operatorname{kl}((1+\delta)\bar\mu,\bar\mu)
\geq\bar\mu\{(1+\delta)\log(1+\delta)-\delta\}.
$$

Thus

$$
\mathbb P\{\bar X\geq(1+\delta)\bar\mu\}
\leq
\left\{\frac{e^\delta}{(1+\delta)^{1+\delta}}\right\}^{n\bar\mu}.
$$

The supplied lower bound $\log(1+\delta)\geq2\delta/(2+\delta)$ implies

$$
(1+\delta)\log(1+\delta)-\delta
\geq\frac{\delta^2}{2+\delta},
$$

which proves the second upper-tail estimate. If $(1+\delta)\bar\mu>1$, the event is empty and the same bound remains true.

For the lower tail, apply the exponential-moment argument with $\lambda<0$, or equivalently optimize at $a=(1-\delta)\bar\mu$. It gives

$$
\mathbb P\{\bar X\leq(1-\delta)\bar\mu\}
\leq
\left\{\frac{e^{-\delta}}{(1-\delta)^{1-\delta}}\right\}^{n\bar\mu}.
$$

Finally,

$$
\delta+(1-\delta)\log(1-\delta)\geq\frac{\delta^2}{2}
$$

for $0\leq\delta<1$, yielding $e^{-n\delta^2\bar\mu/2}$; the case $\delta=1$ follows by a limit.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 210](../../paper-210-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
