<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Draw [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) $Y_1,\ldots,Y_n\sim q$ and use the [importance weight](../../../../../importance-weight.md) $w=p/q$. The [importance sampling](../../../../../importance-sampling.md) estimator is

$$
\boxed{\widehat\theta_n^{\mathrm{IS}}=\frac1n\sum_{i=1}^nw(Y_i)\phi(Y_i).}
$$

The envelope supplies the [support condition for importance sampling](../../../../../support-condition-for-importance-sampling.md). Since $\mathbb E_q[w(Y)\phi(Y)]=\mathbb E_p\phi(X)=\theta$, this is an [unbiased estimator](../../../../../unbiased-estimator.md). Moreover, $0\leq w\leq M$, so

$$
\begin{aligned}
\mathbb E_q[w(Y)^2\phi(Y)^2]
&=\int w(x)\phi(x)^2p(x)\,dx\\
&=\mathbb E_p[w(X)\phi(X)^2]\\
&\leq M\mathbb E_p[\phi(X)^2]
=M(1+\theta^2).
\end{aligned}
$$

Here $\mathbb E_p\phi^2=\operatorname{Var}_p(\phi)+\theta^2=1+\theta^2$. Subtracting the squared [expected value](../../../../../expected-value-split.md) and dividing by $n$ proves the [bounded-weight importance-sampling moment bound](../../../../../bounded-weight-importance-sampling-moment-bound.md) in the requested form:

$$
\boxed{\operatorname{Var}(\widehat\theta_n^{\mathrm{IS}})
=\frac{\mathbb E_p[w\phi^2]-\theta^2}{n}
\leq\frac{M+(M-1)\theta^2}{n}.}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
