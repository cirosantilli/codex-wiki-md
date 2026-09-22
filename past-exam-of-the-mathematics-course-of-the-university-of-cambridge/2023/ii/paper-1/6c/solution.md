<h1 id="6c/solution">Solution</h1>

↑ **Parent:** [6C](../6c.md)

With population $n$, the transition diagram has the two outgoing arrows

$$
n\xrightarrow{\lambda}n+3,
\qquad
n\xrightarrow{\beta n}n-1.
$$

Thus this is a [batch-birth linear-death process](../../../../../batch-birth-linear-death-process.md). If $P_n(t)=\mathbb P(N_t=n)$ and $P_j=0$ for $j<0$, probability enters state $n$ from $n-3$ by a birth and from $n+1$ by a death. Hence the master equation is

$$
\boxed{
\dot P_n
=\lambda P_{n-3}+\beta(n+1)P_{n+1}
 -(\lambda+\beta n)P_n
}.
$$

The [Markov jump-process generator](../../../../../markov-jump-process-generator.md) is

$$
(Lf)(n)=\lambda\bigl(f(n+3)-f(n)\bigr)
       +\beta n\bigl(f(n-1)-f(n)\bigr).
$$

For $f(n)=n$, this gives $Ln=3\lambda-\beta n$. Therefore the [expected value](../../../../../expected-value.md) $m(t)=\mathbb E[N_t]$ satisfies

$$
m'=3\lambda-\beta m,
\qquad m(0)=n_0,
$$

so

$$
\boxed{
m(t)=\frac{3\lambda}{\beta}(1-e^{-\beta t})+n_0e^{-\beta t}
}.
$$

For $f(n)=n^2$,

$$
Ln^2
=\lambda(6n+9)+\beta n(-2n+1).
$$

Writing $s=\mathbb E[N_t^2]$ and using the generator identity gives

$$
s'=6\lambda m+9\lambda-2\beta s+\beta m.
$$

The [variance](../../../../../variance-split.md) $v=s-m^2$ consequently obeys

$$
\begin{aligned}
v'&=s'-2mm'\\
  &=9\lambda+\beta m-2\beta v.
\end{aligned}
$$

If $v(0)=v_0<\infty$, substitution of the formula for $m$ yields

$$
v(t)=v_0e^{-2\beta t}
 +\frac{6\lambda}{\beta}(1-e^{-2\beta t})
 +\left(n_0-\frac{3\lambda}{\beta}\right)
  (e^{-\beta t}-e^{-2\beta t}).
$$

All transient terms vanish, and the [moments of a batch-birth linear-death process](../../../../../moments-of-a-batch-birth-linear-death-process.md) therefore give

$$
\boxed{\operatorname{var}(N_t)\longrightarrow\frac{6\lambda}{\beta}}.
$$

## ↑ Ancestors (10)

1. [6C](../6c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
