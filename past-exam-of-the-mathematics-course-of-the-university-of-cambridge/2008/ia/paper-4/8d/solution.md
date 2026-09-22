<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

The key [telescoping series](../../../../../telescoping-series.md) identity is

$$
c_k=\frac{(q+k-1)q!}{(q+k)!}=\frac{q!}{(q+k-1)!}-\frac{q!}{(q+k)!}.
$$

For the requested [mathematical induction](../../../../../mathematical-induction.md), when $n=1$ the proposed sum is $q/(q+1)=1-q!/(q+1)!$. If the identity holds for $n$, adding $c_{n+1}=q!/(q+n)!-q!/(q+n+1)!$ cancels its last term and yields $1-q!/(q+n+1)!$. Thus it holds for every $n\geq1$. Since $q!/(q+n)!\to0$ for fixed positive [integer](../../../../../integer.md) $q$, the infinite [series](../../../../../series-mathematics.md) has sum $\boxed{1}$.

For the second [series](../../../../../series-mathematics.md), the integral digit condition is $0\leq a_n\leq n-1$, and in particular $a_1=0$. Its partial sums are increasing and satisfy

$$
0\leq\sum_{n=1}^N\frac{a_n}{n!}\leq\sum_{n=1}^N\frac{n-1}{n!}=1-\frac1{N!}\leq1.
$$

Thus the [bounded monotone sequence theorem](../../../../../bounded-monotone-sequence-theorem.md) proves convergence to a [real number](../../../../../real-number.md) $S\in[0,1]$. The same telescoping calculation gives, for every $N\geq1$,

$$
\sum_{n>N}\frac{n-1}{n!}=\frac1{N!},\qquad R_N:=N!\left(S-\sum_{n=1}^N\frac{a_n}{n!}\right)\in[0,1].
$$

If positive digits occur infinitely often, then every tail contains a positive term, so $R_N>0$. If $a_n\leq n-2$ occurs infinitely often, then every tail contains a digit smaller than its maximum. Indeed,

$$
1-R_N=N!\sum_{n>N}\frac{n-1-a_n}{n!}>0.
$$

Consequently the two conditions together give $0<R_N<1$ for every $N$. Were $S=A/B$ a [rational number](../../../../../rational-number.md), with positive [integer](../../../../../integer.md) $B$, choose $N\geq B$. Because $B\mid N!$, the number $N!S$ is an [integer](../../../../../integer.md), as is $\sum_{n=1}^Na_nN!/n!$. Their difference $R_N$ would be an [integer](../../../../../integer.md) strictly between zero and one, a contradiction.

Conversely, if positive digits occur only finitely often, then $S$ is a finite sum of [rational numbers](../../../../../rational-number.md). If digits below their maximum occur only finitely often, then $a_n=n-1$ for every $n>N$ for some $N$, giving

$$
S=\sum_{n=1}^N\frac{a_n}{n!}+\frac1{N!}\in\mathbb Q.
$$

These are exactly the two ways the conjunction of infinitude conditions can fail. Hence the [irrationality criterion for factorial series](../../../../../irrationality-criterion-for-factorial-series.md) is proved in both directions: **$S$ is irrational exactly when both kinds of digit occur infinitely often.**

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
