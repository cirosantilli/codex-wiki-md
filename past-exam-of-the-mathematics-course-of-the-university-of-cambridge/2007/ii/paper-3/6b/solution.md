<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

The pair-birth rate here is the constant immigration rate $\lambda$, while deaths occur at total rate $\beta n$. This interpretation is fixed by the requested mean formula. With $P_n(t)=\Pr(N_t=n)$ and $P_j=0$ for $j<0$, the [master equation](../../../../../master-equation.md) is

$$
\boxed{P_n'=\lambda P_{n-2}+\beta(n+1)P_{n+1}-(\lambda+\beta n)P_n.}
$$

The [Markov jump-process generator](../../../../../markov-jump-process-generator.md) acts as $Lf(n)=\lambda[f(n+2)-f(n)]+\beta n[f(n-1)-f(n)]$. Taking $f(n)=n$ gives $m'=2\lambda-\beta m$, hence

$$
\boxed{m(t)=\frac{2\lambda}{\beta}(1-e^{-\beta t})+n_0e^{-\beta t}.}
$$

For the [second moment](../../../../../second-moment.md) $s=\mathbb E N_t^2$, the two jumps give $s'=4\lambda m+4\lambda-2\beta s+\beta m$. Differentiating $V=s-m^2$ therefore yields $V'=4\lambda+\beta m-2\beta V$. Substitution of the mean and solution of this scalar linear equation give

$$
V(t)=\frac{3\lambda}{\beta}+(V(0)-3\lambda/\beta)e^{-2\beta t}
+(n_0-2\lambda/\beta)(e^{-\beta t}-e^{-2\beta t}).
$$

Thus **$V(t)\to3\lambda/\beta$**, assuming $\beta>0$ and finite initial [second moment](../../../../../second-moment.md). This is [pair immigration with linear deaths](../../../../../pair-immigration-with-linear-deaths.md); births at rate $\lambda n$ would be a different model and would not give the printed mean.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
