<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

[Conditional entropy](../../../../conditional-entropy.md) is $H(U\mid V)=\sum_vP(V=v)H(U\mid V=v)$. Factor the joint probabilities as $P(U=u,V=v)=P(V=v)P(U=u\mid V=v)$ and expand their logarithms. This gives $H(X,Y)=H(Y)+H(X\mid Y)$. Applying the same identity within each conditional law given $Z=z$ and averaging gives $H(X,Y\mid Z)=H(X\mid Z)+H(Y\mid X,Z)$.

Put $E=\mathbf1_{\{X\ne Y\}}$ and $\varepsilon=P(E=1)$. Since $E$ is a function of $X,Y$, the conditional [chain rule](../../../../chain-rule.md) gives

$$
H(X\mid Y)=H(E\mid Y)+H(X\mid E,Y).
$$

By [Gibbs inequality](../../../../gibbs-inequality.md), the first term is at most $h(\varepsilon)\le1$. When $E=0$, $Y$ determines $X$. When $E=1$, there are at most $n-1$ possibilities for $X$ given $Y$, so its [conditional entropy](../../../../conditional-entropy.md) is at most $\log_2(n-1)$. Therefore

$$
H(X\mid Y)\le h(\varepsilon)+\varepsilon\log_2(n-1)\le1+\varepsilon\log_2(n-1).
$$

For $n>2$, rearrangement proves

$$
\boxed{P(X\ne Y)\ge\frac{H(X\mid Y)-1}{\log_2(n-1)}}.
$$

The printed division presupposes $n>2$. For $n=2$ its denominator is zero, and the meaningful statement is the stronger undivided inequality $H(X\mid Y)\le h(\varepsilon)$. For $n=1$ the variables agree surely.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
